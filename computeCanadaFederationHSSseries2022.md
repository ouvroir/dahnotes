# Compute Canada Federation HSS Series 2022

[Programme](https://hss-series-2022.netlify.app/fr/)

## Bienvenue et discours d'ouverture

Mot de bienvenue par : Lydia Vermeyden
Introduction par : Nizar Ladak and Ghilaine Roquet

> L’équipe nationale Sciences humaines et sociales accueille celles et  ceux qui participent à la deuxième édition de la semaine de formation de la fédération Calcul Canada pour les sciences humaines et sociales.  Nous aurons l’occasion d’entendre Nizar Ladak, directeur général de  l’Alliance de recherche numérique du Canada ainsi que Ghilaine Roquet,  vice-présidente Stratégie et planification.

Nizar Ladak, directeur général de l’Alliance de recherche numérique du Canada

Ghilaine Roquet,  vice-présidente Stratégie et planification

### Mot de bienvenue

Calcul Canada va être remplacé par l'alliance à compter du 1er avril 2022

### Ghilaine Roquet: présentation du plan stratégique 2022-2025

Mandat du ministre Champagne

- enjeux écologiques
- déclaration des nations unies sur les droits des peuples autochtones (DNUDPA)
- EDIA (équité, diversité, inclusivité, accessibilité)
- groupe de travail sur les politiques numériques
- plan d'action national en matière de cybersécurité
- financement: nouvelles grappes pour augmenter l'infrastructure. IA + stratégies quantiques
- ajout 1000 chaires de recherche au Canada

Tendance vers l'ouverture

- domaine le moins mature dans les activités de l'IRN
- efforts particuliers vont être faits du côté du logiciel ouvert
- cadres de gestion des données interopérables, travail qui se fait particulièrement dans le domaine de la santé pour mettre en place des standards de définition des données. Améliorer les recherches par la mise en commun
- chaînes de bloc: surtout dans le domaine financier mais aussi aspects pour la pérennisation de l'information 

Libre-service infonuagique

- pas l'intention que tout aille vers des nuages commerciaux, des cas qui ne correspondent pas (confidentialités, besoins spécifiques)
- utilisation de infonuagique commercial comme une extension. beaucoup de chercheur·se·s l'utilisent déjà. Ce n'est pas de le nier mais le faire avec une meilleure sécurité, capacité d'échange d'information et éviter les risques de pertes de données quand les financements de la recherche se terminent

Diversification des modèles de gestion: le nuage

- allocation dynamique et évolutivité du service
- couches d'outils au-delà de l'infrastructure physique (avantage du commercial avec la panoplie d'outils offerts aux utilisateur·rice·s)
- économie de coût potentielle: oui mais pas vraiment démontré. l'avantage serait surtout la rapidité d'accès (~2ans pour une nouvelle grappe. Le commercial est disponible très rapidement)
- expansion de l'infrastructure de recherche numérique, l'étendre vers le nuage pour faire face à des demandes de pointe et faciliter le retrait et l'échange d'information qui sont des risques avérés dans des environnements infonuagiques commerciaux

Innovation axée sur les objects

- besoin de métriques de l'utilisation des ressources pour assurer que l'approche est inclusive, fait la promotion de l'accessibilité, optimisation de l'utilisation par tous les différents groupes
- soutenir le volet collégial 

Intégration omnicanal (hors ligne / en ligne)

- requiert des changements importants au niveau logiciel 
- attente d'accès à l'environnement où qu'ils soient à travers le monde

Increasing integrated research

- users of DRI and joint application for research with newer users

Open-trends

- open science: call to collaborate but want to comply with legislation. There are tools that help for that

Question in slack channel

- [Chris Geroux](https://acenetanyonec-rjy3884.slack.com/archives/C02KCAHQ4NB/p1645553430403599)

  Is the commercial/public cloud a good alternative (or an important augmentation) to operating our own cloud hardware? Is it more cost effective? It seems to be implied from your talk as a possible or at least partial solution to our lack of computing capacity, how will it help us increase our computing capacity more cost effectively and if so can we be reasonably confident it will remain cost effective?

  - envisionned as a complement to the services
  - cloud strategy is evaluating the prices anew
  - researchers are creatures of habits: when they already have commercial cloud service they are used to, they want to stay with it
  - Amazon, Azure, Google....: business opportunity for them. on behalf of the federation, if they garantee an lower-price with added service (strong cybersecurity)
  - advantage because they have not been able to offer quick access (ex: grant time, extend capacity for purposeful opportunities)

Further questions: [ask alliance](**ask-alliance-demandez-à-alliance**)

## Une aventure numérique : Technologie et soutien de la fédération Calcul Canada pour l’avancement de la recherche

Présenté par : Lydia Vermeyden et Megan Meredith-Lobay

> Learn about the national digital infrastructure that is free to access  through the Compute Canada Federation (CCF) for academic researchers in  Canada! This workshop will begin with a short overview of the CCF’s  digital resources and user supports, including the expanding Humanities  and Social Science specific supports. It will continue with a discussion with participants about current applications and use cases for their  research areas and explore potential projects. This part of the session  will include live demos of applicable technologies, and a database  code-along!

### Overview of the CCF’s  digital resources and user supports, including the expanding Humanities  and Social Science specific supports

Compute Canada federation

- not for profit organisation funded by CFI
- privde essential digital infrastructure for industry and researchers in Canda

regional consortia: respond to local needs, target training and support 

#### Supporting research

resources

- high performance, big data and GPU computing
- cloud environment dev space
- terabytes of active data storage with secure backup systems
- large file transfer portals

services

- training
  - discipline specific training, national training
  - high performance computing carpentry
  - summer schools
- centralized software stacks
- nextcloud
- specialized data portals
- FRDR collaboration
- globus file transfer
- database as a service

expertise 

- consultation: helping to determine the resources needed
- designing, optimizing and troubleshooting computer code
- customizing tools
- specialized support is available for a range of disciplines (including HSS)
- visualization specialist
- cybersecurity

#### Getting access

- resource allocations
- services: CCF Wiki, disciplinary suppot
- expertise: consortia website,...

#### HSS Support

- HSS Experts in WestGrid and Aceet
- nation HSS team with domain and technical experts located at sites across the country
- support for Digital humanities Summer Institute

HSS National team

- Félix-Antoine Fortin, U Laval

- Mohammed Jabir, calculQuébec

  

[Software stack](https://docs.computecanada.ca/wiki/Available_software)

- what's not on it, reach out and make a request, will depend on licensing
- users: collaborators must be affiliated to a canadian university

### Database code-along

database as a service via ssh connexion

mySQL hosted on the HSS team virtual machine on the cloud

| IP          | username | password |
| ----------- | -------- | -------- |
| 206.12.93.3 | user18   | HSS2022  |

#### SSH 

```bash
ssh username@ipAddress
mysql -u username
# now shows: `mysql>`
USE movielens;
# Database changed
SELECT * FROM rating WHERE rating=5;
SELECT title, year FROM movie INNER JOIN rating ON movie.id = rating.movie_id WHERE rating.rating = 5 and movie.year=1990;
# remove duplicates
SELECT distinct title, year FROM movie INNER JOIN rating ON movie.id = rating.movie_id WHERE rating.rating = 5 and movie.year = 1990;
```

### Current applications and use cases for their research areas

#### Cloud projects and infrastructure demonstration

In the cloud: website hosted in Arbutus

CCF does not currently offer services for creating virtual machines etc. Requires technical knowledge or funding...

Has been identified as an issue and disproportionately affecting specific disciplines 

for more: session #9 on friday

#### VM

analyse / collecte de données

ex: virtual collaboration space to use

- R 
- jupyter lab
- targuette (contenus qualitatifs)
- postman: GUI interaction with API and URL query test

Utiliser les canaux slack pour discuter de nos projets

## Research Data Management for HSS: From Plan to Preservation, and (Almost) Everything in Between

PDF: 

February 24, 2022, 12:00-2:00pm ET

Presented by: Beth Knazook, Robyn Nicholson, Yvette Rancourt, Victoria Smith, Erin Clay, and Kelly Stathis

> Research data management, or RDM, is  increasingly recognized as an important part of the research enterprise  in all disciplines, including the humanities and social sciences. With  the introduction of the Tri-Agency Research Data Management Policy, and  the broad recognition of principles such as FAIR, CARE, and OCAP, it’s  crucial for researchers to understand and adopt good RDM practices.  You’ll be glad you did! This workshop will give you an overview of the  essentials of RDM, with tips, resources, and tools that you can begin to incorporate into your work right away. Topics will include:
>
> - What counts as research data
> - What a data management plan is, and how it can help you
> - What data curation is, and why it’s important
> - What to consider when sharing your data with other researchers
> - What to consider when preserving your data for the long term
> - What data might be considered sensitive, and how to ensure that these data are properly managed

### Introduction à la gestion des données de recherche

Mireille Léger-Rousseau

Définition des données de recherches

- sources principales à l'appui d'une enquête scientifique
- élément de preuve
- nécessaire pour valider les conclusion

Exemples: données textuelles, fichiers sonores, données tabulaires, questionnaires, entrevues, images, données géospatiales, analyses textuelles

autres typologies: 

- données expérimentales, données d'observation, données opérationnelles
- données du secteur public, données de tierces parties, données de surveillance

Qu'est ce que la GDR? 

Gestion des données de recherche → cycle de vie des données de recherche: 

- guider la collecte
- documentation
- stockage
- partage
- conservation

le projet ne se termine pas avec la publication, devrait se poursuivre en nourrissant de nouvelles questions

Les principes FAIR: 

- Facile à trouver
- Accessible
- Interopérable
- Réutilisable

Pourqoi gérer ses données? 

- commence à devenir obligatoire
- prévenir les risque (désuetude des données)
- éthique, confidentialité et sécurité
- tendre vers la transparence scientifique

Politique en gestion des données de recherche: publiée le 15 mars 2021

- Institutions: devoir de rédiger une stratégie de GRD ([politiques des trois organismes](https://science.gc.ca/eic/site/063.nsf/fra/h_97610.html))
- Chercheur·se·s: doivent soumettre un plan de gestion des donées de recherche

### Plan de gestion des données de recherche

Cynthia Lisée, bibliothécaire, UQAM

#### PDG: Quoi, pourquoi, quand?

- outil de gestion, considère la gestion des données  AVANT de commencer le projet
- expose clairement les stratégies et les outils employés pour gérer efficacement les données
- document vivant qui sera modifié tout au long du projet pour refléter les changements survenus

Un PDG, ça sert à 

- définir des stratégies cohérentes avant le début de la recherche sur la manière dont les données seront gérées tout au long de leur cycle de vie
- identifier les forces et faiblesses des pratiques actuelles et prendre des décisions sur la manière d'ajuster les pratiques
- préparer les données pour la réutilisation future, leur préservation et leur partage
- planifier et réduire le coût global de la recherche par le gain d'efficacité

Quand travailler le PDG? 

- dès qu'on formule une proposition et qu'on planifie le projet
- mettre à jour le document lors de la collecte, l'analyse et le partage des données
- à la fin du projet: préservation ou conservation des données

Pourquoi? va probablement devenir obligatoire

#### Contenu du PDG

- Collecte de données
- Documentation et métadonnées
- Stockage et sauvegarde
- préservation
- partage et réutilisation
- responsabilité et ressource <!-- qui est responsable + coûts potentiels + formations nécessaires pour le personnel-->
- conformité éthique et juridique

Directives générales: 

- commencer par fournir une description du projet de recherche, son but et ses objectifs
- définir tous les acronymes
- éviter le jargon (doit être clair et compris de tou·te·s)
- éviter de laisser des blancs (quitte à noter: compléter à telle étape)
- longueur: dépend de la complexité, généralement 1-5 page
- réutiliesr le contenu pour les demandes éthiques et de financements de projets similaires

#### Ressouces

- documents produits par [portage](https://portagenetwork.ca/fr/outils-et-ressources/ressources-de-formation-de-portage/) (l'alliance)
  - [Créer un plan de données de recherche efficace](https://zenodo.org/record/4012728#.YhfF6lRybVh)
- assisant PDG: contient des [modèles](https://assistant.portagenetwork.ca/public_templates) par discipline
- exemples
  - to introduce Data Management principles to students (and have a bit of fun!), you might consider this Research Data Management Adventure (https://rdm-games.gitlab.io/rdm-adventure/) or this Data Horror Escape Room! (https://sites.google.com/vu.nl/datahorror/home) - These days it's worth having a bit of fun, even with demanding topics like RDM 
- webinaires et vidéos
- personnes ressources par établissement
- [CARE Principles for Indigenous Data Governance](https://www.gida-global.org/care)

### Données sensibles

Jeff Moon

données sensibles

- protégées contret out accès ou toute divulgation injustifiée
- déparsonnalisé: retrait des identifants directs (nom) mais conserve identifiants indirects (âge, sexe)

Lois, règlements et principes

- fédéral et provincial: protection de la vie privée

Devrions-nous partager des données sensibles? Oui! 

- le partage des données sensibles peut rendre la rehcerche plus éthique
- consentement éclairé et autonomie du participant
- les participant·e·s décident du partage des données

Changement de paradigme: 

- avant: 
  - par défaut: détruire
  - consentement = étude originale uniquement
- maintenant
  - par défaut: préserver et partager
  - consentement: utilisation future / générale
  - données peuvent être réutilisées si nécessaire

`Say no to single-use data`

Boîte à outils pour les données sensibles

Boîte à outils pour les données sensibles — destiné aux chercheurs

- [glossaire](https://zenodo.org/record/4088986#.YhfGeHXMLVh)
- [Matrice de risque lié aux données de recherche avec des êtres humains](https://zenodo.org/record/4107119#.YhfGW3XMLVh)
- [Langage en matière de gestion de données de recherche pour le consentement éclairé](https://zenodo.org/record/4107186#.YhfGwHXMLVh)

### Curation de données pour les SHS

Nicole DeMichelis

la curation des données: 

- gestion active des données de recherche de leur cycle de vie complet
- processus itératif qui augmente la valeur de la recherche en optimisant les ensembles de donées pour leur utilisation actuelle et à venir
- FAIR
  - F: identifiant pérenne, métadonnées riches, indexées dans une ressource interrogeable
  - A: format ouverts, fichiers s'ouvrent correctement
  - I: langage formel, accessible et partagé, références à d'autres (méta)-données
  - R: 

Activités de curation de données

- documentation: 

  - informations contextuelles sur les données
  - descripion des conventions de nomenclature des fichiers et de la structure des fichiers (organisation des fichiers: essayer des noms courts mais descriptifs, éviter les hiérarchies complexes ou trop imbriquées: moèle [TIER](https://www.projecttier.org/tier-protocol/protocol-4-0/)) <!-- partie sur la nomenclature, très utile et on devrait la diffuser aux chercheur·se·s-->
  - renregistrement des modifications
  - gestions des droits: informations liées à la confidentiations et utilisations secondaires + modèle de citation des données. 
    - attention: libre accès ne veu pas dire libre reproduction ou libre republication

  

### Le partage des données. Du dépôt à la découverte

Clara Turp

#### Où déposer ses données? 

choix du dépôt: 

- spécifique au domaine ou généraliste?
- dépôt institutionnel, national ou international
- selon la taille des données

Options: 

- canadiennes
  - scholars portal dataverse
  - dépôt fédéré des données de recherche
- spécifique: qualitative data repository ou ICPSR
- autres options
  - institutionnel (qui acceptent les données en plus des publications)
  - site auto-hébergé (attention: maintenance etc.) pensez aussi à déposer les données dans un début (ou s'assurer du moissonnage etc...)

Guides de sélection de dépôts de données

- option de dépôt au Canada: un guide de portage

#### Métadonnées pour les dépôts de données

- métadonnées descriptives permettent la découverte
- éléments communs des métadonnées
- dépôts ont généralement un standard
- important pour 
  - principes FAIR
  - nécessaire pour les systèmes de recherche
  - aide à l'organisation des dépôts

éléments de métadonnées clés

- décrire les données, pas l'article
- penser à la recherche et à la réutilisation (Guide: how to write a (good) data description: developing best practice)
  - quelqu'un pourrait-il trouver les données?
  - y a-t-il assez de contexte pour comprendre? 
- mot-clés: regarder le répertoire de vedette-matière
- licence (choosealicence)
- géospatial: lieu concerné
- identifiants pérennes: 
  - résultats de recherche = DOI
  - chercheur·se·s = ORCID ID


Impact du dépôt via le moissonnage et les outils de découverte



### Préservation des données de recherche

Mireille Nappert, archiviste numérique, HEC Montréal

préservation numérique: tout ce qu'on met en œuvr epou qu'une ressource numérique soit réutilisable aussi longtemps que nécessaire

- validation
- contrôle d'intégrité
- reproduction
- migration
- émulation

Résultats

- authenticité
- accès en continu

méthodes 3-2-1

- au moins 3 copies
- à des endroits différents

outil de renommage: reNamerPro

plan de succession pour les données







## Le pire qui peut arriver...Table ronde sur la gestion des données de recherche

Le 24 février 2022, de 14 h 30 à 16 h HE

Animée par : Nick Rochlin. Membres de la table ronde : Craig Squires (En), Arun Jacob (En), Felicity Taylor (En, Fr) et Maude Bonenfant (Fr)

*Note* : Les discussions se tiendront en français et en anglais. Des services d’interprétation simultanée seront disponibles.

> Pour discuter de comment se passe la  gestion des données de recherche dans la pratique, des membres de notre  équipe technique se joignent à des chercheuses et chercheurs dans une  table ronde où seront présentés des exemples concrets. On y parlera  surtout de situations inattendues qui peuvent se produire et causer des  problèmes de toutes sortes, même des histoires d’horreur! La rencontre  sera dirigée par Nick Rochlin, spécialiste en gestion des données de  recherche au campus Okanagan de l’Université de la Colombie-Britannique. N’hésitez pas à poser des questions sur vos cas particuliers en direct  ou en remplissant [ce formulaire](https://docs.google.com/forms/d/e/1FAIpQLSdanlooKFdnaOsd1TIhLvt7-VXW-jg1IdCquC5inXjO1Pm60A/viewform?usp=sf_link). Bien sûr, vous pouvez vous joindre à nous si vous n’avez pas de questions!
