# Formation IIIF
27 juin - 1er juillet 2022

[Slack](https://app.slack.com/client/T0AL6BTUL/C03LSDDQ4SJ)

[Agenda](https://training.iiif.io/iiif-online-workshop/June2022.html#sessions)



## Introductions and course overview

Course teacher: Glen Robson

### Participants

- Zachary Miller (Dartmouth College) <!-- fellow -->
- Richel Cuyler (Dartmouth College)
- Lena Krause (Université de Montréal)
- Katie Romabiles (Metropolitan New York Library Council) <!-- using cantaploupe-->
- Dana Kerdesky (Dartmouth College) <!-- fellow -->
- Shawné Michaelain Holloway (Black Lunch Table) <!-- audio & multimedia archive -->
- Jenny Mullins (Dartmouth College)
- Jacob Hill (Stanford) <!-- data and service manager at digital archive, IIIF data harvesting + consultation for feature development at mirador -->
- Julia Murphy (Hirshhorn Museum and Sculpture Garden) <!-- digital asset manager and head of photography, modern and contemporary art museum, Washington DC -->

### Course overview

Homework + add questions to the agenda for tomorrow

Listen to guest presentations (in overview): can ask for a topic if it isn't covered

Thursday: 1 on 1 meeting, sign up with calendly

Friday demo session

### What is IIIF?

this year: making IIIF more accessible to smaller institutions

- [ ] add UdeM to the map

fast access to high quality images

iiif v3: added support audio-visual (supported by universal viewer)

interoperable → viewers:

- mirador, more annotation content
- universal viewer
- [Tify (germany)](https://demo.tify.rocks/demo.html?manifest=https://damsssl.llgc.org.uk/iiif/2.0/4574752/manifest.json)
- [IIIF Curation Viewer](http://codh.rois.ac.jp/software/iiif-curation-viewer/demo/?manifest=https://damsssl.llgc.org.uk/iiif/2.0/4574752/manifest.json) (japan), machine learning to interpret japanese characters

Framework

- Image API
- Presentation API
- [Content Search API](https://iiif.io/api/search/1.0) - to search annotations a but like a searching within a PDF file
- [Authentication API](https://iiif.io/api/auth/1.0) - for protecting resources by username or giving lower quality images to unauthenticated users
- [Change Discovery API](https://iiif.io/api/discovery/) - for Aggregators like Europeana to harvest IIIF data
- [Content State API](https://iiif.io/api/content-state/) - to improve the method of taking content from one viewer to another
- [Maps Extension](https://iiif.io/api/extension/navplace/) - to link a Geographical place to a IIIF image. Could be used to Georeference a map or photograph <!-- possible to add multiple locations but not structured/specific metadata-->

IIIF is focused on the presentation but not on creating detailed metadata 

Guides to finidng IIIF Resources: how to find the IIIF resource on the website

- [ ] add UdeM ressources



For tomorrow: 

- intro excercices (try different viewers)
- 1h image API video

## Image API
- best image format ? 
- Good to keep copies in different formats ?
    - archival copy: quality
    - iiif copy: we can compress it
    - all others can be generated on the fly
- minimum resolution ? 
    - no absolute minium
    - problems when the images are small (smallest ok: iphone images), else you don't get the benefit of fast image access
    - way to use a non IIIF image in a manifest (extra)

composite image: 
- one in background, others on top
- overlay requires all images to be iiif (in mirador)
- paint multiple images on a canvas

### Questions
- quels types d'annotations textuelles (ie analyse/interprétation, source, notes)
- meilleurs endroit pour stocker les annotations textuelles ? (dans le manifest ou ailleurs ?)
- quels sont les différents layers ? 
- Comment réperer les zones ? 
- Comment repérer ces différents types d'annotation dans le manifest ?



Photoshop → Save Image Pyramid

Preserves multiresolution information. Photoshop does not provide options for opening multiresolution files; the image opens at the highest resolution within the file. However, Adobe InDesign and some image servers provide support for opening multiresolution formats.



people have multiple image servers behind a proxy to serve hundreds and thousands of users. They all work with the same storage. 

- pyramid tif is fastest to load

supports any input format, but some work better than other
- pyramid tif and jpeg2000: getting higher qualities as you zoom in
- pyramid tif  careful: space requirements → creates very large files but faster than other formats
- larger institutions are using jpeg2000 to reduce storage and therefore cost

Processors
kakadu decoding library (paying, but no free one works as well)

functionality for user to download a copy, create links to different resolutions  

## Presentation API

presentation API [libraries](https://github.com/IIIF/awesome-iiif#presentation-api-libraries)

### Contents

#### manifest _1..*_ sequence _1..*_ canvas _1..*_ content

manifest: json-ld
- label
- metadata and description
- attribution (provider of the manifest)
- licence
- logo (visual branding to indicate the provider of the content)

sequence: ordering

canvas: holder for image contents and other types of annotations
- height and width create and abstract coordinate space

content _1..*_ ressources: images, other types of content annotated onto it

multiple images annotated onto a single canvas: overlay 7:13 [à regarder ensemble!]
<!--terme annotation utilisé pour dire "placé sur le canva"-->

#### Canvas
{
    @type: "sc:Canvas",
    @id: "example.org/canvas/id/1",
    label: "recto, unframed", <!-- display label-->
    height: 2000,
    width: 1500,
    images: [ ...annotations... ] <!-- contains the annotations that paint the image on the canvas-->
}

#### Annotation
{
    @id: "example.org/annotation/id/1",
    @type: "oa:Annotation",
    motivation: "sc:painting", <!-- in the specifications: painting content onto a canvas-->
    on: "example.org/canvas/id/1", <!-- id of the canvas-->
    ressource: { <!-- references an image-->
        @id: "example.org/iiif/123/full/1500,/0/default.jpg",
        @type: "dctypes:Image",
        format: "image/jpeg",
        service: { ...Image API Service...}
        height: 2000,
        width: 1500
    }
}

#### Service
Image API service

reference to the IIIF image API service for the image 
the viewer sees the service and contacts the image API server and requests the content required to be rendered


index --> navigation

### Questions 2022-06-29

- Is there a manifest editor for presentation API v3 ?
  - should be coming out soon
  - should be more complete
- Compatibility between v2 and v3? Our server (small testing server set up by our library) is in v3 and it seems to be causing many issues and errors (it’s hard to distinguish between our mistakes and compatibility issues). 
  - use the [iiif presentation validator](https://presentation-validator.iiif.io/)
  - escaping the / into %2f for cantaloupe to understand that the slashes in the path are the path
- v2 vs v3: [cookbook](https://iiif.io/api/cookbook/recipe/matrix/)
  - v3 supports AV, v2 doesn't
  - v3 manifest can use v2 images but not the contrary (v2 manifest cannot use v3 images)
  - changes in json field
  - [vault](https://github.com/IIIF-Commons/vault) : tool that updates v2 to v3
  - language map
  - no more sequences: list of items

3D and photogrammetry: not yet supported but will be probably in v4 (still early on in the process, x y time and 4th dimension?)

- 3D technical group is open to everybody
- probably couple years before viewers support it
- [UV supports 3D](https://uv-v4.netlify.app/#?c=&m=&cv=&xywh=-2403https://uv-v4.netlify.app/%23?c=&m=&cv=&xywh=-2403%2C-197%2C7373%2C3936&iiifManifestId=https%3A%2F%2Fbiiif-template-example-3kntb3jpl-mnemoscene.vercel.app%2F3d%2Findex.jsonC-197https://uv-v4.netlify.app/%23?c=&m=&cv=&xywh=-2403%2C-197%2C7373%2C3936&iiifManifestId=https%3A%2F%2Fbiiif-template-example-3kntb3jpl-mnemoscene.vercel.app%2F3d%2Findex.jsonC7373https://uv-v4.netlify.app/%23?c=&m=&cv=&xywh=-2403%2C-197%2C7373%2C3936&iiifManifestId=https%3A%2F%2Fbiiif-template-example-3kntb3jpl-mnemoscene.vercel.app%2F3d%2Findex.jsonC3936&iiifManifestId=https%3Ahttps://uv-v4.netlify.app/%23?c=&m=&cv=&xywh=-2403%2C-197%2C7373%2C3936&iiifManifestId=https%3A%2F%2Fbiiif-template-example-3kntb3jpl-mnemoscene.vercel.app%2F3d%2Findex.jsonFhttps://uv-v4.netlify.app/%23?c=&m=&cv=&xywh=-2403%2C-197%2C7373%2C3936&iiifManifestId=https%3A%2F%2Fbiiif-template-example-3kntb3jpl-mnemoscene.vercel.app%2F3d%2Findex.jsonFbiiif-template-example-3kntb3jpl-mnemoscene.vercel.apphttps://uv-v4.netlify.app/%23?c=&m=&cv=&xywh=-2403%2C-197%2C7373%2C3936&iiifManifestId=https%3A%2F%2Fbiiif-template-example-3kntb3jpl-mnemoscene.vercel.app%2F3d%2Findex.jsonF3dhttps://uv-v4.netlify.app/%23?c=&m=&cv=&xywh=&iiifManifestId=https%3A%2F%2Fbiiif-template-example-3kntb3jpl-mnemoscene.vercel.app%2F3d%2Findex.json) already, using a manifest that looks like IIIF but is not (u)
- not officially part of IIIF yet
- exhibit uses UV under the hood and can use the 3D objects that are supported (Ed S.)


TEI: From the page [workshop](https://training.iiif.io/advanced_iiif/modules/FromThePage/)
Image location:

- V&A [Compariscope](https://vanda.github.io/iiif-features/compariscope.html?manifest=img/manifest_constable.json)
- [UCD tool](https://jbhoward-dublin.github.io/IIIF-imageManipulation/index.html?imageID=https://images.eap.bl.uk/EAP922/EAP922_1_5_54/1.jp2)
- [image registration](https://tanc-ahrc.github.io/IIIF-TNC/seminar01.html)
  v3 recipe to do overlay in [cookbook](https://iiif.io/api/cookbook/recipe/0036-composition-from-multiple-images/)

#### common errors

- can't go from an https site to an http manifest 
- CORS issue
  - headers in the image server and manifest
  - viewer won't be able to access the image without them
  - without: will work in our own website but not on others
- JSON issues
  - JSONLint
  - Validator

## One on one session

### Our project

what are we trying to do? digital storytelling
Prototyping phase: we are looking at the available

-  presentation tools
    - juncture
    - exhibit
    - storiiies
- what we could do ourselves?
    - operations that researchers do
    - go beyond a presentation tool, make it into a research tool

What we are doing (specify features of the appication)

- digital storytelling exhibition of righettino image (smooth zoom in/out, show annotations or note of explanation for the different parts of image, etc)
- installed osd and uv with base example each
- dint installed till now 
    -> canvas panel (react stuff), curation viewer (dint find proper documentation for installation), divajs
- current status 
    -> downloaded the manifest with help of oncs (able to see the image in mirador but not in uv)
- uv -> cross origin request blocked error
- going through the github repo and docs of uv to view our image, how we can add and customize interactivity
- openseadragon (we can look at the plugins and extensions and code file examples)
- how we can show or point out exact parts of image which we are going to point out and show annotations for that part (overlay ?)
- how we can add some text or annotations at the different parts of image?

### Discussion

Storytelling in IIIF is a rather crowded space
- exhibit: allows using multiple manifests, doesn't require you to make your own manifest
- storiiiies: single image → more basic
- [Cartinal](https://cartinal.leventhalmap.org/documentation/panel-truck.html) maps-related stoytelling tool
- Omeka
- [Annona](https://ncsu-libraries.github.io/annona/range/)

Do we really need to use a manifest? If OpenSeaDragon doesn't use it

Text annotations encoded in XML-TEI, can they stay in this format? Is there a real advantage to have the annotations stored inside the manifest? 
Alto to annotations [examples](https://glenrobson.github.io/iiif_stuff/alto2annotations/)


[annotorious](https://recogito.github.io/annotorious/)

image zoomers:
- openseadragon
- leaflet
- openlayers

https://glenrobson.github.io/iiif_stuff/
- aller voir le projet avec des [memes](https://glenrobson.github.io/iiif_stuff/meme_challenge/) pour le overlay

## Annotations
browser compatibility: chrome and firefox should both be fine

Workbench issue: v3 images don't work (v2 will work but the thumbnail image in the bodleian editor won't work)

How to generate the correct metadata for the overlay position? no perfect solution, work in progress

Is the size of the canvas in pixels? I can’t figure out how to compute the position for my overlay image
- standard says that it doesn't have to be pixels but it is almost always pixels
- image size is pixels
for our case: 'real’ width and height because we prepared it that way, wouldn’t usually happen
_canvas size / full image_:
width: 9645
height: 7181

_Turin forteress_
x:	3410
y:	2482
width:	1913
height:	2154


Does IIIF keep the image transparency (png)?
- mirador will request it as a jpg, and jpeg doesn't support 
- info.json → [prefered format](https://iiif.io/api/image/3.0/#55-preferred-formats) in the info.json =  png
- ask on the cantaloupe 

level0 media that is not images? audio.. architecture of the server
- no special av server → just put it as a direct link to the content with the https


[Mirador URL](https://projectmirador.org/embed/?iiif-content=https://manifests.collections.yale.edu/ycba/obj/5005) that we can refresh

[annotations Lena](https://annonatate.herokuapp.com)

## [Project demo](https://docs.google.com/presentation/d/1OZwAKY83B_jD0QYiAZq6zTvpx2wYbuEBwJn2c5fwlkE/) day

[Visual essays tool](https://visual-essays.app/)
- looks a lot like juncture

[use of IIIF](https://jhna.org/articles/jhna-2-point-0/) in [art history scholarship](https://jhna.org/articles/rubens-invention-evolution-fall-of-phaeton/)

[all maps](https://allmaps.org/)

Slack channels
- general - general discussion and announcements
- beginner - beginner questions lots of people to help
- iiif-in-the-classroom - ideas for IIIF in the classroom
- [curators_of_awesome](https://github.com/IIIF/awesome-iiif) - become a curator of awesome by helping to curate
- mirador - ask questions and see the latest developments with Mirador
- technical - ask difficult technical questions :-)

[Community Calls](https://iiif.io/community/call/)

Community groups:
- [3D](https://iiif.io/community/groups/3d)
- A/V
- Archives
- Discovery for Humans
- Manuscripts
- Maps
- Museums
- Newspapers
- Outreach

Technical Groups:
- [3D](https://iiif.io/community/groups/3d/tsg/)
- Discovery
- Maps 
- Authentication
- Content Search


Stay informed
- Join the monthly newsletter
- Join the IIIF Discuss email list



notes for my presentation
- having an image server set up by the library
  - great, but in PresentationAPI v3
  - transparency of the images (jpg vs png)
- bodleian as basis
  - editing the manifest
  - locating the overlay position
- using overlays and annotations 
- using the "pre-existing" annotations in xml 
we were thinking of IIIF as developpers - lets code, code, code. We took a major step back and had fun experimenting with available libraries and tools to familiarize ourselves with all that is available before we continue our experimental approaches