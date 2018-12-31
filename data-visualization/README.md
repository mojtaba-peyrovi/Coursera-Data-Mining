
# Coursera Course for Data Mining:


## Data Visualization


### Week 1: The Computer and the Human

Data visualization is not just about seeing data. It's about understanding data and making decisions based on the data.


__Color coding:__ the process of deciding on colors and making decision on what color would be associated with which data.

in the example here: data-visualization.jpg   we say blue color is the faculty members who were the first choice of students, orange second and green third. By a glimpse on the chart we see that the first half alphabetical members where chosen as the first choice and the second half were picked as the last choice.

- It shows that the drop downs where student had to pick faculty members from, shouldn't be sorted by alphabetical order.

This is one of the uses of data visualization, to get the insight that we need to improve the design of the online form.


#### Types of data visualization:

- Mathematical visualization: data results from mathematics
Fractals or Julia sets are some examples of mathematical visualization. example: factal-or-julia-set.jpg
- Scientific visualization: These data come from scientific tools that measure real data based on real-world situations, or based on expensive scientific simulators.
- Information visualization: comes from more abstract sources, like relationship data. It requires some sort of processing on the abstract data to make them ready to be understood. A bit more challenging than the other types of visualization.

#### Domains of data visualization:
- medical imaging; CT scan, etc.
- Business Intelligence
- Educational visualization
- Geographic information systems

In most of data visualization tasks we use 2D graphics.

__Vector shapes vs raster shapres:__

Raster shapes are pixelated shapes, whereas vectorized ones are not working on pixel system.

__Rasterization:__
The process of converting the vector to a raster image. here is the example: rasterization.jpg

__Parabola: شلجمی__

#### Types of coordinates:

- Canvas coordinate system: we can see in the photo: canvas-coordinates.jpg
- Hierarchical coordinate system: there is a canvas within a canvas.  hierarchical-coordinate-system.jpg
- Screen coordinates: used for raster graphics.


One of the tools we can use to make vectors is making SVG (Scalable Vector Graphics)
photo: svg-canvas.jpg and svg-within-svg.jpg

We can make a path by svg. photo: svg-path.jpg  (in the photo M means move without drawing a line, and L means move with drawing a line, also d means data)

photo: svg-closed-path.JPG  in this photo Z means close the path.

__3D visualization:__ in some cases we will have to use 3D visualization.

__Photorealism:__ It describes the cues that tell our perceptual system that when it sees a two-dimensional image it sees a depiction of a 3 dimensional picture.
photo: photo-realism.jpg

__Illumination:__ it has two types.

1) Diffuse illumination: shows brighter surface when facing a light source.

2)Specular illumination: reflects light anywhere on the surface that faces the light.
photo: illumination.jpg

__Occlusion:__ We use this technique to hide some elements behind others, to convince the viewers that the photo is 3d and noto 2d.

There are other techniques for photorealism, such as perspective, or shadowing.

__Non-photorealism:__ in computer graphics most of the time we don't want to illustrate exactly like photos because it would be useless. but instead we use a non-photorealism technique. here is an example of how to illustrate human hears without showing so many aspects of the real photo.    (non-photorealism.jpg)

We can sometimes use a cartoonish illustration that shows the same message and perception from the real photo illustration. like this example: photorealism-vs-non-photorealism.jpg

For making a non-photorealistic illustration, we can use __Silhouette Curves__ that are the border between the element body and the background.

In the case of photorealism sometimes we can't see so much of the object because of lighting and beingn dark in shadow side, but we can use non-photorealism to make it lighter to be able to be seen more. like this photo: photo-vs-nonphoto-realism-lighting.jpg

here are some examples:  photo-vs-nonphoto-example-1.jpg  photo-vs-nonphoto-example-2.JPG

__How does human beings understand and respond to data visualization?__

There are 3 types of reasoning:

1) Deductive reasoning: making valid, logical conclusions based on visualized data. if A then B.
2) Inductive reasoning: if it is true for a case it will be true for all of the cases. it is called Generalization. or find missing points between two points that we extrapolate and guess their values.
3) Abductive reasoning: when we ask why? then we make a model based on the data, for example a linear regression. then we can conclude based on that. in this case we don't need to know the data for every single point. (prediction)

__Intersting:__ most of people see the red closer than the blue.


