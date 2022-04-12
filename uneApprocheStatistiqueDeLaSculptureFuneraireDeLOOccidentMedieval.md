---

title: « Une approche statistique de la sculpture funéraire de l’Occident médiéval : le cas des tombeaux de prélats français (XIIIe-XIVe siècle) »
date: 2022-03-15
description: Compte rendu du midi-causerie avec Robert Marcoux
author: ouvroir
tags:
    - cr
    - midi-causerie
    
---

15 personnes
Serge Lisgnan, Alix, Ersy, Roch, Carole Schinck, Denise Angers, Fadila Mahdi, Josianne T, Crhistine Baczyk
Robert Marcoux, Lena, Suzanne, Kristine, ? en salle

# « Une approche statistique de la sculpture funéraire de l’Occident médiéval : le cas des tombeaux de prélats français (XIIIe-XIVe siècle) »

Robert Marcoux, professeur agrégé à l’Université de Laval Il a publié plusieurs articles sur l’art des tombeaux médiévaux. Plusieurs projets de recherche financés. 

Recherche statistique effectuée sur des tombeaux de prélats français du 15e siècle. retour aux sources méthodologique car thèse sur l’ensemble des tombeaux dessinés du 17e sièlce par Gagnières.

*L'espace, le monument et l'image du mort au Moyen Âge. Une enquête anthropologique sur les tombeaux médiévaux de la Collection Gaignières*. Thèse, ULaval, 2013

Reprise de la même méthodologie et du même corpus en ciblant des tombreaux d’abbés et d’évêque et de prélats dans le but de dégager des tendances selon le statut.

## Corpus

Approche biographique a ses limites, généraliser à partir de cas individuels hasardeux. Avoir recours à des dessins conséquents.

