---

title: Le protocole d’interopérabilité des images IIIF pour la valorisation des collections patrimoniales
description: cr du midi-causerie
author: ouvroir
date: 2022-05-31
draft: true
tags:
    - cr

---

# Le protocole d’interopérabilité des images IIIF pour la valorisation des collections patrimoniales

Midi-causerie du 31 mai 2022

15 personnes sur place, 57 personnes sur zoom 

## Présentations

### Introduction et présentation de IIIF 
Emmanuel Château-Dutier

Construire des narrations visuelles et expositions en ligne

Interfaces programmables API IIIF
- Image API avec paramètres 
- Presentation API
- Authentification API

Pas besoin de tout faire, utiliser des briques disponibles pour faire chaque étape (serveurs d'images, manipuler un manifeste, utiliser une visionneuse)

IIIF v1 en 2012

### Bibliothèque des sciences
Emir Chouchane
Conseiller en médiation technologique - Bibliothèque des sciences du Campus MIL

Mur de visualisation

Collections de cartes, 3D 

<!-- antropolab photogrammétrie-->


### Bibliothèques de l'UdeM

Martin Sévigny, directeur des technologies bibliothèques UdeM, en collaboration avec Christian Belanger et Rémillard

[carré de sable](https://oncs.bib.umontreal.ca/), service encore en développement qui peut avoir des problèmes éventuels (ne rien mettre de "précieux")

Serveur d'images + outils liés
- afficher le info.json
- afficher avec le serveur d'image IIIF (rotation, redimensionnement, ...)
- afficher le manifeste
- ouvrir dans Mirador
- ouvrir dans Universal Viewer
- ouvrir dans OpenSeaDragon

Possibilité de se fabriquer un manifeste, manifest editor à venir (1-2 semaines). Disponible en ligne, mais il sera lié au carré de sable 

## Questions

Découvrabilité des contenus
- protocoles basés sur le LOD


Pourrait-on penser à une manière d'utiliser IIIF dans des contextes de réalité augmentée ou en mixed realities en général? 
- bonne question
- 3JS, environnement virtuel comme interface de visionneuse IIIF

Potentiel pour la distribution des objets 3D plus aux standards aadémiques

Utilisation d'images par d'autres: risque de liens brisés? 
- les URI ne devraient pas changer
- contreexemple: c'est arrivé avec l'ensemble de la collection du British Museum
- Gallica par exemple est relativement stable depuis le début des années 2000 avec le système ark

Rôles des bibliothèques: exposer les collections, fournir les briques de bases
Individus / chercheurs: utiliser les outils disponibles pour comparer, exposer...

## Discussion suivi

Calypso: 
- images ne sont pas en hd actuellement (images de présentation)
- métadonnées absentes (contentDM logiciel en arrière de calypso)
- ne répond pas à l'ensemble des besoins, seulement à certains

Couche métadonnées: en train d'étudier des systèmes pour voir ce qu'ils font, comment le compléter ou changer 
Question de l'intégration du stockage n'est pas comprise, ce qui ajoute beaucoup de travail