- 10% of males are colour blind. it's a good idea to add some  more information to the visualization so that color blind people could also understand it.
- pay attention to contrasts. neighboring colors should have different brightnesses so that people could better see them.
- (nice test [here](http://www.rpdms.com/satillusion/))
- use warm colors in front and cool colors in background.

There are some techniques for getting people to see some shapes bigger, or birghter, or smaller, etc. based on perceptual delusion. this section was so interesting : "[Perceiving Two Dimensions](https://www.coursera.org/learn/datavisualization/lecture/BuZbn/1-3-5-perceiving-two-dimensions)"

In order to use 3d visualization, we tend to use them as minimal as possible, instead using 2d but onyl if it's necessary we will use 3d.


### Week 2: Visualization of Numerical Data

Data visualization has 3 layers:
1) **Data Layer:** obtaining and collecting data, and making sure the data is in proper format, and also having some aggregation and analysis on it.
2) **Mappling Layer:** associating the appropriate geometry with corresponding data channels, and analysis.
3) **Graphics Layer:** Conversion of geometries into graphical image decorations in a displayable way.

__Data Types:__ There are different types of data that we can see in the photo called: data-types.jpg


Ordered: means you can be 1 is greater than 2 or unodrdered means circle can't be greater that rectangle.

there are 3 important types of data 1) Nominal   2) ordered 3) quantitative

__Data Mapping:__ when we mapp data we figure out how to convert data into some primitive graphics that we can display and it depends on our understanding of data and the graphics.

let's learn how to mapp quantitative data:  photo: mapping-quantitative-values-1.jpg

__Ordinal values:__ categorical data we don't know how much they are greater that each other but we know some of them are greater that the others. like shirt sizes.


__Nominal values:__ categorical data we  know how much they are greater that each other but we know some of them are greater that the others.
(photo: mapping-quantitative-ordinal-nominal.jpg)

**Bar Charts:** in bar charts we have discrete data as X and quantitative data as Y.

**Line Charts:** It's useful to have to for showing quantitative values for both X and Y. X better to be independent and Y dependent.

**Scatter plot:** It can be used when we want to show quantitative, independent data for bot X,Y.

**Gantt Chart:** looks like horizontal bar charts but its use is mostly to show consequent data and showing progress. It is also independent-independent. the X is mostly used for time.

** Tables:** used for discrete per discrete view. when we have X and Y independent.


### Week 3: Visualization of Non-Numerical Data

The aim is to visualize data when we don't have specific coordinates associated with the data.


When we don't have coordinates for data, we mostly look for RELATIONSHIP between data rather than the data items themselves.

A graph consists of :

```
1) nodes
2) edges
```

__Complete Graph or Clique:__

When we have all the nodes connected to each other. (photo: clique.jpg)


__Isomorphic graphs:__ When we have identical graphs, which are laid out a bit differently. (photo: isomorphic.jpg)

__Planer graph:__ When the graph is laid out in a way that none of the edges cross each other. in isomorphic photo, the right graph is isomorphic.

__Face:__ it's a region sided by different edges.

IF we see the whole image of two graphs as one graph, we can say we have a graph of two __CONNECTED COMPONENTS.__ but they are disconnected.

There are different types of graphs we can see in the photo: (graph-types.jpg)

__Degree of a node:__ The number of edges connected to the node.

__in-degree vs out-degree nodes:__ in deirected graphs the number of edges coming into the node are called in-degree and the number of edges getting out of the degree will br out-degree.

__Adjacency matrix:__ it is a square matrix, showing the relationship between all nodes. of course the degree of the matrix equals the number of nodes.

##### IMPORTANT: If the graph is non-directed, the adjacency matrix would be symmetric, whereas directed graphs have asymmetric adj. matrices.

(photo: adjacency-matrix.jpg)


__planer vs non-planer graphs:__ As mentioned before, planer graphs are made in a way which none of the edges cross each other. non-planer graphs don't have the advantage. SO, the act of adding the planer graph will be called __"Planer Embedding"__.

(photo: planer-embedding.jpg)


#### Tutte method:
It is a method of drawing planer graphs. the photo shows an example: (photo: tutte.jpg)

IN order to do this we will have to define a matrix called __"Laplacian Matrix- /lap-la-shen"__. this matrix's degree equals the number of nodes. so in case of the cube, the degree would be 8.

each node has 3 edges in this case, so for each node to the node next to it, the value in the matrix would be 0 if there is no edge, and 1/3 if there is an edge.  photo( laplacian.jpg)  

Then we need to do two steps:

```
1- for the nodes we already assigned (we said first we assign nodes 1,2,3,4) we make them all the row zero.
2- then we calculate a new matrix that we call it A=I-L  where I is identity matrix (all values zero excpet the diagonal values which would be ones)
```

