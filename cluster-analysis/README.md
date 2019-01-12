# Data Mining - Cluster Analysis:


## Week 1


### lesson 1, Cluster Analysis introduction:

Cluster analysis, or clustering, or Data Segmentation, is grouping data objects into different groups based on some similarities.

- it is __unsupervised__ because there is no predefined classes.

- it can be used as a stand alone project to understand the data better, or be used as a pre-processing step before doing another step like classification, etc.
- it is one of the popular tools to find __Outliers__. and will be a good tool for __Anomaly Detection__.
- Also can be used in data summerization, reduction, and compression. like vector quantization in image processing.
- Also can be used for __recommendation systems and collaborative filtering.__
- Used for trend detection.
- Used for MUltimedia data analysis, biological data analysis, and social network analysis.

##### What are some challenges?

- people don't know whether to use single level partitioning or hierarchical multi-level partitioning. most of the time the second method works better.
- Whether to have exclusive or no-exclusive segmentations. __Exclusive__ means one sample can only belong to one cluster, but __Non-Exclusive__ means they can belong to more than one.
- What would be the similarity metrics? distance based (Eucildean, road network, vector) or connectivity based (density, contiguity).
- Whether using __Full-space__(when we have low dimensional data) or __Sub-space__ (for higher dimensional data) spacing.
- __Quality:__ how to deal with noisy data? How to deal with different data types? deal with arbitrary shapes?
- __Scalability:__ dealing with high dimensional data. clustering all the data instead of one sample. Or how to deal with incremental and stream data and insensitivity to the output order.
- __Constraint-based clustering?__ sometimes users have their own preferences or constraints.
- finally, interpretability and usefulness of data.

##### Clustering different data types:
__Numerical:__ the most common.

__Categorical data:__ Discrete data like sex, race, zip-code.

__Text data:__ so popular on soclal media, web, or social networks analysis.

__Multimedia data:__ audio, video, image.

(photo: clustring-data-types.jpg)

__Time series data:__ data with equal intervals, such as time.

__Sequence data:__ weblogs, biological sequences, etc.

__Stream data:__ data that flow, means come and go. We can use Micro-clustering for these types of data.

(photo: clustring-data-types-2.jpg) and ((photo: clustring-data-types-3.jpg)
