---
title: Colloque Humanistica
description: cr de de la conférence Humanistica
author: ouvroir
date: 2023-06-26
draft: true
tags:
    - cr
    
---
# Colloque Humanistica 2023

## 26 juin


### Table ronde: Ouvrir les musées au(x) numérique(s)
- Marie Barras, doctorante FNS dans le projet Visual Contagions à l’Université de Genève, gestionnaire des données et des projets numériques au Musée d'art et d'histoire de Genève
- Nicola Carboni, Université de Genève 
- Gabriella Lini, Musée d'art et d'histoire de Genève

Avec Antoine Courtin, Federico Nurra, Julien A. Raemy, Dominik Remondino, Manuel Sigrist

Ouvrir: ouverture, accès ouvert, interopérabilité et documentation umérique
3 axes: 
- défis et possibilités de l'intégration des dernières technologies numériques au sein des musées, Antoine Courtin (Orsay) et Federico Nurra (chef du service numérique de l'INHA
- échanges, standards et bonnes pratiques, Nicola Carboni (chercheur post-doc au projet VC à l'Unige) et Julien Raemy (doctorant à l’Université de Bâle, membre actif des communauté IIIF)
- réception de l'expérience numérique auprès du grand public, Dominik Remondino (responsable de la gestion des collections MAH), actif au sein de CIDOC, et Manuel Sigrist (diplôme UNIL, projets art numérique, dirige le lab ?? dans le musée de l'Elysée)

#### Antoine Courtin: Les données de collection(s)
- progiciel de gestion de collection (TMS)
- catalogue collectif des bibliothèque des musées nationaux (Aleph)
- documents words

