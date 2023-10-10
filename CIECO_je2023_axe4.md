---
title: JE «Ouverture et sémantisation de données culturelles»
author: ouvroir
date: 2023-10-10
draft: 
tags:
     - cr


---


# Ouverture et sémantisation de données culturelles. Perspectives transatlantiques

> Depuis le slogan « Raw data, now! » lancé par Tim Berners Lee en 2012, de nombreuses initiatives ont été lancées tant par les gouvernements que par les institutions culturelles pour ouvrir leurs collections. Après les premières initiatives d’envergure du British Museum ou du Rijksmuseum, l’enquête Open Glam-survey recense plus de 2 600 jeux de données, dont une faible part seulement est publiée en données ouvertes et liées. Force est de constater le peu de place encore occupée par les musées canadiens dans cette enquête. Au moment où la question de l’ouverture des données présente une forte actualité au Canada et au Québec avec les initiatives du Réseau canadien d’information sur le patrimoine (RCIP), les mesures du Plan culturel numérique du Québec, ou encore le Linked Infrastructure for Networked Cultural Scholarship (LINCS). Cette journée d’étude vise à mettre en contact la communauté canadienne et la communauté européenne des Open GLAM en reconnaissant que des données ouvertes aux contenus ouverts, il existe divers modes d’ouverture des collections.


Introduction par Emmanuel Château-Dutier et Andrea Kuchembuck

## Getty Vocabularies: Current Developments, Focus on ULAN
Patricia Harping (Getty Research Institute, Getty vocabulary Program managing editor, États-Unis)

### What are the Getty vocabularies
committing resources to standards and vocabularies since the 1980s

5 Getty vocabularies
- ULAN: names and other rich data for artists, architects, firms, studios, patrons etc. 
    - unique IDs
    - display bio, birth-death, nationalities, roles
    - associative relationships to other people on ULAN
    - contributors and sources, co-references  to other resources
- AAT Art & Architecture thesaurus: terms in several languages, relationships, ...
- TGN Thesaurus of Geographic Names
- IA Iconography authority: proper names, relationships, dates for iconographical narratives, religious or fictional caraters, ...
- CONA cultural objects name authrotiy: titles, artist attribution, cration dates, relationships 

### Why Getty vocabularies
Example of vocabularies used in an object record
Linking to the ULAN vocabulary record
1. disambiguate the entity
2. use associated rich data

Object record: link to the JSON, URI for the concept, link to the term if you want a specific language or term

Purpose
- promote consistency
- retrieval and discovery: rich contextual data

Key characteristics
- standards compliant
    - thesauri compliant = semantic network of unique concepts: hierarchical, associative, equivalent
- authoritative
- reliable future
- unique vocabularies
- rich knowledge bases
- collaborative: grow through contribution from the expert user community → make it relatively easy to contribute

vocab@getty.edu
- process contribution
- quality and scope control

### Current status and priorities for the future
- terms and users are largely western → measure multiculturality with languages. How to make vocabularies more multilingual, multicultural, ...
- definiting the issues → avoid use flags
- expression of ambiguity and uncertainty
- polyhierarchy: multiple classifications for places that are claimed by USA as well as by the Navajo

OpenRefine reconciliation service

SPARQL end point

Improve Interconnectivity

### Questions
Emmanuel Château-Dutier: Makers, instead of artists? adressed in Canada
- ULAN contains makers, one does not have to be a fine art artist to be a part of ULAN, but they haven't changed it since its creation 

Andrea Kuchembuck: Elaborate on interconnectivity between different systems
- still a bit weak on interconnectivity, with VIAF for example
- built by hand until now, but they are working on it

Lena Krause: collectives, specific challenge in street art and changing members of artist collectives
- no worked on it
- deal with architectural firms, have dates associated with relationship so state dates of when people 
<!-- @MaisonMONA would welcome examples if we want to send some in-->

Isolda Gavidia: How do they work on the multilingual aspect of the vocabularies?
- have been working with the user community

Nathalie Thibault: Au MNBAQ, nous avons en commun avec la base ULAN  (1098 créateurs, artistes) 25% de nos collections.. C'est la base Wikidata qui nous permet de faire une veille quotidienne avec ULAN et de comparer nos données.  Je remarque l'élément Wikidata d'un artiste est utilisé dans les données ULAN. Comment se fait cette union? 
- users are doing it
<!-- @MaisonMONA should we send in our reconciliated artists?-->

Do you think museums should use ULAN or use Wikidata? 
- ULAN is better as it is updated more regularly


