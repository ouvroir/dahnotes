# Éditions critiques numériques et multilinguisme

Atelier du GREN, 26-27 septembre



## Le projet eBalzac: enjeux et questions d'une édition hypertextuelle

Andrea Del Lungo, Karolina Suchecka

projet double

1. patrimonialisation: rendre accessible l'œuvre entière de balzac (mise en ligne en 2017: [ebalzac](https://www.ebalzac.com/))
2. possibilité d'interrogation et d'exploitation du texte

### Fonctionnalités partie 1

- correction des textes imprimés par l'auteur, rendre toutes les versions disponibles ainsi que les manuscrits lorsqu'ils sont conservés
- clic pour trouver la définition dans les *Dictionnaires d'autrefois*
- comparaison "par couple" des différentes versions du texte avec logiciel [Médite](http://obvil.lip6.fr/medite/)
  - découverte, même sans lire le texte, que Balzac travaille plutôt par suppression: double de suppressions que d'ajout
  - démontre que le travail créatif de Balzac est aussi fort celui de Flaubert, malgré le mythe de l'écrivain qui écrivait très vite parce qu'il avait des dettes à rembourser
- recherche plein texte: utilisations et nuage de mots de co-occurences (recherche lexicale couplée)

axe hypertexte (2) 

### objectifs

- détection de réemplois (texte d'autres auteurs) en utilisant des fragments de correspondances
- visualisation et cartographie des sources littéraires
- étude des savoirs inscrits dans le texte balzaciens
- analyses stylistiques
- réflexion théorique sur la notion de source, permettant d'affiner les définitions de réemploi, plagiat (homologies), etc-

Corpus cible: 

- œuvre de Balzac dans son ensemble (dont le théâtre et les articles de presses)
- sources potentielles
  - œuvres romanesques de l'époque d'auteurs contemporains ou antérieurs (depuis 1750)
  - ouvrages de littérature panoramique
  - ouvrages scientifiques contemporains
    - physiognomonie
    - phrénologie

Logiciels de détection de réutilisations textuelles

- Tracer, eTRAP
- TextPAIR, ARTFL



## Distant editing : les enjeux des méthodes computationnelles pour la théorie et la pratique éditoriale

Elena Pierazzo, Université de Tours

sorte d'histoire des méthodes computationnelles éditoriales

- *Digital scholarly editing* 2015
- READ project→ transcribus (début en 2016)
- Mike Kestemont, *Artificial Palepgraphy: computational approaches to Identifying Script Types in Medieval Manuscripts*
- eScriptorium

À quoi ressemblera l'édition numérique dans 10ans? 

- faite par des éditeurs ou par des ingénieurs-informaticiens? <!-- ne sommes nous pas la salle qui démontre de l'intersection des deux? grande binarité dans le "eux" vs "nous" -->
- se former
- coopération interdisicplinaire
- éthique

## Discussion

### Dé-spécialisation: l'humaniste tel que celui du florentin du 15e?

Elena

- travail avec les techniciens (convertis en techniciens: humaniste devenu imprimeur)
- ne pas rester dans sa niche, s'investir dans les grandes technologies pour ne pas resté isolé
- présence des humanistes dans les imprimeries a forgé le milieu de l'impression

Andrea

- perspective de la science du texte: permettre à l'édition de prendre forme et trouver sa forme
- pur littéraire qui s'est mis à dialoguer avec d'autres collègues de sciences humaines et avec des informaticiens
- on ne peut pas se mettre à la place des informaticiens, ils seront meilleurs que nous

Claudine Moulin

- cette dichotomie n'a pas sa place vu qu'on travaille avec les informaticiens depuis 30 ans
  - réponse Elena: nouvelles techniques computationnelles sont à un autre niveau. Si on y arrive dans un centre d'humanités numériques, mais qu'en est-il des autres collègues? C'est là qu'on trouve cette dichotomie quand la technologie demande cet engagement
- formations pour les étudiants en *Bachelor of science*
- envisager une progression dans la communication avec "eux"

Emmanuel

- pour collaborer avec des informaticiens, il faut trouver un terrain commun: nos questions doivent être alignées → où sont les points de rencontre sur les enjeux épistémologiques? 
- dépasser la stricte collaboration pour que les questions qui sont propres à notre sujet soient adressées
  - réponse Elena: passer de la *collaboration* à la *coopération*→ passer HN3.0: n'est pas une méthode mais une nouvelle recherche. L'ordinateur ne donne pas des réponses mais des pistes → requiert de la créativité, des nouvelles questions. Demande de la part du département d'informatique à donner un cours HN aux étudiant·e·s en informatique
  - réponse Andrea: au-delà du service → intérêt commun qui a rendu le dialogue possible à parité (2.0). Former une nouvelle génération

Tilar Mazzeo

- cambridge analytica: it understands itself as an organisation that uses digitally produced information in order to tell better stories than we do. Neuroscience (how stories change our minds). 
- if AI is reaching the point where we are no longer the minds thinking the information, if we are no longuer the place in culture where the best and most powerful stories are told, aren't we really in troube? 
- we can't stop AI: maybe our digital productions should attempt to understand how we are able to tell stories that are better than the ones we had
  - réponse Elena: owning the space of digital culture, we can't because we haven't engaged enough into the space
  - 



## Reusing digital editions

Elena Spadini (University of Basel) 

FAIR  →Reuse: maximise poential form datset and research impact

successful stories of reuse: the old bailey online data

- reuse code/tools
- reuse data

how to retrieve the dataset

- web srapping
- accessible dupm
- api
- other query endpoints

open question of versionning (dump = snapshot, API = most recent version)

standardisation <!-- manage standardisation without LOD? -->



## De la transcription automatique vers les éditions numériques avec eScriptorium

Peter Stokes (École pratique des hautes études) 

Kraken: open-source HTR software by Benjamin Kiessling (EPHE)

eScriptorium

- interface web pour faciliter l'utilisation de Kraken
- début en 2019

Limitations of Machine Learning: 

- ML only works if you know the answers in advance
- biases in the data are treasferred directly to the AI
- the data is more important than the software
  - hence it's worth millions to GAFAM
  - hence we should share data



## Discussion

est-ce que vous justifiez également réutilisation de données: perspective pas uniquement d'exploitation et d'avancement scientifique, mais aussi écologique / sustainability? 

- peter: oui, perspective écologique pour réduire la consommation des machines. En pratique c'est pas si évident, il y a toujours des différences (boîte en France qui utilise la chaleur des machines pour chauffer des maisons)

réutilisation: tension entre nécessité de développer selon les spcéificifés des projets et l'envie de permettre la réutilisation

- création d'un modèle est utile et parfois nécessaire
- à quel point la standardisation pré-formatte-t-elle les format épistémologiques possibles? ou à l'inverse, réinventer la roue mais aussi "out of the box"? 
- Elena: niveaux d'ontologie → upper layer ontologies
- la science humaine est une sciences du dissensus: la notion de standard est donc problématique (dissensus dans la structure même des données)

diversifier, proposer une variété des formats pour les données

potentiel didactique de eScriptorium? 

- Peter: introduction à l'IA avec un exemple concret

Tilar: downside of working when we share, we can't control in the way our projects are currently used. Ex: Kraken has come from a military origin, what's its history? Let's say we are using software that is being produced for corporate or military needs: we are creating programs without being able to regulate or control what is happening with it. How do we know we are not being co-opted into expanding government surveillance? 

## Complex Textual Editing through Text Encoding: LEAF-Writer

Diane Jakacki (Bucknell University)



## isidore.science, un instrument d’enrichissement et de recherche pour l’édition critique à l’ère numérique

Stéphane Pouyllau (Huma-Num)

humanum

présentation

- frange d'édition qui ne sont pas passées en TEI
- détournement d'isidore pour expliquer qu'avec les techniques du web sémantiques et l'entraînement de AI, on arrive à post-traiter des textes

isidore: contenus de recherche

- rechercher
- trier, classer, partager
- découvrir

isidore.science avec AI

- suggestion de lectures
- métadonnées de description des textes

### sérendipité

encyclopédies sur CD-ROMS: 

- documents assez peu structurés
- capacité de les exhumer et les refactoriser
- BD des années 90 et début 2000, peu standardisées, bases artisanales peu interopérables ou standards mais ça fonctionne 

hn lab: pratique notamment de dresser des IA pour reconstituer des parcours dans des anciennes BD sur CD-ROM

### Enrichissements et structurations

textes peu structurés

structuration doit s'appuyer sur de l'information pertinente, riche et reliée (pour nourrir les IA)

- réentrainement régulier puisqu'il y a toujours de nouveaux articles etc et mettre à jour les modèles
- traitements: 
  - ajout de concepts par référentiels scientifiques
  - TAL pour texte non structuré
  - classification (corpus de référence, analyse de proximité)
- référenciels: "colle" entre les données/documents

## Discussion

editorial pipeline: 

- upload materials
- assign them to different people (collaborative team with different modes)
- testing transcription tools
- types of documents that people might want to put into xml environment

more aimed at historical documents not contemporary text edition

named entity recognition model

Could LEAF writer kill Oxygen? 

- high costs of Oxygen
- LEAF allows for more people to engage in similar ways as oxygen but it's not as full featured, dont hand write your header
- 80/20 : usually, 80% of people use the mainstream features and only 20% need the highly specialized features

mode de ne pas structurer les nouveaux textes car la doxa branchée car c'est le travail qu'un algorithme fait

AI: sort of a new player, il faut un traducteur-médiateur entre les informaticiens et les informaticiens (AI)

lowtech: on n'a pas besoin de php et mysql pour faire un site web



blog hypothèse, contenu parsé par isidore: éthique du consentement, quel que soit la raison pour laquelle 





## Defamiliarizing Literacy in the First Ten Editions of Bartlett’s Familiar Quotations

Moni Razavi & Constance Crompton (University of Ottawa)

Bartlett's familiar quotations

- snippets of litterature that "one should be familiar with"
- including for for people with limited access to education

Over the timespan of the first ten editions (when bartlett was alive), what kind of material was supposed to be "familiar" to an educated public? 

- extracting the contributor list & reconciliation
- wikidata: a new elephant in the dark → collaborative and shared experience of the reality

data cleaning

- open refine + wiki data
- what to do when the person that is supposed to be quoted isn't the person who wrote it: use their findings since they can be contexualised and seem therefore more reliable
- wiki data place of birth vs citizenship: place of birth was more available
- 5 fields - 300 occupation

data visualisation

creating a sustainable site:

- working with unorthodox of "éditions critiques" and "contexte numérique"
- digital edition is not an edition but a compilation and extension of the original texts

[endings.uvic.ca](https://endings.uvic.ca/principles.html)

- all xml workflow to convert csv to create then xhmtl ...

powerPI microsoft tool for viz



## Fabriquer la littérature: une expérience d’édition numérique en situation critique. Le cas du Novendécaméron

Jean-François Vallée (Collège de Maisonneuve) & Antoine Fauchié (Université de Montréal)

novendécameron : jeu de mot entre "nouveau décameron" et "novendeca" = 19

sorte de performance, littérature-action, en 2021: 

- 22 textes
- 81 jours
- 27 auteur·rice·s/traducteur·rice·s/chercheur·se·s et artistes
- rythme d'une publication bi-hebdomadaire, sur plusieurs plateformes (style feuilleton 19e)

Question: Comment produire des formes littéraires accessibles et lisibles en contexte numérique? comment unifier une série de contenus hétéroclites dans un environnement cohérent? 

des textes, des artefacts, des formats

du dialogue de la Renaissance aux interactions numériques

- modèle des dialogues-cadres du Décaméron et de l'Heptaméron
- ouverture sur des espaces conversationnels en ligne

Technique et technologies de l'édition numériques

- pourquoi le web? briques technologiques existantes adaptées au besoin
- ouverture et Interopérabilité grâce à la base sur des standards, permet réutilisation et généricisation du modèle ici crée
- plus grande facilité d'archivage

Méthodologie expérimentale et des exigences éditoriales

- plusieurs acteurs
- médiums variés: textes, poèmes, images, son....
- cadre temporel serré

- chaîne en développement continu
- low tech - minimal computing
- architecture relativement simple
  - sources versionnées dans un dépôt git
  - CI/CD pipelines
  - artefacts: page web et livres imprimés

Outils: modèle de travail collaboratif, modulaire et décentralisé

- hugo: générateur de site statique
- git
- forestry: interface qui simplifie la collaboration
- infrastructure gitlab (déploiement et hébergement)

Espaces de travail en simultané:

- développements (expérimentations, nouveaux modèles)
- prévisualisations multiples et indépendantes
- production

flux de travail avec Git pour penser les étapes sous forme de branches, les réunir, les arrêter au besoin

transversalité des époques autant que des formats et médiums: web, RS, infolettre, imprimé/imprimable

Conclusions:

- généricisation du modèle? volonté que ce soit réutilisable
- déploiement en continu appliqué à la littérature
- poursuite de la tradition humaniste avec des outils contemporains
- applications possibles dans la sphère de l'édition critique

## Discussion

tension when talking about editions:

- how to make them more accessible, easier...
- we need to learn more, be more specialized...
- [AI]

legal issues and copyright issues have not been discussed today