Vadime Eisseff, Musée et ordinateurs, 1971
Jacques Thuilliers, revue H.A.M.I. (histoire de l'art et moyens informatiques) 

postes de consultation des collections du musée d'orsay en 1989 (?)
vs 
application moible 2023

Service de documentation du muése d'orsay
- premier trimestre 2027

Enjeux: 
- founrir de l'information de qualité sur les collections
- 'etre acteur dans l'élaboration d'une collaboration vertueuse dans l'enrichissement des données culturelles sur les collections, avec les chercheur·se·s
- réalités à prendre en compte
    - progiciels métiers utilisés par les acteurs en interne (maintenance, évolutivité, ...)
    - priorisation des activités au sein d'une institution muséale
    - convention avec Agence photographique dela Réunion des Musées nationaux - Grand Palais (limite de publier sur leur propre site web des images de plus de 800 px)
- Décoreller les données de leur utilisation
- mieux structurer / sémantiser les données 
    - répertoire VangGoghWorldWide CIDOC. profil linkedart → use case pour transformer les données du progiciel vers le format de linkedart

#### Federico Nurra: Ouvrir le (potentiel) numérique des musées
[AGORAH](https://agorha.inha.fr/api): plaforme de données de recherche l'INHA
- 54 bd agrégées dans la même métabase
- importance de structurer les données
- interopérabilité via API
- json-ld pour alignement CIDOC-CRM
- interfaces 
    - portail mondial des revues
    - ...

#### Julien Raemi: Les données ouvertes liées et utilisables (LOUD)
Linked Open Usable Data for Cultural Heritage [phd](https://phd.julsraemy.ch/s/loud/page/home)
LOUD
- équiilibre entre les besoins d'exhaustivité et de précision des données et des préoccupations pragmatiquess

IIIF
Linked Art

LUX Yale Collections discovery

#### Nicola Carboni: Analyse des données et musées

tategallery collection → répondre à des questions de recherche
https://github.com/ncarboni?tab=repositories

#### Dominik Remondino: [museums-online.ch](https://museums-online.ch/)
association des musées suisses
protocole synchrone SRW
- recherches sur la plateforme, recherches dans les bases de données des musées 
- rapide à mettre en place et nécessite peu de réponse
- génère du bruit dans les réponses

protocole asynchrone OAI-PMH (europeana)
- avantage
    - consistance des données
    - contextualisation sémantique
    - vocabulaires contrôlés
- inconvénients
    - important besoin en ressources internes
    - mises à jour régulières potentiellement nécessaires

#### Manuel Sigrist: ouvroir les muéses au(x) numérique(s)
Photo elysée
*\_FIELD* / 2019: sélection de photographiques et controlleur qui mesure le balancement pour déterminer la séquence des images
> venez vous balancer dans les collections du Musées de l'Elysée

Amener un autre type de controlleurs dans les espaces
Labeliser: espace et programme dans le musée
*Artificial intersections* 2020
classification des images, rencontre entre données inter-institutionnelles
- outil de classification, mot-clefs par images

envoi d'une photo par les visiteur, et images qui renvoient des images similaires en réponse

*LCD* 
- déménagement à plateforme10
- comment lier avec la collection du MUDAC
- navigation par la couleur
- beaucoup d'images en nb, mais en les classant sur la gamme chromatique, constat d'absences: peu d'images contenant du violet

NFT dans les musées
#Ukraine 2022
- trophées de guerre

*Open Books* 2023: numérisation de la bibliothèque
- collaboration EPFL+ECAL lab
- naviguer dans les livres numérisés
- interface IIIF, mais aller plus loin: utiliser la puissance de calcul pour analyser le contenu d'un livre et pattern pour aller d'un livre à l'autre

#### Discussion
Quels lieux et quels moyens pour la collaboration? 
- N.C.: est-ce que les musées acceptent les données structurées par les chercheur·se·s ou même par le grand public? intégrer ces données dans les collections muséales, est-ce que ça semblefaisable? 
- A.C: numérique est le lieu de la mutliplication des discours sur les objets patrimoniaux. Mille-feuille informationnel, multiplicité de représentations de l'objet. Qui est l'acteur le plus légitime pour porter ce mille-feuille informationnel ?
- F.N.: enjeux de la paternité multiple des données. proposition en France: objet patrimoinial augmenté? cloud européen de données patrimoiniales (FR + IT) identifiants uniques pérennes: clef du millefeuille.

JR: Standard: doit être pouvoir lu gratuitement. Institutions doivent garder leur pouvoir sur leurs données <!--ah, pas de partage d'autorité ici-->. Contre les standards ISO

AC: vœux pieu vs réalité de l'institution. OAI-PMH: on peut y mettre des choses plus riches que du dc. 

> L'innovation passe par la maintenance 
> Antoine Courtin

Clarisse : standard IIF: quel impact dans la pratique des musées, relation au chercheur·se·s et au public? 
- FN: 5-8 juin: IIIF conf à Naples. Retours des personnes présentes, engagement fort dans l'utilisation de IIIF: standard soupe, requiert uniquement developpement web assez simple. Énorme potentiel à le développer, mais il a fallu une embauche spécialisée. Il faut des moyens. Contre le principe que les HN soient un domaine en soi. Il faut un inverstissement lourd de la part des institutions pour que des ingénieurs et développeurs puisse travailler, à parité, avec les conservateurs etc.
- AC: lâcher prise pour le musée → tou le monde peut s'en accaparer. Ils sont en train de l'implémenter, mais avec l'état actuel de la législation française. C'est de l'interne, mais api qui fonctionne avec des images 800px (loi actuel). Choix stratégique était de l'implémenter, puis il ne reste qu'à enlever la restriction de taille d'image au bon moment. Dimension économique: serveurs IIIF seraient surchargés si leurs VanGogh y sont. Implique beaucoup de "sizer" (dimensionner), ce qui a un coût concret. 
- NC: utilisation de IIIF pour étudier la globalisation par l'image. Toutes les sources utilisées sont IIIF. Si elles n'y sont pas, ils les ajoutent. 10millions d'images pour ça (on été bannis par le serveur BNF parce qu'ils ont fait trop de requêtes)

Utilisabilité des données: données qui "dorment" dans des progiciels type Filemaker. Idée d'exposer ces données et les transformer. Facilité du progiciel pour l'utilisation, type RDF: dire aux chercheurs de faire des requêtes sparql c'est plus compliqué. Est-ce que LOUD aide à répondre à ces questions:
- similaire à IIIF: utiliser sans avoir à comprendre des triplets
- on aggrandit le cercle de personnes capables d'interroger les données
- API documentées et standardiées: pas besoin de refaire 

API chicago art institute: ouverture de chrome qui permet de découverir une œuvre de la collection à chaque utilisation du navigateur

Alternatives: research space comme CMS
Whisky (basé sur drupal)

AC: il n'y a pas de filemaker killer, qui respecte les bonnes pratiques mais aussi répond au besoin des institutions. Cheval de bataille: décorreler l'outil de publication de données avec l'outil qui permet de la saisir.

Michael Sinatra: comment avez-vous réglé la question des droits d'auteur? 
Manuel S: elle n'est pas réglée. Ont le droit dans leurs salles d'exposition mais le projet sur les livres numérisés, on ne peut pas s'en servir en ligne ou s'en servir sur les photos. Technique du opt out? N'a encore jamais eu de plaintes.

FN: Hacker le musée: chacun a des pratiques pirates des données de leurs propres institutions


### Données et patrimoines 
Elina Leblanc 	 

#### L'Initiative Virtuelle Illés: cartographie numérique 3D de la vieille ville de Jérusalem en 1873
- Maryvelma O'Neil, ARCH Jérusalem 	 

[archjerusalem.org](https://www.archjerusalem.org/)
maquette d'Illés, modèle compltet 3D de la vielle vielle de Jérusalem et ses environs
Initiative Virtuelle d'Illés: étuder et protéger le patrimoine 

Maquette réalisée par Stefan Illés entre 1864 et 1873
- étude de comment il a réalisé sa maquette, pourquoi, qui l'a commissionnée?
- maquette est accompagnée d'un modèle signé

Circulation: Vienne (expo universelle 1873), Londres, Zurich, Bâcle, Neuchâtel, Genève (1878)

Achetée et exposée à Genève entre 1878 et 1984, puis prêt permanent (renouvelé au 5 ans) au Musée de la Tour de David à Jérusalem

Spécifications tehcniques
- échelle: 1:500, environ 4x4.3m
- fabriquée en milliers de feuilles de zinc couvertes de mastic
- montées sur un cadre construit en 8 unités topographiques

Démonstration de la modernisation de la ville, présence européenne dans la ville et *extra muros*
modple codé par couleur pour distinguer l'ancienne et nouvelle ville
détails notables: drapeaux consulaires, fenêtres en verre, poteaux télégraphiques

Représentation de quelques monuments historiques aujourd'hui intégralement détruits

app 3d pour visiter (apple) le quartier maghébin (détruit 1967) [Mughrabi quarter digital archive](https://www.palestine-studies.org/en/node/1650013)

Prcessus de nmérisation: *Wired* Duke en 2017-2018
avec Dr Andrew Yip

métadonnées en dc sous la forme de points de repères

Virtual Illés Initiative: Steam
- couches historiques de la ville
- superposition avec des cartes historiques 

Appel à paricipation: 2e phase, histoire sociale et culturelle de Jérusalem ottoman finissante
- clustering et SIG pour créer une visualisation basée sur le temps et la géolocalisation
- algorithmes de modélisation

Ajout d'annotation pour matériel histoire sociale, lettres, témoignages et traces 

3e phase: géographie historique
- documenter numériquement la relation écologique, sociale et économique de la ville avec ses environs pour rendre visibile les transformations du paysage historique

Outil de recherche riche et extensible
index spatial comme méthode d'accès aux documents scientifiques et aux archives
partage en ligne et impression 3D
projection dans des contextes muséaux et espaces publics

Questions
- aspect participatif: comment fonctionne-t-il? formulaire, mail




#### Faire parler les claveaux effondrés de la cathédrale Notre-Dame de Paris : un récit fondé sur le web sémantique et les Linked Open Data 
- Anaïs Guillem, MAP-CNRS 
- Antoine Gros, MAP-CNRS 	 

claveaux: pierres qui composent les arcs des voûts
Cas d'étude: arc F28-30. publication en 2024 

méthodologie de mapping: travail de restitution a déjà été effectué

Constat: récits autour de la restauration était faite autour des protagonistes humains (ingénieurs, tailleurs de pierre, ...). Perspective très réduite, ne montre qu'une petite partie du chantier. Claveau en tant qu'objet comme acteur par lequel voir le chantier.

Le conte de Cendrillon et la quête de la provenance
- retracer une histoire à partir de l'itinéraire d'un objet: quel récit peut-on faire des claveaux effondrés de Notre-Dame? 

> Objects too have agency 
> Latour, 2005, 63-86

- réconciliation de la définition du social (acteur) avec les objets et la mtérialité
- continuité théorique d'assemblage social, objet comme acteur de premier ordre dans les relations sociales
- objets: participants dans le cours d'une paction

Le récit biographique d'un claveau
- en élévation
- chuté
- enfoui,
- nettoyé, dépollué
- numérisé
- restitué
- retaill
- carotté
- restauré
- ...

Problèmes d'intégration des données et interopérabilité
récit non-linéaire favrosie l'utilisation de méthodes issues des sciences de l'information, notamment le mapping, la représentation conceptuelle et l'enrichissement de métadonnées
retracer et combiner la provenance des objets-claveaux et la provenance de données de manière sémantique en rétablissant des liens entre les données

CIDOC
naviguer dans un chantier avec CIDOC et l'objet Claveau
description avec schéma de métadonnées, modèle 7w (who, what, ...)
renseigner le contexte de création de quelque chose
questions simples auxquelles tout le monde peut répondre
traduction assez simple vers CIDOC

Le mapping comme explicitation d'une trame narrative
Mapping: alignement des métadonnées sur un schéma choisi
<!--claveau qui rencontre les corps de métier, d'événements, de lieux-->

Pourquoi des identifiants locaux alors qu'il y a des authorité? 
Incendie, desctruction/modification

Analyse d'activité lapidaire: identification et extraction des métadonnées
Les métadonnées et les données sont souvent mélangées
- identifier
- structurer 
- mapper

chargées dans GraphDB
- requêtes SPARQL

Choix d'adopter une perspective narrativée centrée sur le claveau-acteur et les actvités

Questions
- épistémologie: comment concilier CIDOC (ontologie positiviste moderniste) avec la théorie de l'acteur-réseau? 
	- CIDOC part du principe qu'un objet ne peut pas être un acteur
	- argumentaire: on a besoin d'interroger les objets en tant qu'acteurs
	- questions actuelles des object-oriented paradigm
	- utilisation de CIDOC pour pouvoir aller plus loin
- pour les chercheur·se·s, y a-t-il d'autres moyens de faire des requêtes qui soit plus facile d'utilisation que SPARQL? 
	- contexte: chantier avec plus de 170 chercheur·se·s
	- groupe de travail numérique a une vocation plus transversale
	- expliciter les questions de recherche et les aider à transformer le tout sans requêtes SPARQL
	- collecte des questions de recherche pour aller plus loin dans les requêtes

SPARNATURAL


#### Numériser les archives d'histoire de l'art : la collection de photographies d'Heinrich Wölfflin 
Pauline Jacsont, Université de Genève

Bilan du travail réalisé
Objectif: mise en valeur de ces archives par l'aspect textuel qui s'y trouve
Wölflin: prof à l'Université de Zurich

FonDUE: formes numérisées et détection unifiée des écritures (simon Gabay et Jean-Luc Falcone)
- eScriptorium
- kraken 

Collection de photographies d'Heinrich Wölfflin
- historien de l'art
- lègue de l'intégralité de sa collection de photographie d'art à la bib universitaire de Zurich
- contiennent des notes manuscrites qui font des renvois à ses travaux

Fonds
- 60'000 documents
- différents formats de photographies
- plates de verre (diapositives)
2 campagnes de numérisation pour faciliter la recherche et l'inventaire de ces documents

Description des données
3 catégories de facsimilés (typologie des pages)
- portefolio: indications sur le peinture, le lieu, ...
- illustration page recto: contenu visuel, parfois inscription en dessous (manuscrit ou imprimé)
- illustration page verso: notes manuscrites

Écritures hétérogènes
- différentes langues (allemand, français, italien, ..)
- différents caractères
- différentes mains (catalogueurs notamment)

Construction de vérité de terrain
jeux de données préexistants
- CREMMA Early modern books
- CREMMA 20th century manuscripts
- Lectaurep: notaires de paris
Jeux de données pas très probants

Pas de jeu complètement adapté au corpus
résolution à entraîner un modèle
- vocabulaire de segmentation SegmOnto

Entraîner le modèle sur l'intégralité des données ou distinguer entre les lignes imprimées et les lignes manuscrites? 

Transcription graphémique: comme c'est écrit, pas de résolution d'abréviation

Expériences et résultats
- distinction des premières pages des pages avec les illustrations
- 4 modèles de segmentation
- 9 modèles ATR

Résultats
segmentation
- modèle extrêment spécialisé n'améliore pas spécifiquement la qualité des résultats
- YALTAi: plus précis, particulièrement les notes de bas de page

transcription
- modèles entraînés uniquement des textes manuscrits (GT3) a des meilleurs résultats que le général (GT6)
- utilisation de modèles d'HTR n'améliorent pas les résultats
- modèle très spécifique (GT1) créé sur un échantillon ne perfome pas si bien

3 scénarios pour la transcription de l'ensemble du corpus, dont GT6: perfomme en moyenne sur l'ensemble du corpus

Questions non résolues: 
- comment traiter la segmentation et la transcirption des verso 
- comment traiter les zones moins fréquentées

utiliser Transformeur OCR? GottBERT ou RoBERTa 

dernière étape: création d'une base de données avec les transcriptions pour faciliter la recherche dans ces documents, SGBD(avec eXist-db) ou SGBDR (relationnel avec liens vers documents)? 

Questions
Inflation de corpus en créant des données artificielles? pourquoi l'utiliser ou non? 
- pas penser à le faire parce qu'elle ne l'a jamais fait, mais aussi pas mal d'autres tests à faire
- serait une solution possible d'amélioration des données

Base de données pour les résultats:  envisagé TEI publisher? 
- oui, repose sur exist db


### La 2e (r)évolution des métadonnées archivistiques : contexte, enjeux, méthodes et perspectives 
Florence Clavaud, responsable du Lab, AN

#### Les métadonnées archivistiques, retour sur une histoire récente
~30 dernières années

première révolution des métadonnées archivisitque
- fin des années 90: informatisation
- passage des "instruments de recherche" (ensemble organisé de métadonnées. *Finding aid*) papier à des fichiers modifiables à volonté, diffusables en ligne et exploitables par la machine
- normalisation fondée sur ISAD(G) un stadard international (international standard for archive description - general) publié par l'ICA (international councils of archives) en 1993: stockage natif ou export en format XML/EAD

Pourquoi une révolution? 
- pression du public → produire des "descriptions comptabiles, pertinentes et explicites" pour faciliter la recherche et l0échange d'informations sur les archives
avant l'irruption du public dans les salles, on n'avait pas ressenti le besoin d'échanger des métadonnées.
public = principal moteur des services d'archives

→ alimentation des premiers sites web locaux, puis de portails agrégateurs

Actions
- programmes massifs de conversion rétrospectives d'IR (instruments de recherche)
- rédaction de manuels de mise en œuvre EAD
- numréisation de documents originaux
- SI avec interfaces web
- montée en compétences, ressources humaines
- Standards ISAAR CPF: décrire les producteurs
- SI: Intégrés qui accompagnent la totalité des tâches de la chaîne de traitement archivistique, de la gestion des entrées à la communication en passant par la gestion des espaces et la description
- SEDA: archives électroniques

ANF
- travaux d'encodage, formation et rédaction d'un guide d'encodage entre 2000 et 2004
- analyse quantitative et qualitative de l'existant
- première campagne massive de numérisation entre 2007 et 2013
- deuxième campagne en cours

SIA totalement déployé en 2013, accompagne toutes les tâches de l'archiviste

Bilan après 20 ans: des bénéfices majeurs pour l'usager
- changement majeur dans les modaltés d'accès : transformation radicale de méthodes de recherche en archives
- interfaces web assez proches d'un service à un autre: structurées par EAD
- mise ne place de protails agrégateurs à l'échelle locale, nationale et supranationale

#### Contexte et enjeux de la transition
Bilan après 20 ans: des tendances lourdes
- baisse de fréquentation drastique dans les salles de lecture
des millions d'images, mais seul 5 à 6% numérisé... 

conséquence
- moins de médiation humaine: effacement des méthodes classiques de recherche en archives au profit de la recherche dite "plein texte", des formulaires de recherche avancées et des moteurs généralistes
- réduction du discours écrit dans les instruments de recherche: IR du XIX avaient d'extrêmement longues introductions qui présentent le fonds, explicitent leur travail et présentent ainsi de grands discours historiques


- hausse du niveau d'exigence 
- diversification des usages et usagers

- production paricipative des métadonnées: indexation collaborative

Limites des modèles, règles et pratiques de descrptions
- on a converti la traduction de l'instrument de recherche papier, devenus des documents XML structurés
- deux éléments de contexte seulement sont systématiquement et rigourusement pris en compte: la provenance organique, et le contexte documentaire (*archival bond*)
- avec ISAD(G) et EAD, relations de provenance et d'agrégation prédominent, car prises en compte dans dès les opérations de collecte et de classement

car structure hiérarchique XML et des dossiers

Les interfaces de consultation des métadonnées archivistiques restituent tant bien que mal cette perspective métier, essentiellement bidimensionnelle, qui est difficile à comprendre pour l'utilisateur

Lorsque les institutions produisent et publient des notices d'autorité, c'est le plus souvent uniquement pour les producteurs et même si ces notices forment avec les instruments de recherche un réseau complexe

*caricaturise volontairement*

Solutions pour lier les descriptions de documents entre elles: simplistes, pas très bien utilisées 
- Cela fait des IR des micr-silos, des univers clos
- cela ne facilite pas l'interrogation transverse, l'exploration par rebonds

On les transcrit, on les encode, mais on n'établit pas de rapports entre ce qu'ils décrivent et ce qu'ils disent

Des trois standards, ISAAR reste marginalement employé

Sous-indexation des métadonnées, doublées de l'absence (sauf une exception) de référenctiels de description d'agents ou de lieux, ou de vocabulaires d'indexiation partagés
silence ou bruit à la recherche, pas de porte d'entrée facile

Standards aujourd'hui trop simples, ou simplistes? 
- même traitement pour un agrégat documentaire, des items spécifiques ou des données
Les pratiques et la théorie ont évolué, dont irruption des archives nativement numériques. Provenance fonctionnelle: fonctions, plus stables que les agents. 

Inadéquation entre les standards et les besoins aujourd'hui

IR ont eux-même une histoire
- gestion de mdescriptions multiples pour le même thème: redondances
- des documents ou dossiers ont pu être décrits plusieurs fois au sein du plsuieurs IR, mais même quatifier ce problème est difficile en ce moment
- les métadonnées finissent par masquer la réalité documentaire

Beaucoup de silos, et des conséquences pour l'utilisateur
- première révoltion est toujours en cours: sans passerelles entre les dispositifs & métadonnées de gestion ne sont pas toujours liées aux métadonnées de description
- redondance, dispersion des métadonnées

Exemple sur Henri Labrouste (cf carnet de recherche)

Contexte compliqué
- nécessité de collecter, traiter et communiquer des masses toujurs plus importantes d'archives contemporaines: notion d'archives exssentielles et de macro-évaluation fonctionnelle, elle-même difficile à mettre en œuvre
- urgence stratégique et poids de l'archivage des documents et données nativement numériques
- recherches administratives en hausse
- complexité des questions juridique
- ressources financières et humaines limitées (fin d'une abondance relative des années 90)


Besoins
- réduire la redonance
- améliorer la cohérence
- ouvrir les silos
- faciliter l'interrogation des métadonnées

Leviers à actionner
- prise de conscience des professionnels
- tendance forte au travail collectif
- approche de co-construction
- partenariats avec des équipes de recherche en SHS
- entrée des métadonnées archivistes sur les plateformes d'open data
- stratégies FAIR
- technologies du web sémantique
- IA

#### Méthodes (et exemples) de FAIRisation
modèle RiC-CM: métadonnées comme graph de données liées 

Cadre de référence unifié, utilisation flexible et transition par étapes, extensible
Production de données fAIR
- syntaxe normalisée
- ontologie voulue pour être immédiatement avec les métadonnées existantes

version 0.2 en ce moment
préparation de la version 1.0 pour cet été 

En quoi RiC est-il différent des précédents standards? 
- modélise les objets d'intérêt du domaine et du métier des archives plutôt que le produit de l'organisation des métadonnées de description
- 4 entités: recourd resource (record set, record, record part)
- RiC distingue le contenu intellectuel d'une resource archivistique (record resource) de ses matérialisations physiques (instantiation)
Doit avoir une instantiation, mais le record peut ensuite exister sans son instantiation, ex: document numérisé dont la source a disparu


RiC permet de représenter les métadonnées de description des archives come des graphes orientés d'entités liées comme CIDOC

Ce que RiC permet de faire
- se concentrer sur les objets à décrire
- rendre explicites les relations qui sont déjà présentes dans les IR
- révéler le graphe sous-jacent
- considérer les inventaires comme des documents
- ...

représentation multidimensionnelle, multicontextuelle, ouverte (non finie) qui rend beaucoup mieux compte de la complexité et de l'histoire du monde des archives
- événements
- activité: événement déclenché par un agent
- relations génétiques (originale, copie)
- entités lieux, règles
- multiplication des points d'entrées et liens avec d'autres données

Conversion ANF entier au format RDF/RiC.O et importées dans un triplestore

changement de nature de l'information en question! 
Nœuds: entités, qui sont liées. Chaque nœud devient une porte d'entrée.

Ric est 
- générique et flexible: selon les moyens, on peut choisir le niveau de description
- extensible: permet de concevoir, au besoin, un modèle adapté à des cas particuliers

exemple du projet de recherche ALGORIA (2018-2021)
- projet ANR IGN; réunir virtuellement des photographies aérienne et créer un moteur mutlimodal pour ces images, avec géoréférencement semi-automaatique et plateforme de visualisation immersive 3D

Données sont sur le github de ANF et dotées d'un SPARQL endpoint

Projet ORESM: portail sémantique de la vie université au Moyen Âge à Paris
- référentiel de personnes et collectivités
- ontologie ORESM, extension de RiC-O

Démonstrateur à grande échelle
- sémantiser les mtaédonnées, puis évaluer et améliorer leur qualité
- interface de recherche → sparnatural
	End-user interface for your SPARQL endpoint
- un jeu de données de 58 millions de triplets RDF librement réutilisable sur Github
- premier décompte que les IR n'étaient pas capable de faire mais qu'une requête SPARQL fait très facilement (mais chiffres parfois erronés, car doublons et redondance dans les descriptions)

mise en ligne de deux interfaces de recherche
- utiliser les recherche sauvegardées
- exporter les données

Bénéfice réel, questions qu'on ne pouvait pas poser avant

Travail sur les référentiels, avec les technologies sémantiques
- chantier sur les référentiels de lieux, probable collaboration avec IGN
- interface de consultation et API une fois qu'ils seront sémantisés
- premiers résultats dans un dépôt public sur gihtub

Autres projets avec RiC
- franceArchives
- Pays-Bas dont services d'archives
- ...

#### Conclusion: défis et perspectives
écosystème qui peut aider en retour à enrichir ses propres données
collaboration
articulation RiC avec CIDOC-CRM

ce qu'on peut imaginer
- mettre en relation des items dispersés entre institutions et ou leur manifestations
- fin du cloisonnement entre archives numériques et analogiques
- référeniels alignés
- nouvelles infrastructures, workflows
- interfaces de visualisation
- aliance des méthodes avec l'IA si elle peut être industrialisées et intégrées au SI, via l'HTR, à partir des métadonnées existantes, ...

AI4LAM: chapitre francophone (google groups)

#### Questions
Qu'est-ce qui a inspiré le changement des arborescences hiérarchisées au graphe? 
- permettre à l'utilisateur de s'engager:faire du rdf, mais 2 verrous 
	- les utilisateurs ne connaissent pas SPQARL
	- ne connaissent pas non plus l'ontologie
- plus d'engagement
- chercheur·se·s ne savent pas toujours au début ce qu'ils cherchent: aussi une interface d'exploration
- comblet le gap: permettre de poser de nouvelles questions

Qu'est-ce qui peut permettre une acculturation à ces outils? Presque mouvement inverse: entrainement social à faire accepter/comprendre le fomulaire de recherche
- important: introduire de nouvelles possibilités
- datavisualisation: utiliser les graphiques
- augmenter avec un graphe de connaissance

moteur de recherche du Rijks couplé à un graphe de connaissance

export non pas des uri mais aussi des valeurs textuelles

## 27 juin
### Théâtre et Arts performatifs
Miguel Betti 	 
#### Rendre intelligibles les effets de sources dans une base de données. Circulation, mobilité des spectacles ambulants au XIXe siècle. 
- Johanna Daniel, LAboratoire de Recherche Historique Rhône-Alpes - UMR5190, Institut National d'Histoire de l'Art
- Aurelia Vasile, Maison des Sciences de l'Homme de Clermont-Ferrand 	 

Registre sur les individus et leurs déplacement
[Base *Spectacle de curiosités*](https://spectacle-de-curiosites.msh.uca.fr/), 1800-1880
- 12'000 individus
- 20'000 enregistrements
- 49 services d'archives
- 100'000 événements
Effet de source: inégale conservation des archives de police au travers de la France
Mise en base de données tend à invisibiliser les absences, les creux

##### Comment restituer les "effets de source"?
Comment donner à voir l'inégale granularité des données? 
Comment accompagner l'usager dans la critique de données mises à disposition? 

Visualisation comme moyen de communiquer l'ampleur de la collecte tout donner à voir la non-représentativité des données prises dans leur globalité

Cartographie des points enrengistrés dans la source
Comparaison avec la cartographie des services d'archives dépouillés

Cartographie des villes d'enrigstrement, avec une frise chronologiquement

##### Faire prendre conscience des données manquantes
datascape: Breve, par standford

Visualisation la densité d'événements par personne dans la durée

Naviguer dans le corpus et définir des sous-échantillons pour répondre à des questions

##### Accompagner dans le sous-découpage de corpus pour des questions de recherche
Localisation des lieux de naissance des montreurs de spectacles passés par Agen
- 3200 enregistrements, donc 50% pour la décennie de 1820
- cartogrpahie des lieux de naissance
- visa obtenu avant l'arrivée à Agen, destination déclarée au départ d'Agen

Concentration des naissances dans les pyrénées
Origines des montreurs d'animaux (328)
- liens entre leurs lieux de naissance et le lieu d'enregistrement? 
- point d'arrive est un effet de source
- les lieux de naissances sont constants

##### Conclusion

Pourquoi faire ces visualisations et quels sont leurs statuts? 
Un peu entre les deux:
- explorer le corpus
- produire des visualisation pour transmettre des résutats de recherche
Outils de médiation, interfaces de collaborations
Sans visualisation, ces données sont très abstraites
Elles facilitent la médaition et le dialogue interdisciplinaire entre les acteurs de la bd.

Comment les intégrer dans l'interface de la base de données pour faciliter l'appropriation individuelle de la base? 
existant actuel: recherche mot-clef ou facettes, mais résultat sous forme de tableur
Volonté d'offrir des résultats visuels

##### Questions
faire apparaître les trajectoires; routes, distances

Identification des personnes
- tailles aident à dire que deux entrées sont les mêmes
- policiers recopient les traces qui permettent d'identifier les personnes
Réconciliation vs précision/remonter à la source
Convention d'équivalence entre personnes malgré des graphies différentes
- Première partie de la fiche est réconciliée et déduites
- chaque enregistrement permet de voir ce qui est présent dans la source

Données sur wikidata?
Aimeraient déposer le dépôt de données sur un dépôt pérenne mais doivent convaincre les porteurs de projet
Alignement des archives et des lieux avec geonames

`!--Quel outil pour la publication de la base` -->


#### Décrire et cartographier les théâtres de société (1700-1871) : résultats et perspectives 
- Valentina Ponzetto, Université de Lausanne FNS
dates: lumières et XIXe jusqu'à la fin du Second empire (période faste pour les arts du spectacle)

[portail de données du FNS](https://data.snf.ch/grants)
[portail de données du FNS](https://data.snf.ch/grants)
[DaSCH](https://www.dasch.swiss/): Swiss national data and service center for the humanities (Bâle) → [projet](https://admin.ls-prod-server.dasch.swiss/project/0103)

[site de consutlation](theatresdesociete.unil.ch/projet)
4 points d'entrées:
- carte
- calendrier
- auteurs
- pièces

Créer des archives du théâtre de société, qui jusqu'à présent était considéré comme une curiosité
Envie de créer une bd complexe qui serait accesible de multiples façons
Base non relationelle
- bibliographies
	- correspondances, journaux intimes, pièces
- représentations
	- unité (relie les personnes, les pièces, ...)
- personnes
	- individus
	- collectifs
	- personnes connues dans l'audience

Carte avec lieux (attention aux effets de source), sélecteur temporel, possibilité de rechercher les lieux dans une barre de recherche

Résultats obtenus
- confirmer ou informer les idées reçues à la lumière des données
	- quantifiables
	- comparables
- faire émerger de nouvelles observations

##### Questions
A.V.: Choix de faire une base qui n'est pas relationnelle? 
- Modèle créé de toute pièces, aidée par un collaborateur DH
- disait ce qu'elle souhaitait obtenir et lui trouvait les solutions, en collaboration avec une informaticienne de l'Unil
- non relationnel: recommandé pour pouvoir combiner des données différentes
- n'avait pas réalisé les problèmes techniques représentés
- a beaucoup retardé et compliqué la mise en fonction de la bd
- espoir de la pérenniser: à long terme elle pense que c'était le bon choix

C.B.: Est-ce que c'est basé sur une ontologie type FRBROO? Question de l'interopérabilité? 
- Souhait de mettre en place une intéropérabilité mais pense que c'est impossible vu la construction de la base de données
- ontologie a été modifiée il y a moins d'une année: on peut renvoyer vers des entrées sur d'autres bd, mais c'est un renvoi, pas une vraie interopérabilité
- toutes les données sont ouvertes, en ligne et le modèle aussi

A.V.: vocabulaire contrôlé pour les représentations? Alignement avec wikidata? 
- jamais pensé à aligner avec wikidata
- lieux décrits: ex, "ville, chez M. xxx"


### Modélisation de données
- Julien Raemy 	 

#### Linked Open Data pour l'intégration horizontale des informations des expositions 
- Nicola Carboni, Université de Genève,  University of Geneva 	 
avec Béatrice Joyeux-Prunel et un stagiaire, Thibaut...?

données d'expositions, absence de conceptualisation partagée
utilisation de CIDOC et triplets RDF

CIDOC CRM SIG

Artlas: bd collaborative de catalogues d'exposition du XIXe

réflexion sur les fuzzy temporalities: quadruples
T = < TfuzzyFrom, Tbeg, Tend, TfuzzyUntil>

Pas rpévu de faire une interface
analyses avec jupyter notebooks


#### Modèles et outils pour la publication de métadonnées d'archives géographiques et de leurs données dérivées 
- Melvin Hersent, IGN
IGN, EHESS, IPITA, AN

référentiel d'adresses à Paris au XIXe
Sources
- répertoire du commerce
- cartes et plans

Notion d'Item (contenu intellectuel d'une œuvre) et d'Instance (expression physique d'une œuvre)

4 étapes dans la chaîne de traitement
- reconnaissance
- classification
- géoréférencement: plan scanné → points de contrôles→ plan géoférencé → vectorisation (automatique: îôts et bâtiments, manuelle: rues et adresses): donnée géographique structurée
- structuration

Catalogue de documentation du projet
- sources utilisées
- données dérivées des sources
- plateforme entre les chercheur·se·s

Modélisation FAIR dans données sIG = ISO 19115
- DS_Aggregate: dossier
- DS_Dataset: atlas
- DS_ressource: planches
manque les liens entre items et instances
avantageS: adapté pour décrire des données institutionnelles
documentation est payante! :o 

utilisation de Records in Context Contextual Model RiC-CM
- Record
- instantiations
- instantiations dérivées (numérisation, version géoréférencées)

PROV Data Model: décrire les activités, activités et personnes participant à la production de quelque chose

Le catalogue
- geonetwork: catalogue de ressources géographiques
- utilise nativement ISO 19115
- propose des identifiants unique pour chaque ressource (F)

Ontop:
- pour se conformer aux principes FAIR 
- porteurs de mappings pour l'alignement


architecture en microservices
- docker pour le déploiement
- hébergement d'images IIf
- outils de visualisations

Conclusion
- proposition entre norme ISO et RiC-CM

Questions
IIIF et AllMaps


### Visualisation de données

#### Propositions cartographiques pour l'étude des traductions: le cas de Jane Eyre de Charlotte Brontë 
- Giovanni VITALI, Dynamiques patrimoniales et culturelles


[Jane Eyre Mapping](https://modernlanguagesopen.org/articles/10.3828/mlo.v0i0.375)

[Arabic covers map](https://digitalkoine.github.io/arabic_storymap/)

Primsatic Jane Eyre: Close-reading a world novel across languages

Nouvelles perspectives: questions de la langue
- TTR Type/Token Ration
- lexical richness

pondérer les éditions, selon les maisons d'éditions et les distributions?

### Épistémologie

#### Un monde façonné pa les services Web. Lescture théorique du REST
Giulia Ferretti, UdeM

style architectural REST
maniablité des technologies numériques

Texte de son projet de thèse en API pour structurer son projet de thèse
- écriture de l'API
- structuration de l'information traîtée par l'API

REST est une forme d'écriture textuelle et matérielle
- matière et sens (théorie et technique) sont ontologiquement inséparables
- herméneutique de la matière

Démonstration théorique
- si le champ d'application du dispositif était une pure représentation de la pensée humaine, l'objet informatique n'aurait pas de champ d'aplication spécifique
- si la portée de l'appareil sur note monde était dérivée d'une exécution purement mécanique, cete portée serait radicalement différente de notre compréhension du monde

Comprendre l'impact du numérique sur notre monde? 

Nouveau matérialisme
> penser une relation mutuelle et nécessaire entre la pensée humaine, la culture, le code et l'exécution matérielle
> (Barad, 2007)

culture et matérialité se déterminent mutuellement

technologies évoluent en fonction de nos cultures et besoins
nos cultures évolent en fonction des technologies informatiques

Démonstration pratique
Analyse du style architectural REST
protocole qui structure la majorité des contenus sur le web

Distinguer le code source et la construction architecturale d'un service

Principes REST
- séparation des responsabilités entre client et serveur
- statelessness
- uniformité de l'interface

Endpoint = représentation des resources

Protocoles de fait: choix dictés par des conventions culturelles

REST - JSON 

Interface
- montrer une partie de l'appareil technique et sémantique 
- connexion à l'edpoint: fetch()
- structurer la requête côté client

Travailler avec des représentations d'une ressource

Routes
- chapitres
- extraire les titres

mongoose Scema pour valider les informations entrantes dans la base de données

MongoDB 
représentation des ressources correspond à la structuration de la bd

Matière
- champ de possibilités
- résistance


Architecture de backend: schéma d'accès à l'information
endpoint stocké dans des fichiers


Technosémiotique, Samuel Goyet = API comme architexte


### Images
- Paul Kervegan (https://quartier-richelieu.inha.fr/)

#### Pister des circulations visuelles à l'échelle mondiale. Méthode et premiers résultats du projet Visual Contagions 
- Béatrice Joyeux-Prunel, Université de Genève 
- Nicola Carboni, Université de Genève 
- **Marie Barras**, Université

Circulations visuelles à grande échelle
Mondialisation par l'image

I. Un corpus numérique
- 4500 périodique (1890-1990)
- 1200 villes
- entièrement IIIF

Détecter, extraire et classer les images
- 1787 périodiques
- 278 villes
- 6.8 M illustrations

Juin 2023:
- 4409 périodiques
- 1181 villes
- 10.8 M images

Vectorisation et classification par similarité

Cluster-Surf: carto-chronologie des images

Circuits de diffusion selon le type d'images considéré
- actualité circule dans les pays / ère linquistique

[Exposition au jeu de paume](https://jeudepaume.org/en/evenement/visual-contagions/) 2022

Images artistiques
- circulation des images d'art, particulièrement celles considérées comme innovantes
- tester la pertinence de la méthode computationnelle
- mécanismes de circulation

II. Opérationnaliser les images
90 revues illustrées catégorisées comme "d'avant garde"

plateforme explore 
- visualiser des images
- effectuer des recherches d'images
- sélectionner, nommer, compléter des clusters

Visualiser, récupérer les métadonnées (export csv)

2 types de Cluster: 
- images exactements similaires
- groupes d'images associées à un même style artistique

Etudier des chaînes de circulation visuelle
- clusters d'images similaires produites à des lieux différents, ...

image primitive: située en amont de la châine de circulation

cluster dans une bd orientée graph (RDF CIDOC CRM)
noteboks 

4 indices
- centralité
- interconnectivité
- internationalité
- hybridité: images partagées

Résultats 1910-1945
11000 images, 98 revues
- évolutions chronologiques inhabituelles
1910: république tchèque, france, allemagne
1915 (guerre): france absente
1920: r'ole inédit d'europe centrale
1927: crise et régimes non démoncratiques: france et allemagne

Quelles sont le simages qui ont le plus circulé
1694 ayant un flux visuel "identique" dites "primitives"

Pas d'entraînement 

métadonnées vs similarité vectorielle
Image vs fragment
recomplète les cluster par single search, pistes de recherches qui sont ensuite affinées par l'œil humain

pas uniquement des revues d'art
compliqué pour le figuratif car similarité de forme et non de contenu

#### Memorekall-IIIF : De l'annotation vidéo à la création d'un réseau documentaire 
- Jacob Hart, Université de Rennes 2 
- Clarisse Bardiot, Université de Rennes 2
- David Rouquet

[Memorekall](memorekall.com)

##### Introduction

Projet dont les premières maquettes datent de 2007
Trace de la captation vidéo des arts de la scène
Art de la scène: œuvres disparaissent, donc captation sont des documents essentiels

##### MemoRekall Legacy
- free and open source app
- annotation de vidéos textuelle, graphique, lien  (agnostique au type de documents reliés)
- capsules: code embed pour le partage et l'intégration
- mutlti-utilisateur
- usages pas réservés aux arts de la scène (plusieurs usagers variés)

Captation vidéo
- annotations liés à la temporalité dans la vidéo
- représentation spatiale du corpus sans passer par les corpus

COESO: science citoyenne
documentation de la collaboration entre une chorégraphe et une philosophe
- memorekall
- laban

Comment étendre la capacité de MemoRekall à relier des documents? 
- lien vers des db comme europeana

Comment faciliter la collaboration et créer des capsules FAIR? 

Réimplémentation de MemoRekall basée sur IIIF

La captation est-elle le document principal? 
- la partition devrait être au centre, à laquelle on peut greffer des captations vidéo
- mise en réseau : graph de documents et pour "dé-centrer" la captation

##### MemoRekall-IIIF
- fork du lecteur Mirador pour ajouter un système d'annotation et supporte les vidéos (tokyo: mirador vidéo)
- annotation nestées dans le manifeste: manifestes qui annotent des manifestes
- plugin pour annoter des vidéo
- support multi-utilisateur

Présenté à la conférence à Naples
- va être intégré à Mirador

Dimension en réseau: de l'outil d'annotation vidéo vers un réseau de document
- chaque document peut être annoté
- connexion des documents car l'un annote l'autre

Interfaces data-driven

Réseau des manifestes: visualiser le réseau documentaire

pas d'ontologie dans IIF donc prendre en fonction des métiers
- fait partie de son travail pour penser à l'ontologie dans le cadre de son ERC
- permettre le choix de l'ontologie, de vocabulaires
- travail avec des plugin

1 interface naïve: on ne voit pas IIIF
ensuite, fonctionnalités avancées


### Le jeu vidéo comme objet d'étude : perspectives croisées entre humanités numériques et sciences du jeu
- Yannick Rochat (Université de Lausanne, GameLab UNIL-EPFL)
- prof assistant en jeu vidéo
CH Ludens
yro.ch

Donner un aperçu du champ des game studies
Présenter le jeu vidéo comme domaine de recherche

Paul gooding, *Grand theft archive*
Geoffrey Rockwell, Replaying Japan conf

*Homo ludens* Essai sur la fonction sociale du Jeu, J Huizinga
*Les jeux et les hommes*, Reoger Caillois
*Cybertext*, Espen Aarseth

Jagoda, *Digital Humanities, New Media and Practice-based Research* 2014

Comment les humanités numériques s'intéressent-elles au jeu? 
Pourquoi les games studies devraient intégrer des méthodes des humanités numériques? 

#### A. Méthodes computationnelles et visualisation de données

Peut-on savoir à quelle époque un terme émerge, se cristallise, et peut-être disparaît dans les discours liés au jeu vidéo? 

Abandonware magasine: magasines 
extraction avec google vision (quelques francs pour des milires de pages)

étude des occurrences de termes, ex "cinématique"
Lecture distante d'un corpus de "jeux vidéo historiques"

Étudier les fictions interactives: isaacpante.net/if

#### B. Close reading et analyse "informatique"
Est-ce que le code source des jeux vidéo, ce support invisible dans la création vidéoludique, a quelque chose à nous raconter? 

Montfort et Bogost : du code source vers les logiques économiques, développement hardware. Comment dépasser les limites de la console? 


Nathan Altice 2015 *I am error*
- comment tirer parti ou contourner les contraintes d'une console

*Retrogame Archeology. Exploring Old computer games*, John Aycock

Distant reading with source code: heat map showing code re-use

Etudes des plateformes 

*Homebrew gaming and the begginings for the vernacular digitality*, Melanie Swalwell

Esthétique du nombre dans les jeux vidéo

#### Histoire et préservation du jeu vidéo
Peut-on répertorier tous les jeux vidéo créés en Suisse? 
Comment les inventorier? 

Pixelvetica
- dépôt légal

[Swiss Games Garden](https://swissgames.garden/)


#### Médiation

jeu vidéo pour élèves sans fair eun jeu sérieux
- chaque aspet du jeu devient une fiche pédagogique, un prétexte à l'enseignement

[Lausanne1830](https://lausanne1830.ch/)
- archives de la ville
- gratuit, directement dans le navigateur

#### Modélisation

Premier lien entre sciences du jeu et HN

technologie du jeu vidéo (game engines) pour la modélisation / reconstruction architecturale
représentation de l'histoire dans les œuvres interactives



#### Questions
dimension très sociale du jeu vidéo 
- soirées LAN
- étudier les interactions sociales, la sociologie du jeu vidéo? 

beaucoup de méthodes d'histoire orale




### Assemblée générale de l'Association Humanistica



## 28 juin
###  Circulations

##### Circulation du discours médical de Jean-Martin Charcot : premières observations  
- Ljudmila Petkovic, Sorbonne Université

Jean-Martin Charcot (1825-1893)
- Napoléon des névroses
- Paganini de l'hystérie
- père de la neurologie moderne

##### Circulation des savoirs: cas de Charcot 

leçon cliniques publiques à l'hôpital de la Salpêtrière à Paris

Impact sur le réseau scientifique et artistique

Elèves
- Sigmund Freud
- Gilles de la Tourette
- Joseph Babisky

Littéraires
- Émile Zola → *Lourdes*
- Léon Tolstoï → *La Sonate à Kreutzer*
- Luigi Capuana → *La Torture*


À la jonction des humanités numériques et de l'histoire des sciences
- pister la circulation de la pensée, du discours
- circulation des textes et des allusions

**Question de recherche**
Comment mesurer le degré d'intertextualité entre Charcot et son réseau scientifique et/ou artistique au prisme du numérique?

##### Premières expérimentations

**Corpus**
Fonds Charcot: 201 documents XML OCRisés
- 698 textes rédigés par Charcot
- 133 textes rédigés par son réseau scientifique

Mesurer informatiquement l'impact de Charcot sur son réseau: intertextualité unidirectionnelle (de Charcot → sur son réseau)
Opérationnalisation de l'impact de Charcot sur ses élèves

[OBVIE](https://obtic.huma-num.fr/obvie/charcot/?view=corpus)
- moteur de recherche permettant une fouille avancée des corpus en XML TEI
- repérages de textes similaires par ordre de pertinence à partir des termes en commun

TextPair
- alignement de séquences similaires dans les deux corpus
- génère une liste de passages similaires
- séquences de mots qui se chevauchent

##### Calcul de pertinence des concepts
Repérage de concepts dans les deux corpus en se basant sur le poids de leur apparition

RF-IDF: évaluer l'importance d'un terme dans un document relativement à un corpus plus large

Extraction des termes et expressions popularisés par Charcot
- index d'une déition des œuvres complets de Charcot (1982)
- sans les termes génériques
- prise en compte des formes singulier/pluriel

Expérimentations avec BERT
- prolongements lexicaux et mécanismes d'attention

##### Conclusion
Vers une lecture plus distnace du corpus Charcot

Recherches futures: 
- Charcot vs les autres: initiateur ou transmetteur de certains termes


Questions
- entités nommées? mention directe des personnes?
- 

#### Visual Contagions: extraire et tracer la circulation d'images dans des imprimés illustrés  
- Robin Champenois, École normale supérieure de Paris 
- Béatrice Joyeux-Prunel, Université de Genève

comment ils ont constitué leurs corpus d'images

##### La circulation des images
*Bilder Fahrzeuge*, Warburg
- le plus souvent abordés par l'étude de cas

étude facilitée par la numérisation des périodiques illustrés du monde entier, sources plus variées et encore jamais étudiées à grande échell

Comment tirer partir de cette disponibilité numérique? 

##### Le projet Visual Contagions
utilise de la disponibilité numérique en open access de revues illustrées entre 1890 à 1990 dans plus de 120 pays

Étapes: 
1. détecter des images similaires
2. La plateforme explore

2 critères: robustesse et fiabilité

##### Détecter des images similaires

ambition initiale: similarité fine
ArtMuner, 2019: Shen et al. 
- fonctionne par comparaison de 2 images
- aurait pris des dizaines d'années en temps de calcul

similarité distante
- extraction d'un vecteur descripteur pour chaque image
- comparaison des vecteurs par similarité cosinus

Entrainement avec un réseau de neurones
ResNet18, préentrâiné sur ImageNet

Amélioration
DINO: méthode d'entrâinement non supervisée, meilleure pour la détection de similarités
- ViT vision transformer (image en petits jetons / tokens)
- descripteur puis PCA avec blanchiment = descripteur final

Regroupement en clusters

##### La plateforme Explore

IIIF
tri de clusters depuis 1 an

recherches sur les culsters pour visualiser la circulation (dans le temps et l'espace)


### Posters

#### Des littéraires sur le web : pratiques de recherche autour de la littérature numérique  
- Fanny Mézard, Université Jean Moulin Lyon 3


#### Élaboration d'un processus pour les images 3D reposant sur IIIF  - Julien Antoine Raemy, Université de Bâle/DasCH 
- Rita Gautschy, Université de Bâle/DasCH

#### Étudier le « groupe de Neuchâtel » : de l'édition des Faits à un corpus numérique de la première Réforme romande  
- Sonia Solfrini, Université de Genève

#### Stylo en 2023 : de nouvelles fonctionnalités pour l'écriture et l'édition scientifique  
- Roch Delannay, Université de Montréal 
- Antoine Fauchié, Université de Montréal
- Marcello Vitali-Rosati, Université de Montréal 


#### Projet Fabliaux : de la reconnaissance d'écriture à la textométrie et à la (re-)définition du genre  
- Jules Nuguet, CNRS 
- Ariane Pinche, CNRS

#### Comparaison entre le théâtre en alsacien (1800-1929) et ses traditions dramatiques sources  
- Pablo Ruiz Fabo, Université de Strasbourg 


#### « Typologie textuelle» : un vocabulaire contrôlé pour le signalement et la description des éditions numériques  
- Ioana Galleron, LATTICE 
- Fatiha Idmhand, Institut des textes et manuscrits modernes 
- Alexey Lavrentev, Institut d'Histoire des Représentations et des Idées dans les Modernités


#### MONA: des données ouvertes à la chasse au trésor culturelle  
- Lena Krause, L'Ouvroir d'histoire de l'art et de muséologie numérique, Maison MONA 

#### La modélisation causale du récit historique de Thomas Piketty sur la réduction des inégalités durant la première moitié du XXe siècle  
- Axel Matthey, Université de Lausanne 


#### Intégrer la provenance dans les bases de données de manuscrits médiévaux  
- Alix Buisseret, Université de Genève


#### Les itinéraires des moines voyageurs dans les rouleaux des morts
- Margaux Nguyen Ngoc Minh, Université de Versailles Saint-Quentin-en-Yvelines


#### hedera, la solution de l'Université de Genève pour les humanités numériques  
- Cédric Viaccoz, Université de Genève 
- Hugues CAZEAUX, Université de Genève 
- Mathieu Vonlanthen, Université de Genève 



### Epistémologie

Béatrice Joyeux-Prunel
#### Comment documenter le “moment” des humanités numériques francophones ?  
- Martin Grandjean, Université de Lausanne 
- Aurélien Berra, Université Paris Nanterre 


Humanities computing, Willard McCarthy

SPECLAB Johanna Drucker
Amongst Digital Humanists, Smijana Antonjevic


#### Fabrique de la fabrique : Réflexion sur les pratiques et praticien.ne.s d'écriture dans les Humanités numériques  
- Margot Mellet, Université de Montréal 

[présentation](https://blank.blue/conf/fabrique/)

fabrique:
- remettre en prespective un objet par rapport à des biais de pensée
- inscrire l'objet dans une pratique, rappeler qu'il est une matière qui a vécu par un travail, un labeur

Comment est fabriquée la fabrique? 

*Homo faber*

Flusser: fabrique *Vom Stand der Dinge* 
> caractéristique humaine commune
> fabriquer signifier détourner quelque chose du donné, le transformer en quelque chose de fait/artefact
> les fabriques sont les lieux où l'on transforme le donné en artefact.


Faroki (1988)

*Hidden and Devalued Feminized Labour in the Digital Humanities: On the Index Thomiticus Project 1954-67* Nyhan 100

La réminiscence du politique

No source find, Gerald Raunig
> la connaissance devient une marchandise, qui est fabriquée, manufacturée et échangée comme les marchandises matérielle
> ambivalence de la fabrique du savoir: lieu de nouvelles formes de conflits


Introspections du Undercommons (vs Understanding): se qui se tient en dessous de nos communs
*Thinking through making* Tim Ingold 2012
- faire: rapport qui évolue au gré des pratiques

Exorcisme des sciences humaines
Friedlich Kittler , «Le logiciel n'existe pas» 1993


#### Intelligence Artificielle Littéraire : dialogues entre philologues et algorithmes  
- Mathilde Verstraete, Université de Montréal 
- Yann Audin, Université de Montréal 

Peut-on définir de manière formelle -, ou, plus précisémment de manière computationnelle et algorithmique - un concept littéraire? 

IAL : intelligence Artificelle Littéraire

L'anthologie: Anthologie palatine + Appendix Planudea
- 4000 épigrammes
- 325 autoeurs
- XVI siècles de littérature

[anthologiagraeca](anthologiagraeca.org)


### Conclusion
Humanistica 2024 au Maroc ~7 mai 2024
- recherche idées/volontaires pour gérer le distanciel

faire des pôles: ex une salle à UdeM? 