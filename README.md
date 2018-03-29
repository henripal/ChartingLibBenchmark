# Benchmarking JS charting libraries.

Common task: start with 1000 points on graph, add 1 point every .1 seconds. You can run all these yourself by navigating to the appropriate subdirectory, then serving `index.html`.

Big disclaimer: benchmarking is a difficult exercise, and I probably did *not* follow best practices for performance for all the examples. Also, my performance assessment could be more rigorous than looking at my browser's task manager tab. Feel free to improve on these points!

Small disclaimer: for a charting library benchmark, it could be said that these data points would probably be better seen on a graph :) 

## Highcharts:

Goes to 100pct CPU use immediately. 200MB RAM after a couple extra hundred points.

## Dygraphs:

Abt 50pct CPU use. Stays below 100MB ram even after 2000 points. Much better!

## Taucharts:

110 pct CPU use immediately. 400 MB RAM use after a couple extra points.

## Chart.js:

100pct CPU use immediately. 100MB ram consumption, relatively stable.

## C3.js:

100pct CPU use immediately, 200MB ram consumption, reaches 300MB after a couple extra hundred points.

## Google Charts:

100pct CPU use immediately. 100MB initial ram consumption, goes to 200MB after 500 extra points.

## Rickshaw:

100pct CPU use immediately. 100MB ram consumption, relatively stable even after 1000 extra points.