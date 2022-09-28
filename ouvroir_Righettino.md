---
title: Midi-causerie Righettino
description: cr de la causerie
author: ouvroir
date: 2022-09-27
draft: true
tags:
    - cr


---
# Righettino. Faire parler une image de la Renaissance, un prototype d’exposition numérique
William Diakité, Chaitanya Tekane et Kenan Oudin
Emmanuel Château-Dutier et Denis Ribouillault

<!--12 personnes dans la salle, 11 personnes en ligne-->

Girolamo Righettino vénicien. Théologien, il est un chanoine du Latran, devient évêque, travaille à la défense de la chrétienté
proche des cercles politiques vétiniens de son époque 
- vue de Rome (description textuelle)//1585
- vue de Turin (image) 1mx1m

Vue de Turin:
- publiée en micro-vignettes dans des catalogues d'exposition
- déplacement aux archives de Turin pour découvrir le détail du dessin sur parchemin
- peu étudiée car sa qualité, sa matérialité et son format la rend complexe: idée d'employer des technologies numériques pour mieux la faire voir
- rapport texte-image 

L'objectif est de découvrir ce personnage original, qui se démarque de la figure de l'artiste. Importance de la dimension de l'exégèse dans son oeuvre.
Histoire de l'art en 2022: autres manières de publier, limites du format livresque

Complexité de faire financer ce type d'initiatives <!-- subvention connexion-->

Encodage du manuscrit en XML-TEI avec Johanna Casenave
Solutions techniques pour visualiser le rapport entre le texte et l'image, la disposition topographique dans l'image
Protocole de partage d'images IIIF, permet de diffuser des images en très haute résolution, avec des interactions possibles sur ces images (redimensionnement, traitement, etc.), présente beaucoup de potentiel pour les institutions et les historiens de l'art 

objectifs et public cible:
- double navigation entre la notice et l'oeuvre
- facilité pour la première utilisation
- simplicité de la navigation pour les publics récurrents
- moins de clics possible, accès rapide

wireframe produit avec un outil de prototypage Figma
- exposition virtuelle divisée entre la visite guidée et la visite libre 
- tutoriel
- chapitres 
- surbrillance autour des items concernés par chapitre
- visite guidée: approche linéaire
- visite libre: interactions avec la souris de l'utilisateur (surbrillance pour passer par dessus un item, clic pour afficher dans le texte, sélection depuis le texte pour voir l'item dans l'image)

