---
title: Atelier de photogrammétrie
description: notes et suivi de l'atelier de photogrammétrie
author: ouvroir
date: 2023-03-08
draft: true
tags:
    - cr


---

# La photogrammétrie sur le terrain

Kristine Tanton


Photogrammétrie, balayage laser, total station: différences et moyens différents de capter des sites, l'architecture, les lieux

Outils disponibles et utilisation pour la recherche
Disciplines: archéologue s'en sont beaucoup plus servi que les historien·ne·s de l'art

Kinect azur: transformation de la kinect Xbox mais pour le PC, utilisé pour la RA

## Définitions

> SfM: structure from Motion
> technique permettant de construire des modèles tridimensionnels à partir d'une série de photographies

La structure à partir du mouvement est le processus d'estimation de la structure 3D à partir d'images 2D

Distinctions entre la numérisation laser et la photogrammétrie

- balayage laser: haut niveau de précision sur un grand espace
- photogrammétrie: documentation d'espaces plus petits, moins de rpécision mais plus de photoréalisme visuel

Total stations

- utilisé par les arpenteurs, géomètres etc. 
- mesures et entrée de coordonnées précises de certains points
- enregistrer des distances pour des points de référence
- mesurer les angles

3D scanners


## Logiciels

- [Agisoft Metashape](https://www.agisoft.com/)
- [Polycam](https://poly.cam/)
- [Reality Capture](https://www.capturingreality.com/) (seulement PC)
- [sketchfab](https://sketchfab.com/): plateforme sur le web, facile à utiliser et très utilisé

## Projets

### Utilisation par Kristine

reconstitution de monuments perdus ou qui ont subit des modifications majeures

- chapelle détruite mais il reste des fragments
- intégration des fragments dans la reconstitution
- bien distinguer visuellement les "preuves physiques" de la reconstitution

Est-ce qu'il y a des corespondances etre les formes utilisées entre deux chapelles?

[Paris past and present](http://paris.cdh.ucla.edu/)

- lady chapel of Saint-Germain des Prés, embedded dans le site

### ARC/K

OSBL [Arc/k Project](https://arck-project.org)
photogrammetry 101 → cheat sheat (envoyé par courriel)

projet de lancement: palmyre

- reconstitution de la partie détruite par crowdsourcing des photos de touristes
  <!-- intéressant pour les zones de conflit mais aussi pour les zones impactées changements climatiques-->

- impliquer le public dans la conservation du patrimoine

zones floues: manque d'information → clarifie le fait qu'il manquait de l'information, éthique/transparence du travail

sketchfab: annotations pour guider la visite

### Netsuke  Hands-on

[Netsuke, Hands-on](https://echo.mbam.qc.ca/en/history-landing/7cf1e0ca-de77-46bb-8876-e9bca6ab6559), Musée des beaux-arts de Montréal, Laura Vigo 

### Digital Pilgrim 

[Digital Pilgrim](https://sketchfab.com/britishmuseum/collections/digital-pilgrim-a75f0aba434244b5b8de74970561cab4),  The British Museum



### Mesopotamia

[expositions en ligne](https://mesopotamia.getty.edu), Getty

- autre vue sur l'objet (qu'en musée)
- visite de la galerie du musée (documentation des expositions), puis reality capture des objets
  webGL → fait appel à la carte graphique


### Getty Assyrian tablets photogrammetry scans

[Jordan Halsey](https://jordanhalsey.com/the-getty-assyrian-tablets-photogrammetry-scans/) → photographe préféré du Getty

[“A New Way to Experience Art Online”](https://www.getty.edu/news/get-closer-to-ancient-mesopotamia-than-ever-before/) Getty



### National park service (US)

[US National Park Service: Photogrammetry Applications and Examples](https://www.nps.gov/articles/series.htm?id=4B2E480A-1DD8-B71B-0B41FD201137856F)

capturer les parcs avce drones pour documenter les sites

- Hickman Bridge Trail-Head Rockfall Area


utilisation de la photogrammétrie

- documentation d'un site
- capture non destructive
- exposition
- pas le même usage que les images gigapixel ou panorama

ex cathédrale à Chartres, des modifications physiques ont été faites pour garder uniquement ce qui date du 13e et la polychromie de l'époque. Le faire en ligne sous forme de couches aurait évité la destruction de ce qui n'était pas considéré important (dont la valeur change avec le temps)

### Maison MONA 

œuvre d'art *Dé[faroucher]  - un détour dans Villeray* de VahMiré (Ludmila Steckelberg), créée lors d'une résidence d'artiste à l'automne 2022. Informations disponible sur demande (info@monamontreal.org)



## Démo

### Polycam

- iPad et iPhone Pro car équipés avec LIDAR
- payer pour exporter dans plusieurs formats
  - obj pour lgiciel CAO comme Vectorworks (conception 2D et 3D)
    - obj → mesh (n'est pas "solide")
    - jpg → images (vêtement / peau)
    - mtl
    - si on disperse les fichiers, l'objet sera "cassé"
  - stl pour impression 3D (remplit l'image pour pouvoir l'imprimer)
  - point cloud: points capturés
  - other
- version gratuite: permet de sauvegarder mais pas exporter
- outils similaire: scannerverse


appliquer une texture pour donner une impression naturelle
LIDARD: Capture les mesures (pulse de lumière) distances avec l'appareil

importation dans vectorworks

- l'objet n'est pas placé dans la bonne orientation
- avec LIDAR pas besoin de scale quand on importe l'objet (sans, il peut être beaucoup plus petit...)


### Agisoft metashape

new photoscan

- stitches photos together (align them) and builds a mesh
  résultat
- pas à l'échelle
- prend du temps pour l'orienter

### Artstep

[Artstep](https://www.artsteps.com/): construit des espaces d'exposition, espace limité, permet de programmer un parcours et diffuser en ligne (ordinateur et téléphone)

### ARCscene

ArcGIS → accès au département de géographie
[ARCscene](https://desktop.arcgis.com/fr/arcmap/latest/extensions/3d-analyst/3d-analyst-and-arcscene.htm): application de visualisation 3D qui vous permet de consulter vos données SIG en trois dimensions.


