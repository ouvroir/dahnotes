# Redonner vie aux données vectorielles sur la ville de Montréal au 17e et 18e siècles



Léon Robichaud

Laboratoire d'histoire et de patrimoine de Montréal 

Midis du Labo, 28 octobre 2021

___

## Conférence

*Legacy data*: données patrimoniales au formats désuets/sous-utilisées

- refaire une collecte? 
- convertir, nouvelle infrastructure



### Projet initial

CCA + exposition *Montréal, ville fortifée au XVIIIe siècle*. projet mutlimédia

nouvelles technologies du début des années 1990

borne interactive (Alan M. Stewart, groupe inspiré par Louise Deschenes): 

- évolution du parcellaire
- évolution du bâti 
- évolution de la population

Solution 3D: Centre for Landscape Research Toronto

- Recréer les chaînes de titres 1705-1805
- recréer environnement bâti
- identifier les propriétaires

Sources: archives, plans, etc..

- pas d'infrastructure centralisée pour la collecte de données
- cartographie sur ArcGIS (1720, 1765, 1805)
- fusion des fichiers d'attributs avec la cartographie
- logiciel PolyTRIM, conçu pur visualiser les paysages

--> permis la compréhension la transition d'un bâti en bois vers un bâti en pierre, changements dans les origines ethniques des propriétaires, pôles de spécialisation par métier ou fonction commerciale

Redéfinition du projet de 1992-1995

base de données relationnelle (Oracle)

gréer l'incertitude et l'imprécision

Données textuelles publiées en ligne en 1996 (Archives nationales du Québec): remparts.info/adhemar_php

Données 2D et 3D : cartes et données exportées selon les demande



### Défis de la récupération (SIG, 3D)

Transposer les données pour qu'elles soient plus accessibles aujourd'hui

Fichier de données géomatiques sans SCR (référence perdue). Export sans les données de projection

Fichiers 3D en formats désuets: possibilités de les importer dans Autodesk, mais ne peuvent pas être générés de manière procédurale et environnement ne correspondait pas aux environnements actuels

PolyTrim n'était pas un SIG: 

- replacer les plans sur une couche actuelle
- validation de mesures en pieds français
- identifiants n'ont pas suivi, ont été ré-attribués manuellement

### Ajout de nouvelles données

Corrections / finalisation des données pour les besoins d'analyse: 

- clôtures--> couches à associer (plan de fortification + cartographie des lots et des bâtiments de 1725)
  - représentation avec une ligne (polyligne rend l'attribution des propriétaires mitoyens compliquée)
  - indices de confiance
  - matériau probable
- jardins: espaces vert (cultivés = potagers, plantes médicinales, vergers, jardins d'agrément)

Modélisation 3D

- rassembler tous les modèles sur une même plateforme
- création procédurale d'éléments en format OBJ (pour relier avec la base de données)

Interface simplifée pour la visualisation des artefacts du site du marché 

Défis

- 3D en logiciel libre (sans ESRI ou Autodesk)
- Respecter la topographie (pentes et rues en angle, bâtiments en pente...)
- générer éléments du modèle selon leur position cartographique
- chaque bâtiment doit être sélectionnable (id pour associer à la bd) puis recréer une interface semblable à celle d'il y a 25 ans

Projet d'expansion: 

- sortir des fortifications
- ajouter cours d'eau et routes (de l'époque, cartographiés par Valérie Mahaut)
- côte Saint-Joseph
- localiser les lieux importants (ressources naturelles, lieux symboliques, lieux de défense)
- sites occupés par les Français et les peuples autochtones
- cartographier les résidence (propriétaires vs habitants)

Collaborations en cours et à venir: 

- publication sur la plateforme DH UdeS
- [Lab histoire et patrimoine de Montréal](https://lhpm.uqam.ca/)
- Nouvelle-France numérique
- ...

Gros défi de la pérennisation des interfaces

## Période de questions

- pensez vous que vous insèrerez éventuellement des plans, images, photos, etc. avec les bâtiments, rues ou secteurs représentés ? Enjeux des droits de reproduction 
  - *mettre les liens? *

- interface OBJ (format standard pour diffusion et échange objet 3D)  + WebGL comme librairie pour gérer l'interaction (cedi gml pour représentation environnement 3D urbains mais autres défis): vraie interface de consultation (Requêtes, interactivité) 
- python post-grest pour gestion BD (vues) mais option de télécharger les shp
- Comment publie-t-on une carte GIS (de QGIS) sur le Web ? extraire un PDF ou un PNG pour une image statique. Si on veut la relation avec les données: plateforme comme schéma (contient base géo + fichiers associés) cartoDB: possibilité de déposer quelques couches avec BD gratuitement

