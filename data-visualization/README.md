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
