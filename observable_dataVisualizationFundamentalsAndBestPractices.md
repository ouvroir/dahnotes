# Data Visualization Fundamentals and Best Practices 

Robert Kosara: data visualization as a research, teacher and practinionner

[eventbrite](https://www.eventbrite.ca/e/course-data-visualization-fundamentals-and-best-practices-tickets-558920144197?keep_tld=1)

[course description and notebook set](https://observablehq.com/@observablehq/datavizcourse)

## Introduction

march 7th, [youtube](https://www.youtube.com/watch?v=WJ1c54Ab-o8)

### Basic Chart Types

#### Scatterplots

- mapping each object at position on x and y 
- range = axis
- general view / overall shape: relationship/correlations in the dataset
- things that stick out : unusual values (function differently in average)

plot `title` => tooltip!

anscombe dataset different views (to check again)

#### Bar chart

- sort

plot `sort: {x: "y", reverse: "true", limit: 8}`

- compare values

- bar charts vs tables

  - tables are great for precise data
  - visualisation is for structure and patterns. precision is not usually what is wanted
  - If you need precise numbers, either use a table or label/tooltip

- curtting off the x axis to remove 0-300 and keep only 300 to 600

  - theoretically one can see the differences better
  - however, we look at bars as length
  - when you cut off the axis, you don't realise the biais
  - misguiding: people might not check the 
  - the point of the chart is to show the numbers to understand them, and intuitively understand the difference, which you can't do if you need to remap the values

  > cardinal sin of data visualisation

#### Pie chart

- too similar to bar charts, people mistakenly use pie or bar charts for the wrong reason
- distribution of part to a whole not good at comparison between sizes
- categorical axis: color
- number: length on the arc
- very hard to guess the differences between two areas
- 
- donut chart (whole in the center)
  - often considered a bad idea
  - will develop next time

#### Line chart

- standard line chart: only one possible value for the position on the x axis
- assume that there is a continuity: draw lines between the positions
- common rule (though not proven by research): rough overall 45° "banking on"

`Plot.lineY`

### Questions

- radar charts: very dependent on the order of the radial axis  (especially the area can change drastically depending on position)→ rather poor chart 