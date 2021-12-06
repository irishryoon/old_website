---
layout: page
title: computational neuroscience
description: A multi-system comparison framework for neural population encoding and propagation.
img: assets/img/neuro_img.png
importance: 1
category: research
---


While network science offers exceptional tools for neuroscience, they are limited by the assumption that the system of interest fundamentally consists of pairwise interactions only. <a href="https://link.springer.com/article/10.1007/s10827-016-0608-6"> Algebraic topology</a>, on the other hand, provides powerful tools for studying complex systems with higher-order interactions. I use algebraic topology to study neural activity structure. 

In particular, I am interested in how multiple brain regions collectively process information. For example, it is known that information is projected from the primary visual cortex (V1) to higher visual areas such as the anterolateral area (AL). However, not much is understood regarding the nature of the projection: How selective is the information distributed to higher visual areas? How much of the information encoded is a result of the projection? 

To address the above questions, I developed a framework for comparing neural activity structures in multiple brain regions. Topological methods can be applied to the correlation matrix of spike trains to extract encoded information in each brain region, as illustrated in the following figure. Given spike trains that have been recorded simultaneously from multiple brain regions, I used spike train correlations across brain regions to trace the encoded information from one brain region to another. The algorithm allows researchers to better understand the nature of the information distribution process across brain regions. 

<div class="row">
    <div class="col-sm mt-3 mt-md-0">
        {% responsive_image path: assets/img/neuroscience.png title: "example image" class: "img-fluid rounded z-depth-1" %}
    </div>
</div>
<div class="caption">
    This image can also have a caption. It's like magic.
</div>


*<span style = "font-size:0.8em">Correlations among spike trains can be used to build a topological space representing the information encoded in the brain regions. The topological features are summarized in the barcodes. </span>* 

Paper and code are scheduled to appear on arXiv in December 2021. 

*Current project at University of Pennsylvania & University of Delaware (2019-2021). Joint work with <a href="http://www.chadgiusti.com/">Chad Giusti</a> (U. Delaware) and <a href="https://www.math.upenn.edu/~ghrist/">Robert Ghrist</a> (U. Penn).*


