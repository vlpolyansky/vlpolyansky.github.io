---
layout: archive
title: "Master thesis proposals"
permalink: /teaching/
author_profile: true
---

## Geometric analysis and exploration of neural network expressivity
{: #linear-regions }
**Last updated:** 4 November 2020

An overall success of deep neural networks in the recent decade has been addressed many times and explained by a notion of their high expressivity. Indeed, having large number of layers in a network contributes to the highest complexity of a function that can be learned by the network. Nevertheless, this potential does not ever seem to be utilized on practice. Moreover, as shown in {% cite NIPS2014_5484 -f teaching %}, shallow neural networks can be trained to have similar performance as of deep networks.

One measure of neural network expressivity can be defined as the number of different activation patterns that occur in the network, where an activation pattern represents the behavior of all non-linearities that occur for a given input. Such measure intuitively represents the complexity of input space geometry learned by the network. Recently, it has been shown by {% cite hanin2019deep -f teaching %} that the *expected* deep network expressivity in this sense is equivalent to one of a shallow network with the same number of neurons, and is independent of the number of layers.

In this master project, we will focus our attention on activation patterns of neural networks, and their corresponding regions in the input space. We propose three main directions to choose from for the project.

1. *Statistical exploration.* In this direction, the main task would be to perform experiments to propose and confirm or reject hypotheses about the regional structure of a network. Questions that we may consider include an analysis of a region distribution for classification and regression tasks, correlations between the distribution and relation of such distribution to the decision boundary. Furthermore, the study could be extended by considering data-driven network initializations for classification or representation learning, and contrast them to standard random weight initialization schemes.

1. *Boundary traversal.* The core part of this direction would include an adaptation of a graph traversal methodology from our recent publication{% cite polianskii2020voronoi -f teaching %} to the domain of activation regions. Such applications would bring us to a novel algorithm to obtain the regions which might be more computationally efficient than other existing methods. This methodology would also allow us to study the decision boundary of a given classifier directly. Additionally, we might look at topology of the decision boundary by viewing the system of activation regions as a *cellular (CW) complex* (learning about topological data analysis will be one of the outcomes of working on this part).

1. *Active training control.* The main idea is to investigate ways to train a neural network for a given dataset while enforcing desired properties on its regional structure. An example for such property could be a "high expressivity along the decision boundary," where boundary information would be provided by some oracle. Simultaneously, this project will investigate the validity of an assumption that the "network expressivity does not change during training" when a non-random handcrafted initialization is considered.

**Requirements:**<br>
 * Background in Machine Learning/Computer Science or Mathematics
 * Good programming skills and understanding of code organization in at least one ml library, e.g. pytorch or tensorflow

**Contacts:**<br>
 * Vladislav Polianskii, vpol (at) kth.se
 * Matteo Gamba, mgamba (at) kth.se


## References
{% bibliography -f teaching %}

{% include base_path %}

{% for post in site.teaching reversed %}
  {% include archive-single.html %}
{% endfor %}
