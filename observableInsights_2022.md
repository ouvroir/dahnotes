# Observable *Insight*

Oct 26 - Oct 27, 2022

[program and info](https://hopin.com/events/observable-insight/registration)

contact team [support@observablehq.com](mailto:support@observablehq.com)

[Become an Ambassador](https://observablehq.com/@observablehq/become-an-observable-ambassador)

## Day 1 - 26 octobre

### Welcome

Melody Meckfessel, CEO and Co-Founder, Observable

Bring data, context and logic into one place to gain insight into data

### An API to Track Press Freedom

Harris Lapiroff, Principal Web Developer, Freedom of the Press Foundation (FPF)

Paul Buffa, Data Visualization Developer, Observable

> The U.S. Press Freedom Tracker records incidents include arrests, border stops, physical assaults, subpoenas, equipment damage, and more. Tracker data is made available through an API that can be used to track trends, aggregate incidents related to specific events, and more. We'll show off how the API is already used to power interactive data visualizations and give an overview of how anyone can access and use the data.This talk will include code examples, but is open to any skill level.

#### US press Freedom Tracker

2017 launch of the US Press Freedom Tracker

Systematically document press freedom incidents: central repository

11 categories of incidents

#### API for Press Freedom

[API](https://pressfreedomtracker.us/api/edge/)

Django REST interface to interact with API

#### Case Study: BLM Protests 2020

Timeline of Incidents, Highlight by category

Cumulative incidents at various cities

#### Other observable notebooks

Years of tracking press freedom

Press freedom Tracker data integrity

#### Notebook demo

Paul Buffa 

uses SQL: 

- DuckDBClient 
- SQL cell and write queries

#### Questions

What do the different colors on the beeswarm chart represent? Also do they cluster in some particular way? I.e. most common at the center?

- represent the categories of each incident
- incidents that have multiple categories: some charts
- do not cluster in any particular way
- beeswarm with x axis for exact day? it would explode at may 2020

...

### Animating Any Viz (SVG and Canvas) with GSAP

Dea Bankova, Graphics Journalist, Thomson Reuters

Maxene Graze, Independent Data Visualization Engineer

> Starting with an overview of how to create awesome animations in GSAP with just a few lines of code, we will delve into applications of GSAP in animating SVG and Canvas. This will be a hands-on workshop in Observable and we will also go over some “gotchas” - like how Observable’s D3’s select might trip you up. We will aim to make this workshop accessible for people with no prior GSAP experience, but ideally you will have some D3 and Canvas skills and an interest in taking them to the next level!

[GSAP](https://greensock.com/gsap/): Professional-grade JavaScript animation for the modern web

canvas vs svg:

- Canvas heaps faster. SVG starts to stall with 2000+ points
- The core difference between SVG and canvas is that SVG is a vector API, and canvas is a raster API.
- SVG's primitives are lines and circles and etc, and you can manipulation them as their geometric ideas. Canvas's primitive is a pixel, so when you draw a circle, it just ends up being a bunch of colored pixels with no group identity.
- Canvas is like an immediate mode UI, you draw the whole view every from, while SVG is more like a UI framework with an object model for the UI

Use observable prototyping especially with inputs. When it gets more advanced, use a framework

### Navigating the Data Science Career Confusion

Gabriela de Queiroz, Principal Cloud Advocate, Microsoft

> Data Science careers are still in high demand, with many job opportunities and attractive salaries. However, reading through the job descriptions can be overwhelming. They are ambiguously defined and can vary greatly from company to company. In this presentation, I will talk about data science and walk you through the different roles a Data Scientist can take and the important skills for a successful career.This talk is suitable for all, no matter how early or late you are in your career.



Josh Wills (may 3, 2012)

Data scientist: Person who is better at statistics than any other software engineer and person who is better at software engineering than any statistician

Before moving to the industry, was in academia for several years 

- Industry timing is so challenging: right now, today, by friday. Very short timeframe. So much time in academia
- it didn't need to be perfect, it needed to be good enough, or better than it was

### Adopting Observable Panel

- Melody Meckfessel, CEO and Co-Founder, Observable
- Ananya Roy, User Success, Observable
- Robert Harris, Data Visualization Engineer, Stitch Fix, Inc.
- Paulino Oliveira, CEO & Founder, Belo
- Chad Steed, Distinguished Research Staff, Oak Ridge National Laboratory

exposing what you do, smoother than jupyter (hard to share with non-data scientists, executives etc)

notebooks that combine documentation and tooling for data scientists

### Building A Creative Career With Data with Shirley Wu

Shirley Wu, Independent Creator of Data Visualizations

> In this fireside chat with Shirley Wu and Wayne Sutton, they'll cover lessons learned from Shirley's award-winning career as a creative developer, author, and product designer. Shirley was also one of Observable's first Ambassadors. They'll also cover industry trends and what's the future of Data Visualization.

creative career with data



### Observable Roadmap

Melody Meckfessel, CEO and Co-Founder, Observable

3 product offerings

- free tier individual
- teams : subscription based products to work in organisation in private environment and workspaces
- entreprise: onboarding, training, tutorials, additional services and features

create, maintain and evolve in open-source: plot, d3, collab 4with vega..

### How We Work with Observable *at* Observable

- Allison Horst, Data Scientist Advocate, Observable
- Michael Freeman, Data Visualization Developer, Observable
- Paul Buffa, Data Visualization Developer, Observable
- Visnu Pitiyanuvath, Engineer, Observable
- Amanda Waite, Engineer, Observable

#### Data wrangling with arqquero

Mike, former Prof at U Washington

[observablehq.com/@demoteam/wrangling-at-observable](https://observablehq.com/@demoteam/wrangling-at-observable)

- arquero aq 
- .select(aq.not("shitty column"))
- .fold() <!--pivot-->

tinytools : import wrangler for visual composition of requests

#### Database 

Paul Buffa, db dev, product education team

[observablehq.com/@observablehq/pauls-observable-tips-tricks](https://observablehq.com/@observablehq/pauls-observable-tips-tricks)

- duck DB, framework for databases in browsers
- CSV with Parquet
- set up inputs to help people explore data content (use submit: true to only run the query when the submit is clicked)
- d3 Goup with dropdowns
- bespoke tooltips
- links with plot 
- annotations with plot with d3.bisect

#### Monitoring what's happening with Observable

Amanda Waite, head of engineering, VPoltrack art

using observable as dash and analysing a problem

- example service: create thumbnail from notebook 
- thumbnailer dashboard demo
- barcharting your errors!

>  You should optimize the things you care about deeply

#### How to cheat at life with JavaScript, computer vision and augmneted reality

Visnu, engineer, working with Paul on data warehouse

https://observablehq.com/@visnup/cheat

How to cheat at life with JavaScript, computer vision and augmetted reality, JSConf Hawaiî, feb 2019

- set
- wordle

games, cheat by coding

## Day 2 - Oct 27

### Welcome

Melody Meckfessel

### Observable Can do That? 

Mike Bostock, CTO and Co-Founder, Observable

> A list of techniques to show what's possible with Observable.

### The Happiest Notebooks on Earth

https://apreshill.github.io/happiest-notebooks-on-earth

Alison Hill, Director of Knowledge, Voltron Data

> Notebooks hold a special place in every data scientist's heart. They may treasure every moment creating their own, or commenting on others' notebooks. Or they may sincerely and truly hate notebooks. But notebooks are useful. How could we "imagineer" better notebooks? I’ve made and read hundreds of notebooks in the past decade. In this talk, I'll share key principles for developing happier notebooks – ones that are more fun to write, more fun to read, and more fun as an onramp to the next ride.

«I don't like notebooks», Joel Grus @joelgrus

Imagineers: creative team of artists and engineer

utilidors

- config settings in YAML
- outsource a script or document
- reuse code chunks in different places
- conditional evaluation of code

multisensory experience & smellitizer

- *useful* headings
- navigation TOC
- description of data
- logical order



### Waterlines

[observablehq.com/@oliviafvane/i-drawing-water-in-old-maps?collection=@oliviafvane/watermarks](https://observablehq.com/@oliviafvane/i-drawing-water-in-old-maps?collection=@oliviafvane/watermarks)

Olivia Vane, Interactive Data Journalist, The Economist

> Across a collection of 4 Observable notebooks, Olivia has explored how to draw and animate 'waterlines'—an old technique for showing water in maps—in JavaScript. This talk will present the project, spanning design, history, coding, and maths. Olivia will share lessons and reflections around the power of images, connecting to historical examples and writing in notebooks.

'[Dive into Color](https://oliviavane.co.uk/dive-into-color)' [Cooper Hewitt Smithsonian Design Museum, New York City](https://www.cooperhewitt.org/)

can you draw waterlines with code and add them to interactive maps online?

- get inspired by history
- don't forget about the power of aesthetics
- more computational essays (explore, explain, live code, images, input controls...)



Wow, beautiful custom HTML. View of thumbnails and details of maps makes me wonder: is there any IIIF integration with Observable?



### Build an Advanced Report from Simple Pieces

Ian Johnson, Data Visualization Developer, Observable

> In this workshop we will build an e-commerce dashboard using real data using open source components and libraries like Observable Plot, Observable Inputs and D3.jsWe will start with a simple SQL query, make it more advanced and then layer interactivity and visualization. In the end we will have something like [this report](https://observablehq.com/@observablehq/which-items-are-purchased-together).



### Eurovision Results of Spanish Artists, Composers, and Lyricists by Gender

https://observablehq.com/@irenedelatorre/eurovision-data-analysis-with-plot

Irene de la Torre Arenas, Visualization Lead, UCB

> This project studies if the Spanish participation in Eurovision has been a fair representation of its society in terms of gender. It takes a special focus on the team members who, although invisible to the general audience, shape the messages that reach them: lyricists and composers.This session will show how this project was produced: from using Plot.js to make quick sketches to using Observable Cells to assemble the final website.No programming expertise is needed.

### Five Thousand Years of Graphics

tophtucker.com/classic-research

Toph Tucker, Software Developer, Observable

> When you look at a menu of the kinds of chart you could make, can you guess which came first? A sprint through a hundred milestones in visualization research, from cuneiform to the computer.

#### 1. Signs, Measures, and Maps

2700 BC - 1644

Quipu, Andes

#### 2. Dawn of the Abstract Plane

1644 - 1886

earliest recognizably modern charts

Marshall Islands stick charts (documented by a missionnary): patterns of ocean swells as part of a vector field

Ammassalik wooden maps of greenland coastline (dated by colonial documentation, no inuit date)

#### 3. Expansion of Science into Statistics, Psychology, and Eugenics

1886 - 1959

Aggregations, quantifications of people, and the reflexive quantitative study of the effectiveness of quantitative visualisation

History is troublingly linked to eugenics

artists: Kandinsky, Man Ray, Picasso (connection between more abstract visualization & more abstract art).

​     

#### 4. The Computer I

1959 - 2000

Mechanical ways of seeing

PIA14032 Jet Propulsion Laboratory   (coloring the images)



#### 5. The Computer II

2000 - ...

new dawn of the abstract (dynamic) place on the personal, networked, mobile computer, with graphics as both art and interface

2007 Jeffrey Heer, George Robertson        Animated Transitions in Statistical Data Graphics

2011: D3

2016 Archie Tse: fewer interactives at NYT: readers just want to scroll

materials realities of each time inform the abstract visualisations

tophtucker.com/classic-research

scrollytelling

There is a "visibility" promise available in Observable that fires when the  cell is visible. For more nuanced scrolly telling I think you'd need to  use the intersection observer browser API

Stumbled on this data physicalization timeline gallery, seems like a good complementary read: [dataphys.org/list/gallery/](http://dataphys.org/list/gallery/) :)

### Observable in the University Classroom and Research Lab

David Kirkby, Physics & Astronomy Professor, UC Irvine

> This session will provide an overview of how I use Observable in my teaching and research at the University of California, Irvine, with sample notebooks and web pages. It will help other academics understand the benefits of the platform, and give examples of engaging students and research collaborators without Observable or JavaScript experience.

> If you want to learn more about the Observable EDU programs email us at [support@observablehq.com](mailto:support@observablehq.com)

quilt design 

largely exposing observable to people who aren't developers 



---



### Making It Personal: Visualizing the Current State of Access to Assisted Reproductive Techniques in Europe with Observable

Carmen Torrecillas, Data Visualization, Civio

> A case study in how to convey and personalize complex data in a way that audiences can process and engage with at a glance. This session is open to anyone interested in the creative process of data visualization. We will cover workflow topics such as importing several Observable notebooks into one final piece and handling the internationalization process at the end of the project. Check out this [article ](https://civio.es/medicamentalia/2021/11/02/ART-EU-access/)on Civio.



### Observable in Higher Education: Institutional Research Use Cases

Sara Quigley, Senior Data Analyst UC Berkeley

> This session is intended for data analysts working in decentralized settings (such as a large research university) with private data (such a FERPA-protected data) in a few contexts such as ad hoc analysis, data wrangling, and building and sharing dashboards with non-technical people.  We'll walk through examples of securely loading data into Observable,  data reshaping with libraries like Arquero and iteratively building dashboards with Observable Plot and sharing them using the Teams feature.



### Show me another: How to start investigating criminal justice (and other things)

David Eads, Data Editor, The Marshall Project

> Learn how The Marshall Project, a nonprofit news organization that covers the US criminal justice system,contends with messy and incomplete data. Observable notebooks and Hasura APIs power the internal tools that help us sample cases to find reporting leads and review our stories.And we'll show how those internal tools become publication-ready products. This session is for all skill levels.





### Student Data Jam Recap

Learn about Observable’s Data Jam, one of our education programs, and hear from the winning student team from our most recent Jam - Koi Pond!
