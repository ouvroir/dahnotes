# Analyse de données et visualisation en Python

2 et 3 novembre 2021, Pier-Luc St-Onge, Calcul Québec

**Objectifs de la formation**:

- charger des données tabulaires
- sélectionner un sous-ensemble de données
- transformer ou corriger des données
- grouper selon les valeurs d'une ou plusieurs variables
- calculer des statistiques descriptives
- visualisation les données manipulées

formation adaptée et traduite en français de [Datacarpentry](https://datacarpentry.org/python-ecology-lesson/)

juypterhub: user16 dat-2021-02

## 1. Données

pandas --> La bibliothèque Pandas fournit des structures de données, produit des graphiques de haute qualité avec *Matplotlib* et s'intègre bien avec d'autres bibliothèques utilisant des tableaux *NumPy* (qui est une autre bibliothèque Python). Python str is object in Pandas, date & time available as data types.

DataFrame --> sert à gérer les données 

attribut <!-- déjà disponible, déjà calculé, il faut juste aller les chercher. Attribut statique--> vs méthode() <!-- doit être calculé et peut contenir des arguments-->

- data = pandas.read_csv()
- data.head(), data.shape <!-- dimensions array []-->, data.columns, data.tail()
- data['column_name'].count() <!-- nb valeurs non nulles-->, .mean(), .std(), .min(), .max()
- data['new_column'] = data['old_column'] with math operation
- data.dtypes: types for each column, add column within crochet
- data.describe(): statistique descriptive, data['column'].unique()<!-- array des valeurs uniques-->, data['column'].nunique() <!-- nb unique-->
- data['column'].astype(), attention compliqué convertir quand valeurs manquantes 
- .plot(kind='bar') 'line'
- .sum
- .unstack () <!-- after a group by de deux propriétés-->

```python
s_plot = sspt.plot(kind='bar', stacked=True,
                   title="Poids total par site et sex")
s_plot.set_xlabel("Site")
s_plot.set_ylabel("Poids (g)")
```



## 2. Sélectionner

- surveys_df**.loc**[0, ['species_id', 'plot_id', 'weight']]

- surveys_df.loc[0, ['species_id', 'plot_id', 'weight']]

- : --> all 

- surveys_df.loc[0:4, 'month':'plot_id']  <!-- use colum names and not colum count--> attention: sélection inclusivement le dernier (4) et (plot_id). Pour exclure : iloc

- rangées an == 2002--> sélection par critère surveys_df[surveys_df['year'] == 2002]. !==, <, >, <=, >=, ~ <!-- inverse d'une sélection-->

- plusieurs critères, parenthèses: & et | 

- Sélection des enregistrements et des colonnes nécessaires:

  ```
  selection = surveys_df[(surveys_df['sex'].isin(["F", "M"])) & 
                         (surveys_df['weight'] > 0)][ ['plot_id', 'sex', 'weight'] ]
  ```

- pandas.isnull : when true, cell is nan

- Pour sélectionner les enregistrements ayant au moins une valeur NaN

  surveys_df[pd.isnull(surveys_df).any(axis=1)]<!-- axis = 1 -> horizontal-->

- dataframe.copy 
- fillna (fill nana), dropna <!-- dataframe avec aucune rangée non définie-->
- df_sans_na.to_csv('lcoation/file_name.csv', index=False)

## 3. Combiner des DataFrame avec Pandas

- pd.concat([list of df], axis = 0) <!-- 0 = vertical-->
- .reset_index(drop=True) élimine colonne de l'index et en refait un nouveau$
- .columns
- .merge(left="table on the left", right="table on the right", left_on=="colum name where intersection", right_on="colum name where intersection"). if junction key identique, on="colum name where intersection". how="left" (inner join), "right", "outer" (union)

## 4. Automatisation du traitement de données

- os --> .mkdir, lsdir

```python
for annee in surveys_df['year'].unique():
    # Créer un nom de fichier unique pour chaque année
    nom_fichier = os.path.join(dossier_annees, "data/surveys_" + str(annee) + ".csv")
    print(nom_fichier)

    # Sélectionner les données complètes de l'année en cours
    surveys_annee = surveys_df[surveys_df['year'] == annee]
    surveys_annee.to_csv(nom_fichier, index=False)

os.listdir(dossier_annees)
```

## 5. Créer des graphiques avec Plotnine

Bien que `matplotlib` soit un module de visualisation  largement répandu, très flexible et puissant, son utilisation est  parfois compliquée. Pour ce chapitre, nous allons utiliser le module `plotnine` qui facilite la création de graphiques hautement informatifs tout en s'intégrant bien avec Pandas. Le fonctionnement de `plotnine` se base sur le module R `ggplot2` et [The Grammar of Graphics](https://link.springer.com/book/10.1007%2F0-387-28695-0) par Leland Wilkinson.

parenthèses pour capter l'objet retourné par Plotnine. Plus tard on va ajouter (+) des options supplémentaire et la somme doit préférablement être sous la forme d'un seul objet qui sera affiché par Jupyter Notebook.

- créer canva: (p9.ggplot(data=surveys_complete))
- Définir les "aesthetics" (ou `aes`) du graphique en sélectionant les variables du DataFrame qui seront "mappées" (via `mapping`) à divers éléments du graphiques. Les plus importants paramètres de `aes` sont : `x`, `y`, `alpha`, `color`, `colour`, `fill`, `linetype`, `shape`, `size` et `stroke`.

```python
# Créer un gabarit
axesWL = p9.ggplot(data=surveys_complete,
                   mapping=p9.aes(x='weight', y='hindfoot_length'))

# Afficher les points
scatterWL = axesWL + p9.geom_point()

# Enregistrer l'image
scatterWL.save("scatterplot.png", width=10, height=10,dpi=300)
```

```python
# Créer un bar chart
(p9.ggplot(data=surveys_complete,
           mapping=p9.aes(x='plot_id'))
    + p9.geom_bar()
)
```

geom [doc](https://plotnine.readthedocs.io/en/stable/api.html#geoms)

```python
(p9.ggplot(data=surveys_complete,
           mapping=p9.aes(x='weight', y='hindfoot_length', color='species_id'))
    + p9.geom_point(alpha=0.1)
    + p9.xlab("Poids (g)") + p9.ylab("Longueur de patte (mm)")
    + p9.scale_x_log10()
    + p9.theme_bw()
    + p9.theme(text=p9.element_text(size=12))
)
```

```python
#Distributions
(p9.ggplot(data=surveys_complete,
           mapping=p9.aes(x='factor(plot_id)',
                          y='weight',
                          color='species_id'))
    + p9.geom_jitter(alpha=0.3)
    + p9.geom_violin(alpha=0, color="grey")
    + p9.scale_y_log10()
)
```

```python
#Lignes à travers le termps

yearly_counts = surveys_complete.groupby(['year', 'species_id'])['species_id'].count()
yearly_counts = yearly_counts.reset_index(name='counts')

(p9.ggplot(data=yearly_counts,
           mapping=p9.aes(x='year',
                          y='counts',
                          color='species_id'))
    + p9.geom_line()
)
```

```python
# 1 graphique par facette
(p9.ggplot(data=surveys_complete,
           mapping=p9.aes(x='weight',
                          y='hindfoot_length',
                          color='species_id'))
    + p9.geom_point(alpha=0.1)
    + p9.facet_wrap('sex')
)

# groupby 
# regrouper par:
# besoins pour le graphique: year, species_id, sex (données de base)

yearly_weight = surveys_complete.groupby(['year',
                                          'species_id',
                                          'sex'])['weight'].mean().reset_index()
(p9.ggplot(data=yearly_weight,
           mapping=p9.aes(x='year',
                          y='weight',
                          color='species_id'))
    + p9.geom_line()
    + p9.facet_wrap('sex')
)
```



```python
# Créer un thème
mon_theme = p9.theme(axis_text_x = p9.element_text(angle = 90))

(p9.ggplot(data=surveys_complete,
           mapping=p9.aes(x='factor(year)'))
    + p9.geom_bar()
    + p9.xlab("Year")
    + p9.theme_bw()
    + mon_theme
)

```



## 6. Matplotlib

