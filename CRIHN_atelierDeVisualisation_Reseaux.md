---
title: Atelier de visualisation
description: notes de l'atelier de visualisation avec Anton Boudreau Ninkov avec le CRIHN
author: ouvroir
date: 2023-04-18
draft: true
tags:
    - cr
    
---
# Visualizing Litterary Social Networks in the Fred Wah Digital Archive

Atelier de visualisation avec Anton Boudreau Ninkov and Deanna Fong

## Deanna's research
[Fred Wah Digital Archive](https://fredwah.ca/)
- canadian poet of Swedish and Chinese origin
- work that is situated within the community: names, places, institutions, publications

How can network analysis yield a more complex and nuanced picture of the social context within, and surrounding Wah's work?

## Anton's work
Qu'est-ce que l'analyse de réseau? connexion/relations (arrêtes) entre les entités/acteurs (nœuds)
- identifier les structures des groupes et des clusters
- identifier les positions des entités individuelles

### Use of Network Analysis in Anton's work
varied analysis of metadata with textual documents

**Analyse par co-liens des sites web consacrés aux vaccins** (avant la COVID, 2014-2019)
- co-lien: sites qui sont référés (par lien) par le même blog/site
- analyse links by crawling websites to represent the network
- au sein de chaque groupe, des sous-groupes se manifestent

Système de visualisation pour interragir avec la visualisation en réseau, sélection pour afficher de la métadonnée: mot-clefs, carte, sentiment analysis
Way to apply context to data visualisation
tool built in [Tableau](https://www.tableau.com/learn/articles/data-visualization): tool selected because he thought it would be easier, but ended up programming in js in Tableau... Would probably have built the whole thing in D3 if he had known. Tableau is "free" for students, but better to subscribe to free software

**L'analyse des mots-clés dans le temps des publications d'éduction médicale**
- keyword network analysis
- each article has keywords associated with it → see similarity in use of keywords
- requires a lot of data cleaning
- evolution of clusters through time periods, following the narrative

[VosViewer](https://www.vosviewer.com/) (Leiden University, based for bibliometric research)

**Le réseau de collaborations Fred Wah**
- site web qui a concentré et catalogué toutes ses œuvres dans un seul espace sur le web, built in [Drupal](https://www.drupal.org/about/9) (originally 7, recently upgraded to 9, great as it structures data but strict, when it comes to changing the structure)
- créer des analyses de réseau visuelles des collaborations du réseau Fred Wah pour mieux comprendre son travail collectif

## Collaboration

First step: export the data from Drupal
- csv export (work in progress): publication, name
- viewing collaborations, how people are connected together through Fred Wah

[Gephi](https://gephi.org/)
- proximity to show the similarities
- removed the lines because too many links
- litterally every relation is flat (co-writing, edition, review, dedication mention)

Reading the visualisation after a decade of studying canadian litterature
- blue cluster: work around identity writing (chinese-candian heritage)
- orange: as a more mature poet and writer, becomes included in anthologies such as "greatest canadian poets"
- green: generation, shared aesthetic "experimental"
- dark green: american modernists in a transnational moment of contact
- Roy Kyoka → in the middle, person who had a lot of friends and connected everybody

Bringing back the lines
working on other aspects

Ethics
- what questions do we want to ask of our data set? 
- what context is needed to make sens of what we're seeing? 
- what is our responsability to communities of production as custorians and interpreters of this data? 

Biographical information for each node (person)
Relationships of labour and care that go into building a community

View with more nuance without loosing the contextualisation

> There is a whole world yet to be discovered

## Discussion

How to address contextualisation? 
Felicity Tailor, *desire lines* (exposition [ici]](https://www.uottawa.ca/bibliotheque/toutes-nouvelles/exposition-desire-lines) et [ici](https://artexte.ca/exposition/desire-lines-des-espaces-narratifs-en-deplacement/?noredirect=fr_CA))
- 3 journals published in Toronto around the same time: art, political activism
- network analysis to see people who are central
- went back to the community and had live oral history interviews


"This is a representation of something we can make sense of =/= this is the reality"