Collection Gagnières répond parfaitement (en ligne sur [Collecta](https://www.collecta.fr))
1 500 tombeaux, conservés ou détruits. Usage des dessins problématique car en l’absence du modèle difficile de juger de leur qualité. La question de la rigueur des dessins revient régulièrement.

Consensus selon lequel dans l’ensemble, les dessisns seraient suffisants pour servir à la recherche. Exemple Dalle encastrée à Saint-Ouen de Rouen.
Mais la prudence reste néanmoins de mise car des écarts sont parfois constatés. Surtout s’il s’agit d’étude qualitative qui porte sur un nombre limité de dessins.

Réduire les probabilités d’erreur et éviter la corription de l’analyse.
Pour mon étude 225 dessins utilisés. Pour assurer la cohérence du corpus, a limité le cadre géographique de son étude et chronologique (stabilisation art funéraire). Tombeaux qui offrent un panorama stable de la typologique. Division égale entre les clergés séculier et régulier.

124 prélats vs 104 évêques. 

## Méthodologie

Même si pense pouvoir faire 


84 tombeaux sur un total de 225, dont 104 abbés et 121 évêques

Convertir les données en données numériques = formalisation du corpus.
Étape décisive mais aussi très exigeante. 

Ni arbitraire. Formalisation qui passe donc par la production d’une grille de codage précise dont la production s’obtient après plusieurs itérations.

Grille composée de caractères qui réunissent différentes modalités. Réunir ensemble du corpus. Différents caractères. Date, statut clérical du défunt, localisation. Rapports internes, matériaux, typologie.

Dans l’idéal, doit cible modalités cohérentes. Risque de bloquer l’analyse en suscitant des artefacts. Raison pourlaquelle les modalités de datation rarement établie de manière normée. Car en divisant le corpus en 3 obtient périodes issues de la division du corpus.
La division du corpus qui établit les modalités d’adaptation plutôt qu’une adaptation normée.


## Analyse factorielle multivariée

CSV, corpus prêt pour l’analyse statistique.
Plusieurs façons de travailler. Personnellement utilise l’Analyse factorielle multivariée. Surtout car cette analyse se prête parfaitement aux corpus historiques qui concernent un même corpus.
Type d’analyse qui se prête parfaitement au caractère relationnel du corpus selon ses modalités. Identifier la mpolarisation d’une population par le calcul de distance entre les modalités multiples.

Méthode Bertin Cibois.
Calcul de distance en fonction des écarts à l’indépendance. 
Pas seulement croiser entre elles deux valeurs isolées de leur contexte mais toujours tenir compte de ce contexte pour tirer des résultats issus de leur croisement.

## Analyse

Recours au programme R
Générer deux graphiques
- distribution tridimentionnelles
- graphique à barre pour le croisement de manière visualiser l’effet de polarisation

Premier graphique distribution de la population, permet de saisir rapidement la polarisation des individus sous la forme de clusters ou d’agrégats. Il s’agit de graphiques tridimensionnels, axes qui expriment les tendances polarisantes. Possible de choisir des axes distincts pour mieux évaluer les tendances.

Ici axe 1 et 3 qui offraient la meilleure visualisation.
D’emblée, hormis quelques individus isolés. On constate dès le premier coup d’œil que le corpus n’est pas immédiatement éclaté ce qui reflfète sa relative cohésien.

Ensuite possible de filtrer la cohésion en fonction de certains caractères pour voir où se concentre la polarité.
Population bien polarisée en fonction de ce caractère, ce qui valide donc l’enquête identitaire.

Possible de croiser ces caractères avec la méthode Bertin-Cibois.
Croisements effectués impliquent tous ce caractère clérical.
Premier croisement lieu : abbaye, cathédrale et autre. Or, le graphique montre très nettement des tendances fortes avec des écarts à l’indépendance.

Correspondance marquée entre la cathégorie d’abbé et d’abbaye. Abbé y reste souvent après sa mort.
Pour les évêques l’attachement à la cathédrale moins important mais pas absolu.

Localisation des tombeaux à l’intérieur même des lieux, en partie établi par le statut des défunts. Sanctuaire des églises typiquement pour les évêques, pour les abbés le cloître.

Caractères internes. Profond attrait matériaux précieux pour les évêques dont le cuivre. Pour les abbés la pierre.
Ostensation et prestige et humilité.

Sans surprise, se déploie également dans le format même des tombeaux. Ronde-bosse vs plate-tombe.
Absence éphigie chez les abbés.

Confirmer avec les mathématiques ce qui aurait pu relever de l’intuition. 

Pour la crosse, l’analyse factoriel, rôle encore plus positif car permet de trancher si sa position signale un statut particulier. En se référant à des sources médiévales, supposé que rerprésentation devait être présentée de la même manière : juridiction tournée vers l’extérieur ou l’intérieur. Logique lithurgique. De même, gauche et droite.

Premier croisement statistique qui permet de montrer que évêques tendance porter la crosse à gauche, abbé à droite.
25 exceptions chez les abbés soit le 1/4

Crosseron, ouverture vers la droite plus fréquente chez les abbés. Mais données peut concluantes pour affirmer claire tendance. Impossible d’affirmer que position déterminée par le statut desdéfunts.

Habits mitrés. Alors réalisé que symmétrie entre tombeaux des évêques et tombeaux mitrés. Nouveau croisement. Totalité évêque qui portent à gauche, proche abbés.

En les retranchant, écarts à l’indépendance beaucoup plus tranchés.

Découverte au sujet de la crosse montre tout l’intérêt d’effectuer une analyse statistique importante. Pas seulement faire ressortir des tendances, fréquences. Analyse qui permet de faire ressortir des exceptions à la règle. En forçant à interroger ce qui autrement aurait passé inaperçu. Aller-retours fertiles entre masse de données et analyse qui aurait échappé à des facteurs individuels.


Question utilisation IA 

Question quantitatif et HA
Quantitatif et numérique.

Forme de curation que le corpus comment traité. Avoir plus de 250 exemples, corpus important.

Objectif est d’obtenir un échantillon, dès lors qu’est conscient des bais de ce corpus. Moi-même aussi effectué des sélection. Mais s’assurer que l’on ait une bonne distribution.

Beaucoup d’arbitraire dans la collection Gagnières.
Tenté en ayant recours à Palissy de faire la même chose avec tombeaux existants. Pas énormément photographies mauvaises. 125 tombeaux et finalement corpus pauvre.

Préciser aussi que les modalités ne vont pas dans le détail non plus.

Statistique et quantitatif. Se complète, un outils essentiel au virage que doit emprunter l’histoire de l’art en général pour concilier l’individuel et les données massives. S’intéresser à un individu, intéressant, mais ne permet pas de comprendre la dynamique générale. Peut-on formalisaer les tableaux de Poussin. Matériaux, mais pour les catégories. Un outil pratique.

Question sur l’encodage. Caractère un peu binaire.
Quel processus ?
L’idéal pour l’analyse factoriel, avoir peu de modalités. 2 caractères et oui/non.
Problématique identitaire qui orientait la grille de codage. Pas intéressé à la présence des anges, des animaux. A limité ses caractères. Aurait pu avoir plus de modalités, car plusieurs fois autre : rassemble d’autres modalités mais concernait très peu d’individus. Pas eu trop de difficultés à produire la grille de codage.

Le plus difficile la crosse et le crosseron. Direction du crosseron et celle par rapport à l’éffigie.

Thèse 1 500 individus. Là qu’apris que bloque si trop peu.

Corpsu des abbés, quid des différences entre les cisterciens et les bénédictains. Les puristes les cisterciens.

Article qui débute avec citation de Bernard de Clairveaux.

Question des exceptions