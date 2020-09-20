Chart.js API.


![chart](https://encrypted-tbn0.gstatic.com/images?q=tbn%3AANd9GcQ6raUqFkZK8Tl0XvM8QEtl6xwKR77gH2xrUA&usqp=CAU)


Charts are far better for displaying data visually than tables and have the added benefit that no one is ever going to press-gang them into use as a layout tool. They’re easier to look at and convey data quickly, but they’re not always easy to create.

A great way to get started with charts is with Chart.js, a JavaScript plugin that uses HTML5’s canvas element to draw the graph onto the page. It’s a well documented plugin that makes using all kinds of bar charts, line charts, pie charts and more, incredibly easy.

To see how to use chart.js we’re going to create a set of 3 graphs; one will show the number of buyers a fictional product has over the course of 6 months, this will be a line chart; the second will show which countries the customers come from, this will be the pie chart; finally we’ll use a bar chart to show profit over the period.

![ch](https://camo.githubusercontent.com/ca884126d1d74829f36c8fa2e6947d8a411aed1f/68747470733a2f2f7777772e63686172746a732e6f72672f6d656469612f6c6f676f2d7469746c652e737667)

Drawing shapes with canvas
+ The grid
 Normally 1 unit in the grid corresponds to 1 pixel on the canvas.
 The origin of this grid is positioned in the top left corner at coordinate (0,0). All elements are placed relative to this origin
 So the position of the top left corner of the blue square becomes x pixels from the left and y pixels from the top, at coordinate (x,y). Later in this tutorial we'll see how we can translate the origin to a different position, rotate the grid and even scale it, but for now we'll stick to the default.
 
 + Drawing rectangles
Unlike SVG, ``<canvas> ``only supports two primitive shapes: rectangles and paths (lists of points connected by lines). All other shapes must be created by combining one or more paths. Luckily, we have an assortment of path drawing functions which make it possible to compose very complex shapes.

 **There are three functions that draw rectangles on the canvas:**

+ fillRect(x, y, width, height)
Draws a filled rectangle.
+ strokeRect(x, y, width, height)
Draws a rectangular outline.
+ clearRect(x, y, width, height)
Clears the specified rectangular area, making it fully transparent.
Each of these three functions takes the same parameters. x and y specify the position on the canvas (relative to the origin) of the top-left corner of the rectangle. width and height provide the rectangle's size.

Below is the draw() function from the previous page, but now it is making use of these three functions...


+ Drawing paths
Now let's look at paths. A path is a list of points, connected by segments of lines that can be of different shapes, curved or not, of different width and of different color. A path, or even a subpath, can be closed. To make shapes using paths, we take some extra steps:

1. First, you create the path.
2. Then you use drawing commands to draw into the path.
Once the path has been created, you can stroke or fill the path to render it.
Here are the functions used to perform these steps:

+ beginPath()
Creates a new path. Once created, future drawing commands are directed into the path and used to build the path up.
Path methods
Methods to set different paths for objects.
+ closePath()
Adds a straight line to the path, going to the start of the current sub-path.
+ stroke()
Draws the shape by stroking its outline.
+ fill()
Draws a solid shape by filling the path's content area.

![line](https://apexcharts.com/wp-content/uploads/2018/01/basic-line-chart.svg)

+ Arcs
To draw arcs or circles, we use the arc() or arcTo() methods.

arc(x, y, radius, startAngle, endAngle, anticlockwise)
Draws an arc which is centered at (x, y) position with radius r starting at startAngle and ending at endAngle going in the given direction indicated by anticlockwise (defaulting to clockwise).
arcTo(x1, y1, x2, y2, radius)
Draws an arc with the given control points and radius, connected to the previous point by a straight line.
![arch](https://encrypted-tbn0.gstatic.com/images?q=tbn%3AANd9GcTnrJ_7WGY_8Ep0jFB7VLu5MVFN0_DlmvbstA&usqp=CAU)
