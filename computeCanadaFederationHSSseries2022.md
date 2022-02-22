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

### Current applications and use cases for their research areas

### Live demos of applicable technologies

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

```



