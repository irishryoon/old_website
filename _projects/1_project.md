---
layout: page
title: computational neuroscience
description: a project with a background image
img: assets/img/12.jpg
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

Paper and code are under preparation. 

*Current project at University of Pennsylvania (2019-2021). Joint work with <a href="http://www.chadgiusti.com/">Chad Giusti</a> (U. Delaware) and <a href="https://www.math.upenn.edu/~ghrist/">Robert Ghrist</a> (U. Penn).*





Every project has a beautiful feature showcase page.
It's easy to include images in a flexible 3-column grid format.
Make your photos 1/3, 2/3, or full width.

To give your project a background in the portfolio page, just add the img tag to the front matter like so:

    ---
    layout: page
    title: project
    description: a project with a background image
    img: /assets/img/12.jpg
    ---

<div class="row">
    <div class="col-sm mt-3 mt-md-0">
        {% responsive_image path: assets/img/1.jpg title: "example image" class: "img-fluid rounded z-depth-1" %}
    </div>
    <div class="col-sm mt-3 mt-md-0">
        {% responsive_image path: assets/img/3.jpg title: "example image" class: "img-fluid rounded z-depth-1" %}
    </div>
    <div class="col-sm mt-3 mt-md-0">
        {% responsive_image path: assets/img/5.jpg title: "example image" class: "img-fluid rounded z-depth-1" %}
    </div>
</div>
<div class="caption">
    Caption photos easily. On the left, a road goes through a tunnel. Middle, leaves artistically fall in a hipster photoshoot. Right, in another hipster photoshoot, a lumberjack grasps a handful of pine needles.
</div>
<div class="row">
    <div class="col-sm mt-3 mt-md-0">
        {% responsive_image path: assets/img/5.jpg title: "example image" class: "img-fluid rounded z-depth-1" %}
    </div>
</div>
<div class="caption">
    This image can also have a caption. It's like magic.
</div>

You can also put regular text between your rows of images.
Say you wanted to write a little bit about your project before you posted the rest of the images.
You describe how you toiled, sweated, *bled* for your project, and then... you reveal it's glory in the next row of images.


<div class="row justify-content-sm-center">
    <div class="col-sm-8 mt-3 mt-md-0">
        {% responsive_image path: assets/img/6.jpg title: "example image" class: "img-fluid rounded z-depth-1" %}
    </div>
    <div class="col-sm-4 mt-3 mt-md-0">
        {% responsive_image path: assets/img/11.jpg title: "example image" class: "img-fluid rounded z-depth-1" %}
    </div>
</div>
<div class="caption">
    You can also have artistically styled 2/3 + 1/3 images, like these.
</div>


The code is simple.
Just wrap your images with `<div class="col-sm">` and place them inside `<div class="row">` (read more about the <a href="https://getbootstrap.com/docs/4.4/layout/grid/">Bootstrap Grid</a> system).
To make images responsive, add `img-fluid` class to each; for rounded corners and shadows use `rounded` and `z-depth-1` classes.
Here's the code for the last row of images above:

{% raw %}
```html
<div class="row justify-content-sm-center">
    <div class="col-sm-8 mt-3 mt-md-0">
        {% responsive_image path: assets/img/6.jpg title: "example image" class: "img-fluid rounded z-depth-1" %}
    </div>
    <div class="col-sm-4 mt-3 mt-md-0">
        {% responsive_image path: assets/img/11.jpg title: "example image" class: "img-fluid rounded z-depth-1" %}
    </div>
</div>
```
{% endraw %}