(photo: matrix-a.jpg)

Now in order to find the X value for the rest of the graph, we will make a linear system and we solve an equation. It will return us the x values of the missing point. we will do the same thing for y values.

(photo: laplacian-x-values.jpg and laplacian-y-values.jpg)

After extracing these equations, we can vectorize them like this:  photo: vectorized-laplacian-equations.jpg

And finally we solve the equation and we get the following shape: laplacian-solved.jpg


#### Conclusion from Tutt method:
In order to make a graph planer, we don't need to necessarily follow the whole matrix representation and deal with all difficult and time consuming process. Instead, we can easily do this:

```
Nail donwn some of the nodes, then for the rest of the nodes, calculate their position in the way that for each node, the position would be the average of its neighbors.
````

#### GEM Force Directed Layout:
Another way to make planer graphs, is called GEM.
we can see an example here:

(photo: GEM.jpg)


__Centralities:__ There is a rule that says the nodes with higher degrees will be positioned around the center, whereas, the ones with lower degrees will position toward the periphery(حاشیه).

__Isolation Metric:__ sum of distance between the given node to all other nodes.

__Distance:__ The distance between two nods, will be the count of edges making the shortest route to the second node.

(photo: centralities.jpg)

__Betweenness centrality:__ It is a metric that returns all shortest paths between any two nodes that pass through the given node.

In order to simplify graphs, we can remove the edges that have few shortest paths going through them. the result would be a graphs that has as many edges and the nodes.
we can see the sample here:  photo: graph-simplification.jpg

#### Edge Bundles technique:

In this way, we put all the nodes in a ring. Then we draw the edges between the nodes, inside the ring.

This example show this method. The shape on the left side, shows the emails between 132 employees on a month.

(photo: edge-bundle.jpg)

In order to group some the edges together to form __Wire Bundles__, we need to find communities among nodes and form clusters of nodes called __Communities__. In order to have communities, we will isolate nodes which have similar edges behavior and they make clusters.

(photo: community-discovery.jpg)

Then inside the graph, there will be __Community Nodes__ that are not part of the original graph, but they show merging of the nodes in each community.

Example:

photo: edge-bundle-ezample-1.jpg

edge-bundle-ezample-2.JPG

__Filtering Edge Bundle:__ By using edge bundles, we can filter the relationships between different nodes, and it give very good information on what's going on in the dataset.

(photo: filtering-edge-bundle.jpg)


### Tree Map:

Tree map is a very useful method to show hierarchical relationships.

photo: tree-map.jpg & tree-example-1.jpg  & tree-example-2.JPG


__Here is how we draw and treemap based on a tree graph:__

photo: trremap-layout.jpg

Also, this photo shows how we calculate the contribution ratio of each node:

photo: treemap-calculation.jpg

Tree maps are good to show hierarchical relationships, but not great for ordinal relationships.
### Principal Component Analysis:
We had this in Machine Learning with Coursera(reducing the features of the dataset), but according to the lecturer here, there are packages that already do it for us and we don't have to know the details in order to be able to use this technique.
In order to do this technique we need to take the date and subtract the mean from them. it will give us the __Covariance Matrix.__
(photo:covariance=matrix.jpg )
    - Covariance matrix is a symmetric matrix.
Principal Component analysis, keeps the data that keeps the most effect in the variance and gets rid of the ones with least influence.
(photo:princile-component-analysis.jpg)

__Multidimensional Scaling:__
It is another way of dimensionality reduction method.
__Metric MDS:__ Multidimensional Scaling: when you try to preserve the distance between data points.
(photo:MDS.jpg)

##### Packing:
sometimes we want to have a visualization that shows the data points but not just as points. we want them as different shapes.

One of the examples is a map called __Word Cloud__. here is a good website that makes this: [wrodle.net](http://www.wordle.net/)

###### example:
(photo: word-cloud.jpg) The most used words are shown larger than the others.

When we have circles as data points we can have the size of the points relevant to the quantity. this example shows the population of each country: packing-example.jpg.

##### Cartogram:
there is an example of it here: cartogram.jpg

How to make cartograms?

We scale each  area as much as their density. then the corners of the areas with start disconnecting. we need to calculate the new corners by finding the average of all points that make the intersection and find new corners.
here is the photo: creating-cartogram.jpg

##### Choropleth:

This type is so popular and we can see them everywhere. It shows the density by color saturation.

(photo: choropleth.jpg)