## BAnQ: agence ISNI pour le Québec
Danielle Poirier (Directrice des métadonnées et de la normalisation bibliographiques, Direction générale de la Bibliothèque nationale, Bibliothèques et Archives nationales du Québec, Canada)

ISNI:
- identifiant unique
- normalisé ISO
- de portée universelle
- 16 chiffres
- exprimé dans un URI

ISNI: personnes ou organismes qui créent, collaborent, produisent, distribuent des contenus principalement culturels

À quoi sert-il? 
- identifier de manière univoque et pérenne des personnes et des organismes
- psserelle entre différentes bases de données

administré par une agence internationale à Londres, données conservées dans un base d'OCLC

BANQ devient agence ISNI pour faire suite à la mesure 111 (Plan d'action concernant les données sur les contenus culturlels québécois) du Plan culturel numérique du Québec
- représenter tous les milieux: musées, livre, arts de la scène, ...
- maintient du fichier d'autorité

Grandes étapes du projet (1 an)
1. Envoi massif de données (personnes et organismes) csv
    - 220800 personnes
    - 77700 collectivités
3. Développer un module d'envoi automatique quotidien
4. Envoi de demandes individuelles par formulaire pour les documents non couverts par le dépôt légal, service élargi
    - génèrent des données d'autorités à partir du formulaire
    - formulaire pour ajout individuel: 1 personne, pas de batch pour le moment

Tableau de bord
- interne
- suivi des envois 

Et maintenant
- mise en valeur: arrimage à d'autres sources de données 
    - wikidata! (Rhizome: écrivains québécois)
    - wikipedia
- en discussion avec le RAAV actuellement
<!-- @maisonMONA entrer en contact pour présenter notre projet: isni@banq.qc.ca, danielle.poirier@banq.qc.ca-->





### Questions

Nathalie Thibault: Au MNBAQ, nous avons 2265 artistes, créateurs, écrivains avec un ISNI. Plus de 50% de nos artistes. Nous créons des autorités ISNI pour des artistes décédés (depuis plus de 30 ans) Pour les artistes vivants, nous leur acheminons le lien pour créer eux-mêmes leur identifiant

Quels sont les mécanismes internes de résolution de l'autorité? 
- mutualisation de données
- logiciel qui compare avec l'existant dans la base
- système de pointage par zone
- résolution manuelle

Lena Krause: Que faire avec les différentes autorités: ULAN, Wikidata, ...?
- BANQ: reçoivent des documents d'artistes → dépôt à la BANQ → fiche d'autorité
- ISNI est inter/multi-domaine

Nathalie Thibault
- ULAN → dimension internationale 
- ISNI → permet de savoir s'il y a eu des documents qui ont été publiés par l'artiste, gravures déposées etc. Augmente l'interopérabilité avec les fonds de la BANQ
- Wikidata → multilingue, nourrit les artistes québécois et canadiens

Federico Nurra
- ISNI: **autorité pour œuvres déposée**s, gestion bibliothéconomiques, n'a pas de mission encyclopédique
- ULAN: pourrait avoir cette ambition encyclopédique
- wikidata: aspect communautaire, agrège ce qui est en ligne, fonctionne comme un hub mais sans qu'il y ait le contrôle plus "propre" de l'ISNI et ULAN
- en France: IDREF à la fois sur l'alimentation institutionelle mais aussi la contribution de chercheur·e·s et de la communauté
- difficile équilibre entre l'institutionnel et le communautaire

Federico Nurra: développement de l'identité numérique, ORCID. Prévu des formes de moissonnage de ces identifiants liés aux auteurs par rapport aux publications courantes et futures, publications numériques? 
- oui, le dépôt se fait 

Emmanuel Château-Dutier: ISNI fournit des identifiants et non des notices. Cependant sa portée est encyclopédique selon lui, c'est plutôt l'effet des contributeur·se·s? 
- toute les personnes qui ont contribué à une œuvre
- toutes les œuvres ne seront pas présentes dans l'ISNI, c'est une base de données pour les personnes


## Table ronde 

Animée par 
- Emmanuel Chateau-Dutier (Professeur en muséologie numérique, Université de Montréal) 
- Cindy Veilleux (Responsable des projets de diffusion numérique des collections, Musée d’art contemporain de Montréal)

Avec la participation de 
- Andrea Kuchembuck (Directrice de la gestion des collection, des ressources documentaires, des services techniques et de l'audiovisuel, Musée d’art contemporain de Montréal, Canada)
- Federico Nurra (Chef du service numérique de la recherche à l’Institut national d’histoire de l’art, France)
- Danielle Poirier (Directrice des métadonnées et de la normalisation bibliographiques, Direction générale de la Bibliothèque nationale, Bibliothèques et Archives nationales du Québec, Canada)
- Alexandre Naud (conseiller en développement culturel numérique au MCC, co-responsable de la stratégie commune franco-québécoise sur la visibilité des artistes francophones)



A.K.: situation particulière au MAC, 97% des artistes dans la collection sont des artistes vivants. Diffusion des données sur le MACrépertoire, contact de l'ensemble des artistes pour les droits → données sont véritablement à jour.
- mise à jour de l'information: processus énergivore
- question des renseignements personnels et des droits & identification des ayants droits
- partage de l'information et de l'interopérabilité

F.N.: établissement avec double-tutelle enseignement&recherche
- AGORAH (2006 - ): plateforme des données de la recherche de l'IHNA et de ses partenaires. Personnes sont des notices documentaires, pas de référentiel SKOS, intégration
- refonte d'AGORAH (2019 -) choix de garder cette structure mais en passant par un modèle en graphe et les exposer par les biais des ontologies les plus répandues dans le domaine. Alignement des notices à des référentiels et d'autres autorités: ISNI, VIAF, IDREF, ULAN
- [GINCO](http://culturecommunication.github.io/ginco/) est une application multiutilisateurs dédiée à la gestion de référentiels terminologiques

A.N.: MCC dans la même dynamique, rôle de sensibilisation et de développement d'une certaine culture de la donnée dans le domaine. 
- État des lieux de l'utilisation des données dans le domaine fait par l'OCCQ: démontre enjeux, silos, désintérêt parfois
- portion de l'autorité: [RPCQ](https://www.patrimoine-culturel.gouv.qc.ca/rpcq/accueil.do;jsessionid=4A5D4D335FED5478FEEC0D5C3DD0CEBC?methode=afficher)
- ont des identifiants propres au ministère
- mesure 111 
- travail de littératie numériqu
alexandre.naud@mcc.gouv.qc.ca
e à faire

D.P.: BANQ rôle intéressant serait la collaboration, recevoir de la donnée pour les artistes dont les estampes n'auraient pas été traitées encore par exemple

Consentement & renseignements personnels
D.P.: 3 cases à cocher dans le formulaire et ajustements avec la loi 25, volonté d'améliorer ça encore
A.K.: genre, identité / origine

F.N: Agorah 
- une faiblesse dans les genres (homme, femme, inconnu), champs pas toujours renseigné. Sources historiques
- même problème pour les nationalités, parti pris a été d'associer la nationalité à l'empreinte géographique contemporaine du pays, ce qui pose de véritables soucis sur les régions en conflit par exemple. Contrainte de limiter une explosion de termes différents (ce qui arrive pour la gestion de termes géographiques)
- communauté scientifique doit s'interroger avant de pouvoir répondre à des enjeux socio-culturels

A.K.: Questions de la valorisation de la culture autochtone: enjeux de dénomination des lieux, des groupes culturels

E.C-D: Ontologie des populations autochtones, document encore sous forme tabulaire. Partage d'autorité autour de l'élaboration de ces données

E.C-D: Questions de validation et auto-déclaration. Comment collecter l'auto-déclaration:
- AK: formulaire de l'ISNI est un début
- AK: pratiques basées sur l'usage jusqu'à présent, les successions ont également leur mot à dire

E.C-D: Est-ce que la BANQ reçoit des demandes de rectifications? 
DP: oui par courriel, demande de retrait d'information 

E.C-D: MCC pas en capacité de proposer des solutions techniques pour endosser la gestion d'autorité. Wikidata comme hub: lie des autorités existantes, est-ce une solution viable? Déléguer la gestion des autorités? 
- F.N: LOUD linked open usable data. Création de données sémantiques, mais nous ne créons pas les interfaces pour rendre accessible l'information. 
- F.N: Wikidata comme pont, parce que c'est simple à utiliser. Requiert mise à disposition d'API simples pour l'utilisation de ces ressources. Créer des autorités, mais aussi des interfaces pour utiliser/réutiliser des données? 

A.K: hésitation d'envoyer l'information à l'extérieur, à l'étranger → ce qu'on peut partager, ce qu'on ne peut pas. Mais en ce moment le MAC détient l'information la plus à jour

A.N: Question de l'interface est un enjeu et d'y rester agile. Normaliser la diversité est un enjeu à tous les points de vue. 
- Avantage dans la facilité de Wiki était l'évolution de la plateforme mais aussi la contribution des pairs. Solution à court terme car outil simple pour regrouper des identifiants
- Dans un monde parfait, il y aurait un seul gestionnaire d'autorité, mais ni possible ni viable. Dépend du point de vue pris sur les objectifs. Mais on ne peut pas demander aux institutions d'avoir le même niveau et de cumuler dans les bd l'ensemble des identifiants possibles. Requiert de prendre les décisions les plus logiques: quelques notices d'autorités par excellence, représentatives du secteur pour prendre en considération les besoins du milieu
- mettre en place des bonnes pratiques

E.C-D: partage d'autorité? partage d'expérience
- F.N: [ONOMA](https://wwwdev.inha.fr/fr/agenda/parcourir-par-annee/en-2017/juin-2017/onoma-un-referentiel-d-acteurs-du-ministere-de-la-culture-ancre-dans-le-web-semantique.html) → projet adHoc porté par le ministère (FR). Temps n'était pas mûr pour le mettre en œuvre. Il n'y avait pas de service numérique au ministère de la culture, quelques persones qui comprenaient les enjeux et portaient le projet mais ça manquait de prise auprès des institutions. C'était il y a 8 ans, aujourd'hui les besoins émergent avec l'exposition de collection en ligne mais les choses ont beaucoup changé. Il y avait un manque d'infrastructure portante: peut-être avec la nouvelle organisation du ministère avec un service numérique. Travail louable dans la sensibilisation 

E.C-D: partage d'autorité? BANQ collaboration enrichie avec les musées? produire les autorités dans un écosystème culturel?
- D.P.: recevoir de la données de certains partenaires externes 
- D.P.: données partagées dans VIAF, donnéesQuébec mises à jour à chaque semaine. Projet de partager les données d'autorité mais en pause à cause de la loi 25, cherche une certitude à ne pas causer de vague.

A.K: MAC œuvres sont du patrimoine public national donc responsabilité de contribuer les données à des autorités.

E.C-D: Préparation des données, qu'est-ce que ça signifie, pour les institutions, sont-elles prêtes à utiliser et à partager des données d'autorité? Est-ce que les logiciels le permettent? Quelles sont les conditions préalables en terme de normalisation des données, étapes nécessaires pour mettre en place pour de tels dispositifs?
Est-ce que le MAC utilise des autorités? 
- A.K.: processus de validation multi-source: ULAN, Artists in Canada, LOC. La plupart des informations ont été mises à jour. Moment particulier, à la veille d'une migration de base de données → changement technologique qui permettrait d'aller plus loin (autant pousser l'information que l'importer) que le système utilisé depuis 20 ans
- F.N.: préparation → faire pression sur les éditeurs de progiciels pour faire évoluer les services. Insérer dans le cahier des charges les besoins explicites de contribuer et pouvoir intégrer les autorités
- A.N.: demander minimalement un identifiant ISNI pour les dépôts de projets, incitatifs et stratégies pour continuer à sensibiliser. Objectif du PCNQ: aider le milieu à se structurer

D.P: système désuet donc dans le cahier des charges, insistent pour avoir un avoir un système qui supportera des données RDF ou du moins partageables. Données respectent la norme RDA qui a connu une refonte complète qui permettre de les lier plus facilement. 

E.C-D: Bénéfices à la production et à la diffusion de données d'autorités? A-t-on des exemples réussi, quelles sont les opportunités que ça ouvre? 
- F.N.: visibilité en ligne = visibilité dans le monde réel. 
- A.K: faire des liens interdomaine serait un grand avantage d'une vision plus holistique de l'œuvre dans son contexte de création. Avec le projet de transformation du bâtiment → partie de la collection n'est pas accessible, se basent beaucoup sur la diffusion numérique est d'autant plus important.
- A.N: obligation de la vision du patrimoine = préserver le patrimoine avec des données claires et bien structurées. Visibilité au sein de l'hyper-offre culturelle. Pari est de travailler sur la qualité de la donnnée car c'est un levier pour la découvrabilité pour permettre aux producteurs de rayonner. Modèle capacoa, dialog, liq (librairies indépendantes du québec): petits projets qui donnent espoir
- D.P: collaboration, essayer de pousser les identifiants aux producteurs pour que ce soit déjà indiqué lors des dépôts.

### Questions

L.K: Documentation publique du opt out?
- reseigner le fait que les gens ne veulent pas qu'on renseigne le genre pourrait aussi poser problème.
- inexistant pour le moment