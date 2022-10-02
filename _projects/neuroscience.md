---
layout: page
title: topology & neuroscience
description: A topological approach to neural encoding
img: assets/img/neuro_img.png
importance: 1
category: research
---

What does it mean for there to be circular structures in neural activity? 

Consider a collection of images with different orientations shown in the following figure (Figure 1A). We consider the red and dark orange images as having high similarity, whereas the red and green images have a low similarity. What would happen if we arranged the eight images in a way that respects this similarity? The eight images would be arranged in a circular fashion, as shown in Figure 1B. 

<div class="row">
    <div class="col-sm mt-3 mt-md-0">
        {% responsive_image path: assets/img/neuro_cyclic_structures.png title: "example image" class: "img-fluid rounded z-depth-1" %}
    </div>
</div>
<div class="caption">
	Figure 1. Circular structure of data. **A.** Collection of images. **B.** An arrangement of images based on the similarity of orientation reveals a circular structure. **C.** Collection of neural activities (spike trains). **D.** Consider two spike trains to be similar if the vertical lines are well-aligned after "sliding" one spike train by a small amount. An arrangement of neural activity based on spike train similarity reveals a circular structure.   
</div>

Similarly, consider a collection of neural activities (called spike trains) shown in Figure 1C. Each row indicates the activity of a single neuron over some time period. The vertical line indicates the neuron's firing at a corresponding time. If we observe the neuron for, say $$ M $$ time intervals, then each spike train is a binary vector in $$ \mathbb{R}^M $$. Given two spike trains $$ s_1 $$ and $$ s_2 $$, let's measure similarities between two spike trains as the amount one needs to ``slide" $$ s_1 $$ to ``match" with $$ s_2 $$. Then, the red spike train is similar to the dark orange spike train, but it is quite dissimilar to the green spike train. Again, if we were to arrange the spike trains in a way that respects this similarity, we would arrange them in a cyclic manner (Figure 1D). 

Now, suppose there are many images and long spike trains that we cannot make the arrangements by hand. How would a computer recognize that these high-dimensional data contain cyclic structures? Let $$ P $$ denote the point cloud representing a system of interest, such as the collection of stimulus or neural activity. We calculate the similarity between every pair of elements in the system. We construct a representation of the system as we vary the similarity level by a sequence of simplicial complexes. The loops in this sequence are summarized by a persistence diagram, where the points far from the diagonal represent the large loops. See the following figure. 

<div class="row">
    <div class="col-sm mt-3 mt-md-0">
        {% responsive_image path: assets/img/neural_PH.png title: "example image" class: "img-fluid rounded z-depth-1" %}
    </div>
</div>
<div class="caption">
	Detecting circular structures from high dimensional data. Given the data (either images or spike trains), we first compute a matrix encoding pairwise similarity between all elements in the system. We then create the sequence of simplicial complexes that represents the connectivity of the system at various similarity values. Finally, we summarize the loops in the simplicial complexes using a persistence diagram. As before, points far from the diagonal represent significant structures.
</div>


So far, we have seen that persistence diagrams can indicate if a collection of images or spike trains contain circular structures. Consider a hypothetical experiment in which we present a stimulus video to a mouse while measuring its neural activity. Let's assume that the persistence diagram indicates that there are two circular structures in the stimulus and one circular structure in the neural activity. Is the unique circular feature in the neural activity reflecting one of the circular features in the stimulus? If so, which one? Such questions are topological manifestations of fundamental problems in neuroscience called neural encoding that study how neurons represent information. 

<div class="row">
    <div class="col-sm mt-3 mt-md-0">
        {% responsive_image path: assets/img/encoding.png title: "example image" class: "img-fluid rounded z-depth-1" %}
    </div>
</div>
<div class="caption">
	Neural encoding, stated as a problem in topology. Consider an experiment in which we present some stimulus while measuring neural activity. The persistence diagrams indicate that there are two circular features in the stimulus while there is only one circular feature in the neural activity. Which feature of the stimulus is represented by the neurons?
</div>


<figure>
  <img src="https://github.com/irishryoon/irishryoon.github.io/blob/4695cd962724a74ff89650897d0185cef439b594/assets/img/encoding.png"/>
  <figcaption>Neural encoding, stated as a problem in topology. Consider an experiment in which we present some stimulus while measuring neural activity. The persistence diagrams indicate that there are two circular features in the stimulus while there is only one circular feature in the neural activity. Which feature of the stimulus is represented by the neurons?</figcaption>
</figure>

To address the above questions, I developed a framework for comparing the persistence diagrams from the stimulus space and the neural activity called the analogous bars method.

The methods paper has been accepted in the Journal of Applied and Computational Topology, conditional on minor revisions. A follow-up paper implementing the method on simulated and experimental neuroscience datasets is under preparation.

*Joint work with <a href="http://www.chadgiusti.com/">Chad Giusti</a> (U. Delaware) and <a href="https://www.math.upenn.edu/~ghrist/">Robert Ghrist</a> (U. Penn).*


