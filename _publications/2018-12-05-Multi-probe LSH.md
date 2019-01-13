---
title: "Image Color Search Engine"
collection: publications
permalink: /projects/lsh
excerpt: 'Implementation of Multi-probe LSH, an improved algorithm LSH for high-dimensional as an approach to Nearest Neighbor Problem.'
date: 2018-12-05
---

Partner: [Anna Buchman](https://github.com/abuchman14)

## Abstract
Multi-Probe Locality Sensitive Hashing (LSH) is used to resolve similarity search in high-dimensional data. The basic concept of LSH is to reduce dimensionality while reserving similarity to a certain extent [2]. Previously existing LSH algorithms required heavy amounts of either time or space.  Multi-Probe LSH was able to achieve high accuracy in finding similar objects to a query, while being both time and space efficient. Multi-Probe LSH was first introduced in a paper in 2007--in their experiment, 2GB memory was able to hold a Multi-Probe LSH index for 60 million image data objects [3].

## Implementation
We first implemented the algorithm, developing a model that can realize image similarity search. The source for our image data is in References: [1]. This source has more than 10000000 images--we used 502521 images and the size of 15 generated hash tables only around 428.5MB, and our database is 426.3MB. The data also include strings of URLs. The size can be smaller if we use other index to handle URL. We experimented with the same process in the paper: First, we converted the images into histograms. When querying, we used  Euclidean distances to find the top k candidates. To determine accuracy, we found the true k most-similar images by computing the Euclidean square distances from the query to every other image in the set. Next, we implemented the Multi-Probe LSH method with different values of parameters and measured their accuracy and runtime.

## Results
![lsh_image1](https://chien-wei.github.io/files/lsh/i1.png)  
Example 1: A common street photo with nice blue sky.

![lsh_image2](https://chien-wei.github.io/files/lsh/i2.png)  
Example 2: A gray scale photo.

![lsh_image3](https://chien-wei.github.io/files/lsh/i3.png)  
Example 3: A taxi photo that has many yellow pixels.

![lsh_image4](https://chien-wei.github.io/files/lsh/i4.png)  
Example 4: A photo that has mostly green with other colors.

## Demo
The demo web application is under construction... Here is a screenshot for it:
![demo_temp](https://chien-wei.github.io/files/lsh/temp.png)  


## Reference
[1] Open Images Dataset.[https://github.com/cvdfoundation/open-images-dataset#download-full-dataset-with-google-storage-transfer](https://github.com/cvdfoundation/open-images-dataset#download-full-dataset-with-google-storage-transfer).  
[2] Gionis, A., Indyk, P., and Motwani, R. Similarity search in high dimensions via hashing. In Proceedings of the 25th International Conference on Very Large Data Bases (San Francisco, CA, USA, 1999), VLDB ’99, Morgan Kaufmann Publishers Inc., pp. 518–529.  
[3] Lv, Q., Josephson, W., Wang, Z., Charikar, M., and Li, K. Multi-probe lsh: Efficient indexing for high-dimensional similarity search. In Proceedings of the 33rd International Conference on Very Large Data Bases (2007), VLDB ’07, VLDB Endowment, pp. 950–961