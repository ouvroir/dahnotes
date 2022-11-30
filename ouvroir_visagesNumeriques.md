---
title: Midi-causerie avec Antoine Courtin
description: midi-causerie du 29 novembre
author: ouvroir
date: 2022-11-29
draft: true
tags:
    - cr

---

# Visages numériques d'un futur centre de recherche
L'exemple de l'EPMO
[Midi-causerie avec Antoine Courtin](https://mobilizon.fr/events/4773dea6-c970-43c4-a722-ca0b83f2e89e)

Participation:
- 13 personnes sur place
- 5 personnes en ligne

Réflexions en construction.
CRR, Centre de ressources et de recherche. Volonté de l’établissement public de disposer d’un centre et d’un lieu physique pour promouvoir la recherche mais aussi la connaissance sur les collections et sur l’art du XIXe siècle.
- Favoriser la diffusion des connaissances sur nos collections et l’art du XIXe s. auprès du public, des spécialistes, et du grand public.
- Accroître et mieux valoriser les ressources physiques et numériques
- Proposer de nouveaux servcices et mieux accueillir les usagers.
- Enrichir les missions et améliorer les conditions de travail de l'équipe / faire connaitre et valoriser les différentes facettes de nos métiers

CRR Centre de Ressources et de Recherches
- lieu physique: l'hôtel de Mailly-Nesle
- ONNI Objets numériques non identifiés

Deux composantes étroitement liées.
Le lieu physique, hôtel particulier dont une aile conservée. Deux verrières qui constitueront les deux salles de lectures du CRR.

Aucun échaffaudage pendant 1 ans (à cause des jeux olympiques).
Salles de lecture : dossier œuvre et fonds patrimoniaux.
Mettre en regard dans un espace physique la documentation et la bibliothèque afin de pouvoir naviguer entre la documentation et les ouvrages.

Un espace pour la programmation scientifique. Des bureaux pour les agents. Un espace de traitement des fonds (archives d’artistes ou de galeries).

Espace d’accueil de jeunes chercheurs. Un  [appel à bourses doctorales](https://www.musee-orsay.fr/fr/articles/bourse-doctorale-de-la-fondation-des-amis-pour-le-rayonnement-des-musees-dorsay-et-de-lorangerie-214914). 

Une phase de préfiguration car l’objectif final, en raison des contraintes architecturales est une ouverture pour les 40 ans de l’EPMO 1986 = 2026-2027.

## Les visages numériques du CRR

En avoir dans la phase de préfiguration et dans la phase d’ouverture.

Plusieurs paramètres à prendre en compte : Le musée est un lieu tourné vers l’exposition qui mobilise toutes les forces vives. Moins d’engagement sur la consolidation des données.

Question de l’externalisation vs internalisation des développements : 100% externalisés.

Question de la conversion des données. Il existe un existant : portail agrégatif du moteur collection. Notices documentaires pour Les Andelys de Signac : Jocond, RMN_Grand Palais, Joconde :
- page musée Orsay
- Joconde agrégateur intermédiaire
- agrégateur RMN-Grand palais

Des enjeux de synchronisation des objets de collections sur ces différents agrégateurs de données : Le musée d’Orsay n’a pas versé depuis 2011. Enjeu de la qualité des données et de la confiance.

Fonction placé au sein du département de la conservation des collections alors qu’il existe une direction du numérique. Positionnement crucial pour le projet.

Évolution des pratiques métiers. 2/3 agents au musée depuis plus de 15 ans. Implique conduite du changement, formation interne. 

Problématique d’ouverture avec la RMN. Convention qui ne permet pas actuellement de diffuser une image de plus de 900px pour les collections en ligne.

Une réalité technique. FileMaker reste l’outil principal du musée pour toutes les bases de données. Gros problème lié aux changements de politique tarifaires = 2024 plus de financement pour les licences.

Approche data, communication, scientifique

### Data : shéma global de données patrimoniales
systématisation la mise en discours et la mise en données

Décoreller la données des Systèmes d’information métier

Trois étapes
- relier, aligner, enrichir les jeux de données produits en interne au sein de la direction de la conservation
- reliler aligner enrichir avec autres acteurs au sein de l’établissement
- alignement avec corpus de référence fournis par les partenaires

État des lieu des progiciels métiers.
- TMS SIGC Système intégré de gestiond de collection, [thèse](https://www.theses.fr/s347635) Carl Pineau (Bruno Bachimont) : données desriptives sur les collections et les entités personnes
- DAM digital assets management, mis en place cette année. Gestion des œuvres mais aussi communication des expositions. 95% images, un peu de vidéo. Une banque d’images à l’échelle de l’établissement
- Catalogue de la bibliothèque, rattaché au CCBMN Catalogue collectif des bibliothèques des musées nationaux
- SIA Système information archivitique en cours de mise en place. ATOM
- Dossier d’œuvres numériques DONUM (outil non id)
- Bdd de recherche FileMaker pro / [Collective Access](https://www.collectiveaccess.org/). 20 bases en fonctionnement. Sculpture polychrone et À nos grands hommes dans Collective Access.
- GED SharePoint

Divers progiciels métiers mis en place au cours de l’histoire du musée et sans lien entre eux.

Deux approches : on rebat toutes les cartes, ou bien on reprend l’existant (ex. TMS 10 ans pour la mise en place au MO).

L’approche retenue a plutôt été celle de penser une maison des données (data warehouse, data lake) qui serait alimenté par le croisement de ces données avec une consolidation des données dans cet environnement = **externalisation de l’intelligence de données en dehors des logiciels métiers.**

Possibilité d’être consommé afin de décoreller l’outil de gestion des applicatifs.

À partir de nos logiciels 
Seconde étape, pouvoir être alimentés par des corpus externes gérés par le MO. Référentiels métiers, bibliographie, etc. 
Corpus externes de références via des partenaires. Exemple réception critique des salons.

Première initiative très modeste : pour les collections en ligne juin 2022.
TMS / Drupal pour le site web.
Pas d’API ou de webservice natif de TMS. Mise en place d’un Backend Symfony qui à partir des Flux XML de TMS permet d’alimenter une API pour Drupal.

Drupal qui actuellement fait le travail d’intelligence et de croisement des données. À terme, pas à Dupal de le faire. 

Exemple notice documentaire en ligne du répetroire des artistes.
Un agrégateur de données. 
- Des informations qui viennent de TMS, (référentiel acteur, etc.)
- Outils de signalement papier
- Lien dynamique vers le catalogue de la bibliothèque (mais version actuelle du CCBM ne permet pas de récupérer nombre d’ouvrage)
- Image provenant du DAM

Autre initiative, articulation dynamique des contenus documentaires avec le site web en s’appuyant sur les identifiants numériques uniques du système TMS.
Dès qu’un communiquant appelle une page web, automatiquement créée un lien vers la notice de l’œuvre.

Un cas d’usage symptomatique : la question des Salons
Permet de multiples approches
- provenance
- réception, etc.

Exemple parfait pour examiner les régimes du discours.
Problématique aussi car la Base Salon, une base entièrement réalisée sur FileMaker (multiple bdd).

Ensemble d’identifiants numériques d’une même œuvre
- id œuvre
- id œuvre dans la transcription du livret du Salon
- id dans Omeka S d’une étudiante sur la production du salon
- id agorah INHA, envois de Rome
- page wikidata sur l’objet
- page Arts & Culture de Google (1000 œuvres versées par MO au Google art Project en 2011)

Chaque identifiant porte des informations singulières sur ces objets.
Base du musée, localisations dans la salle (mise à jour au 24h), texte éditorial.
Salon information du livret. Base doctorante, médaille obtenue au salon.

Mais d’autres informations ailleurs. Documentation papier qui vient des dossiers d’œuvres ainsi que d’autres ressources.

Recherche extraction presse numérisée de Gallica. Twitter et éditorialisation de contenu. Ou encore le Street view de la muséographie de cette œuvre dans la grande nef alors qu’elle a depuis été déplacée.

Conclusion
- cibler les inforamtions pertinentes et éviter l’infobésité
- automatiser les flux d’information mais garder l’éditorialisation par les expetrs
- restitution de ces informations

## Communication des activités

Visage numérique du CRR ne peut pas se réduire à la production de données pour la recherche. Il faut également produire des contenus éditoriaux.

Choix de revendiquer un site indépendant en décorellant le site 
du CRR de celui du musée.

2023 Carnet de recherche sur la plateforme Hypothèses à la fois pour commencer à proposer des contenus éditoriaux mais également assummer cette phase de préfiguration.

Qui dit nouveau bâtiment, dit déménagement, et donc que la documentation ne sera plus accessible en 2026...

Différentiation carnet de recherche du site vitrine.
SIte vitrine, wiki ? club 19, annuaire, programmations scientfiqiue.
explore.musee-orsay.fr, outils de données

Édition scientifique du CRR. Pas possible de décoreller du Musée scientifique. Revue 48-14, 1995-2011. Objectif de réanimer cet outil scientifique. L’idée étant d’avoir un outil print/web avec barrière mobile de 1 an. Numérisation rétrospective sur Persée.

Catalogues, une boîte de pandore. Catalogue Scientifique des collections par techniques ?
- Quire ?
- Articulation avec TMS

Retro-planing
- 2023 AMO datawarehouse, ATOM, Migration Collective access, SIGB, Carnet de recherche
- 2024 dev datawarehouse, plugin ATOM et DAM, migration collective access, marché pour portail 
- 2025
importance (devrait être reflété dans le budget) maintenance en 2027 et enrichissement externes renouvelés en 2028

## Questions - discussion

Comment bénéficier aux SI métier en retour, quels services

L’objectif est d’avoir une étape intermédiaire qui permette un jour de couper la pate aux progiciels. Mais demande qui est que dans trois ans puisse avoir une vision transversale sur ce qui est disponible. In fine, implique de faire des migrations d’outils dans les p

Un outil nuémrique d’alimentation intelligente des dossiers d’œuvre.
Une documentation papier
- dossiers œuvre
- générale
- artistes et perso
- topo

S’est posé la question de l’alimentation des dossiers d’œuvre dans un contexte de plus en plus numérique. En effet, actuellement catalogues de vente en ligne. Screenshot imprime et inscrit n° inv puis verse au dossier d’œuvre.

Comment voir autrement l’enrichissement dans un contexte de plus en plus nativement numérique.

Réflexion en cours.
Utiliser des méthodes issues de la GED avec des méthodes de la LAD Lecture automatique de document, reconnaissance de zones.

Problématiques d’acquisition et de traçabilités pour les données créées. Ensuite quelle interface pour la consultation.

Numérisation des dossiers œuvres seule 800 000 euros... sans interface.
Clairement une automatisation des flux aujourd’hui possible mais éditorialisation qu doit être réalisée par les experts.


Pourquoi ne pas utiliser un id stable entre l’institution et l’œuvre pour croiser la base de données ?

Une excellente question mais aussi très problématique. Ce que veut faire le Getty avec le [CONA](https://www.getty.edu/research/tools/vocabularies/cona/index.html), et en France ce que devrait faire le ministère de la Culture. Avoir des identifiants uniques attribués à l’objet patrimonial.

Il s’agit d’un des objectifs du projet ESPADON notamment avec le laboratoire du Louvre qui produit nombreuses données sur les œuvres.

N° inventaires loins d’être uniques au MO.

Plusieurs bonens nouvelles : Gauthier Poupeau vient d’arriver au MCC en tant que Data Architect.
Pression de la commission européenne pour alimenter Europeana en données de qualité. Oblige à revoir le moteur Collections. En 2025, la Fr doit fournir 300% en Ht qualité. Refonte du moteur Collection car l’opérateur.

Historique des accrochages.
Un de mes objectifs projets sousmarin. Nous avons actuellement plus de 12 000 (18000?) vues d’exposition et d’accrochage des collections permanentes. C’est énorme. Sans compter 10 000 tirages papiers non numérisés des exposition de 1986 à 2000 (devenu nativement numérique entre 2000 et 2002).

Nous sommes plusieurs à militer pour que devienne un programme de recherche. 
MOMA avec Google
98 000 notices documentaires 89% illustrés au moins d’une image.


CIECO: Nouveaux usages? 
le travail du CRR va-t-il transformer l'institution, le travail à l'interne ou sa diffusion? 

Si fait déjà bien modestement une vue d’ensemble des ressources textuelles et corpus de référence dans un moteur de recherche plus articulé. Moins en moins dans la recherche de l’innovation et plus dans la maintenance.

Déjà ouvert beaucoup de portes mais pas forcément bien ouvertes. Pour les collections en ligne, beaucoup de choses qui ne vont pas. Relier les corpus de référence à la presse du 19e. Pépites à trouver.

ML actée dans la phase de maison des données intelligente.
Pour la 3D ne fait pas grand chose. Regarde énormément, mais surveille ESPADON, objet patrimonial augmenté, connecté avec projet Aïoli de Livio Di Luca. 


En train de déelopper le plugin pour que le contenu de la médiathèque soit avec IIIF

Négociation RMN

Question de la patrimonialisation de l’objet numérique. Exemple du musée brésilien dévasté par les flammes. Finalement représentation numérique dernier objet patrimonial avec disparition autres objets. De plus en plus une question qui va se poser avec des fonds nativement numérique.

Quid des versements numériques. Bnf correspondance de Chris Marker.

Plusieurs réseaux
- réseau des bib des musées de France porté par INHA
- et réseau des bib et des centres de documentation (car nous documentation place particulière)
- autre réseau porté par le MO, Club 19 qui regroupe les institutions muséales avec des collections importantes dans les musées en région