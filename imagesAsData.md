---
title: Images as data
description: CR de présentation de Laurent Tilton (university of Richmond, midi du CRIHN
author: ouvroir
date: 2022-03-29
draft: true
tags:
    - cr


---

# Images as Data

[Lauren Tilton](https://rhetoric.richmond.edu/faculty/ltilton/)
- PhD Yale
- associate professor, University of Richmond
- Humanities Data in Art
- [Photogrammar](https://photogrammar.org/maps)

midi du CRIHN en partenariat avec le département d'histoire de l'art et d'études cinématographiques

How might viewing images through computational methods support the study of visual culture?
- [distant viewing Lab ](https://www.distantviewing.org/) with Taylor Arnold: intersection between disciplines and fields
- papers, software, datasets & other forms of scholarship

Data science / digital humanities <> visual culture studies

What is this an image of? 
- computation and humanistic frame 

Arnold and Tilton, _Distant Viewing_, MIT Press
Computer vision:
- computational mode and technology of communication
- people must assign which features to view in images
- not outside of cultura, social, and historical ways of seeing and practices of looking
- theory and method for the computational exploration of images through the application of computer vision

It is quite hard to tell a computer _how to see_
- what is it an image of? 
- objects
- scene
- people
- environment

Computer breaks pixels into arrays of number to which meaning is assigned (sgnifier)
- almost infinite array of pixels that can "represent" the same object, such as a bike, endless configurations that represent the same concept
Field of computer vision focuses on how computers automatically produce ways of understing digital images
- training algorithms to look in the ways we are interested in

Distant: 
- distant from the eye, for computational methods "see" by calculating images as numbers
- disntace as scale, interpretation of images can exceed a person's physical ability to view (where's the payoff if you are not scaling up?)

Viewing:
- process of deconding → therefore not objective
- making explicit the computational processing of images shaped by ways of seeing and practices of looking
- acknowledging that images convey messages differently than forms such as text and their computational corrolaries such as characters

Neither neutral nor objective space


## Method
- **Annotate** the corpus algorithmically, using and adapting computer vision and machine learning algorithms to create and identify a code system (naming the pixels)
- **Organise** the annotations and metadata (data and image data reuninification)
- **Explore** the data wih visualizations, models, summary statistics and other EDA methods (exploratory data analysis, John Tukey, framework and theory)
- **Communicate** results such as through public projects and scolarly venues

Pipeline: data science, not assuming you already have the data but adding the step of creating your dataset (from forms of data, including visual data)

## Exploring a collection
American government photography FSA-OWI project
- images to support the new deal
- expanding the vision for the collection: document/archive the current state of America

filing the photographs with phtographer and caption. Trying to figure out how to organise them → how to archive a photography collection? (though museums and archives)

How to get an understaing of the entire archive, not just the 6 to 8 very famous of photographs? 
How to look at it "as a whole"? 
Common focus a certain type of images of rural poverty that are circulating constantly. Geogrpahically and spacially pretty narrow, as well as for the photographers. 

current interface at the [Library of Congress](https://www.loc.gov/pictures/collection/fsac/)

How to use distant viewing to view it as a whole.
- collect: scraped all the data from the LO, metadata and images (in 2010, there was no API, now there is but they broke the API because the size of the collection is larger than the page capacity of the API)
- Annotate: identify eements, algorithm created bounding boxes and attaches labels to it
- organize: find themes using the algorithms' categories, image similarity, using metadata
- explore: by variable 
- communicate: 
    - methodological papers
    - [public site](https://photogrammar.org/maps) that tries to communicate arguments (interpretive lens) while still being exploratory, reorient how we think about the collection while offering a new perspective. Follow a photographer accross the country though time, delve further into a phtography. Using image similarity for recommendations, allowing to discovery of the 40'000 photographs that had no metadata
    - [ADDI viewer](https://github.com/distant-viewing/addi): shows the algorithmic decision making of different models

labels such as `mountain`, `sky`, `person`, `horse`
thing: can be counted
stuff: can't be counted
can interpret *where* in the frame a label is, spatial/compositional information

Back and forth: annotate, explore, annotate, explore...

image similarity: stopping a neural network before the final layer, identifying similarity without telling the how. Is not told to look for something but just matches images, makes connections
- images that resemble each other to the eye of the machine
- netwoek of photographers by style

viewing the images again, in a different way, using the algorithm (creating boxes for ground and sky, conveying strenght and monumentality by looking up to DC)

how to automate captions to facilitate discovery and access?

### DVT distant viewing toolkit
open source python toolkit : funding announcement to come for a GUI making it more accessible, and exporting the data to explore it in other software such as pixplot (connection tools)

## Questions
Would you be able to determine which kind of lens was used? 
- probably, reverse-engineering. Very interesting questions, to be explored

The copyright question
- between caution and exploratory approach

ADDI viewer
- at which stage did you come to work on it, how did it come about formally and informally
- 5 collections of early 20th century photography collections of LOC
- analysing how alogrithms act when applied on these data sets
- interface reveals some of the ways the alorigthms that are making decisions