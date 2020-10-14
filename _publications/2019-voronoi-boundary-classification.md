---
title: "Voronoi Boundary Classification: A High-Dimensional Geometric Approach via Weighted Monte Carlo Integration"
collection: publications
permalink: /publication/2019-voronoi-boundary-classification
excerpt: ''
date: 2019-06-10
venue: 'Proceedings of the 36th International Conference on Machine Learning'
paperurl: 'http://proceedings.mlr.press/v97/polianskii19a.html'
citation: 'Polianskii, Vladislav, and Florian T. Pokorny. "Voronoi Boundary Classification: A High-Dimensional Geometric Approach via Weighted Monte Carlo Integration." International Conference on Machine Learning. 2019.'
thumbnail: /images/thumbnails/2019-icml.png
authors: 'Polianskii, Vladislav, and Florian T. Pokorny'
year: 2019
---
Voronoi cell decompositions provide a classical avenue to classification. Typical approaches however only utilize point-wise cell-membership information by means of nearest neighbor queries and do not utilize further geometric information about Voronoi cells since the computation of Voronoi diagrams is prohibitively expensive in high dimensions. We propose a Monte-Carlo integration based approach that instead computes a weighted integral over the boundaries of Voronoi cells, thus incorporating additional information about the Voronoi cell structure. We demonstrate the scalability of our approach in up to 3072 dimensional spaces and analyze convergence based on the number of Monte Carlo samples and choice of weight functions. Experiments comparing our approach to Nearest Neighbors, SVM and Random Forests indicate that while our approach performs similarly to Random Forests for large data sizes, the algorithm exhibits non-trivial data-dependent performance characteristics for smaller datasets and can be analyzed in terms of a geometric confidence measure, thus adding to the repertoire of geometric approaches to classification while having the benefit of not requiring any model changes or retraining as new training samples or classes are added.

[Download paper here](http://proceedings.mlr.press/v97/polianskii19a.html)