conception et implémetation du [prototype numérique](https://ouvroir.umontreal.ca/righettino/)
possibilité de circuler librement dans l'image comme dans le texte, rapport bidirectionnel
démonstration de principe pour IIIF

Protocole IIIF
- standardiser la description des images et leur diffusion sur le web
- apparaît en 2011 dans un collaboration entre la British Library, Standford, BNF, ...
- API (interfaces web) image (2012) et API de présentation
- écosystème assez vaste avec des outils développés depuis plus de 10 ans

essai avec des outils existants pour les expositions numériques mais ne correspondent pas vraiment aux besoins pour le projet Righettino (documentation de chaque outil disponible: Exhibit, Storiiies)
- pas possible d'importer plusieurs images
- qualité réduite
- la qualité des interactions n'était pas satisfaisante

Étapes
- recherche et rédaction 
- encodage du texte
- détourage des items
- [analyse des outils existants](https://github.com/ouvroir/IIIF/tree/main/documentation/exhibition_guided_tour) avec une grille de lecture
- librairies de développement javascript pour programmatiquement créer les fonctionnalités désirées

Deux librairies en vue:
- OpenSeaDragon: très utilisée, plus ancienne (prédate IIIF car fait de l'hyperzoom)
- CanvasPanel (Digirati): plus récent, développeurs principaux contribuent énormément au développement actuel de IIIF
Vonlonté de travailler avec des frameworks javascripts moderne (svelte) pour gérer les interactions, les variables et les états. Complexité dans l'utilisation avec OpenSeaDragon. CanvasPanel fonctionnait très bien mais le développement est en cours, premiers tests très faciles et rapides, mais soudain lorsqu'il s'est agit d'insérer les items en svg dans les images, CanvasPanel n'avait pas encore implémenté cette fonctionnalité.
Se sont rabattus sur OpenSeaDragon et les plugins, manque de documentation.

Format des données: travailler avec du XML dans l'environnement web est toujours un petit peu pénible. L'application est basée sur le texte.

API de présentation IIIF:
- manière de définir une exposition virtuelle
- décrite par un manifeste

Pas utilisé de manifeste parce qu'au début on pouvait faire sans (choix de commencer simple pour initier le prototypage)
Utilisation d'un manifeste est possible, permettrait de mettre toute l'information liée aux annotations directement dans l'image. Par contre, on a aussi développé nos propres manières de présenter les annotations, la description peut difficilement être utilisée dans tous les cadres (sémantique limitée)

Résultats de l'expérimentation
- design assez fonctionnel et précis: désir d'affiner, permettre la comparaison (deux images et deux notices), envisager un format tablette (et réalité augmentée) pour la consutation devant l'oeuvre
- concentration des interactions entre l'image et le texte
- état de l'écosystème IIIF: est-ce que le laboratoire pourrait y contribuer puisque nous allons continuer à nous en servir
- quelle est la possibilité de rendre cet outil générique (pour quoi, pour qui)? quelles seraient d'autres types d'opérations qu'on pourrait faire? Comment décrit-on les textes et les images pour généraliser
- technologies à employer: développer des librairies ou des componsants
- chaînes plutôt simples pour mettre en place une telle exposition (pour l'ensemble des étapes)


Autres contenus:
- sources
- bibliographies
- images en rapport: iconographie qui a été rassemblée dans la recherche et dans les analyses (comparatives), inventivité dans l'iconographie de Righettino. Construire un référentiel pour les stocker

## Questions
Kristine
- le potentiel du projet est énorme
- prérequis nécessitent une collaboration: encodage du texte, création de storyboard, découpage des images, implémentation des interactions et publication web
- intégration des textes, images, bibliographie, annotations: prochaine étape dans ce type de recherche
- difficultés dans la diffusion de ce type de projet
- comment intégrer les compétences techniques et de design avec les besoins des chercheurs? 
    - collaboration n'est pas juste une répartition des rôle
    - terrain commun de traduction, dialogue
- vulgarisation de la recherche

Denis
- comment publier ce type de recherche? on développe une relation particulière avec l'image, plus authentique qu'une médiation linéaire
- besoin pour ces objets qui ont une complexité qui perdent en attractivité dans les formats traditionnels
- format catalogue demeure le format le plus utile, le plus maléable mais il reste encore une étape à faire: les besoins du développement relancent un processus d'écriture final pour aligner avec le prototype
- désir de rendre l'outil accessible à un public niché: ex le public italien
- ouverture du projet pour permettre à d'autres personnes d'y contribuer


Quelle est la taille de l'image? 
- Environ 1m par 1m
- il faudra qu'on rajoute l'échelle (faisable avec IIIF)
Matérialité: image fragile qui ne peut pas être exposée, elle ne peut même pas être déplacée dans leur laboratoire de photographie numérique, aide des outils numériques pour répondre aux enjeux de conservation, diffusion et valorisation

Dispositif de visites guidées
- envisager la création de visites guidées thématiques
- ce serait possible avec un balisage supplémentaire 

Notices: 
- fonctionnement par cataloguage, lecture de l'image
- travail basé sur le texte écrit par l'artiste sur sa vue de Rome
- renvoi vers des portions de l'image ou des corpus spéfifiques, vers des sources et des ressources
- utilisateur Lambda qui puisse se cultiver, se questionner


L'histoire de l'art numérique change notre facon de voir les images, conception de la vision. C'est le cas pour la reconstitution de l'architecture en 3D (voir l'intérieur et l'extérieur en même temps). De même pour les images, y inclure toute une bibliothèque (intégrer des liens, des ressources, entités qui sont documentées)
écrire à l'heure de l'hypertextualité

Outils spécifiques pour l'écriture de l'histoire de l'art
Comment rendre la matérialité de l'image

équipe qu'il faudrait si on était un grand centre
- designer d'interface
- développement d'outils pour réduire les difficultés techniques

Ce projet est une discussion de longue date entre Emmanuel et Denis: 
- intérêt d'un carnet de bord
- vision d'une facilité et d'une simplicité d'utilisation d'un outil qui existerait, mais en fait ils n'existent pas (encore). Il faut les développer et il faut des moyens pour les mettre en place.

Comment rendre la recherche plus inclusive? ne pas renforcer les carcans en matière de catégories et de formats, particulièrement pour l'éditorialisation de recherche historiques par exemple