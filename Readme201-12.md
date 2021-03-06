# canvas

# Easily Create Stunning Animated Charts With CHART.JS

Charts are far better for displaying data visually than tables and have the added benefit that no one is ever going to press-gang them into use as a layout tool. They’re easier to look at and convey data quickly, but they’re not always easy to create.

1. Setting up
The first thing we need to do is download Chart.js. Copy the Chart.min.js out of the unzipped folder and into the directory you’ll be working in. Then create a new html page and import the script:
[CHART.JS](https://github.com/chartjs/Chart.js)
<img src="IMAGE/CHART.JS.jpg">

2. Drawing a line chart
A- To draw a line chart, the first thing we need to do is create a canvas element in our HTML in which Chart.js can draw our chart. So add this to the body of our HTML page:

<img src="IMAGE/CHART.JS1.jpg">

At first sight a canvas looks like the img element, with the only clear difference being that it doesn't have the src and alt attributes. Indeed, the canvas element has only two attributes, width and height. 

B-  Next, we need to write a script that will retrieve the context of the canvas, so add this to the foot of your body element:

<img src="IMAGE/CHARTS.JS3.jpg">

Inside the same script tags we need to create our data, in this instance it’s an object that contains labels for the base of our chart and datasets to describe the values on the chart. Add this immediately above the line that begins ‘var buyers=’:

<img src="IMAGE/CHARTS.JS2.jpg">

If you test your file in a browser you’ll now see a cool animated line graph.

3. Drawing a pie chart
Our line chart is complete, so let’s move on to our pie chart. First, we need the canvas element:

<img src="IMAGE/CHARTS.JS4.jpg">

Next, we need to get the context and to instantiate the chart:

<img src="IMAGE/CHARTS.JS5.jpg">

Next we need to create the data. This data is a little different to the line chart because the pie chart is simpler, we just need to supply a value and a color for each section:

<img src="IMAGE/CHARTS.JS6.jpg">

Now, immediately after the pieData we’ll add our options:

<img src="IMAGE/CHARTS.JS7.jpg">

These options do two things, first they remove the stroke from the segments, and then they animate the scale of the pie so that it zooms out from nothing.