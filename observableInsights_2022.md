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

