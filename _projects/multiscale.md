---
layout: page
title: Sheaf theory for data science
description: Applications of persistent sheaf cohomology.
img: assets/img/PointCloudExample.png
importance: 4
category: research
---

For my PhD dissertation, I worked on applications of topology to data science. I used <b>cosheaves</b> and <b>spectral sequences</b> to compute <b>persistence</b> in a distributed manner. I applied such distributed computation to study <b>multi-density data</b> and recovered the information lost in persistence diagrams. 

For example, consider the following point cloud and its coresponding persistence diagram in dimension one.

<div class="row">
    <div class="col-sm mt-3 mt-md-0">
        {% responsive_image path: assets/img/PointCloudExample.png title: "example image" class: "img-fluid rounded z-depth-1" %}
    </div>
    <div class="col-sm mt-3 mt-md-0">
        {% responsive_image path: assets/img/PD.png title: "example image" class: "img-fluid rounded z-depth-1" %}
    </div>
</div>

By observing the persistence diagram, one would conclude that there is one significant feature. However, one can see from the point cloud that there are small but significant features that are densely sampled. My construction of distributed computation allows one to identify such significant features that are neglected by traditional methods. 

Here is a 30 minute video of my presentation at <a href="https://www.ima.umn.edu/2017-2018/SW5.21-25.18/27292">IMA special workshop on Bridging Statistics and Sheaves.</a>

The paper can be found on <a href="https://arxiv.org/abs/2001.01623">arXiv.</a> Here is a copy of my <a href="https://repository.upenn.edu/edissertations/2936/">PhD dissertation.</a>


*University of Pennsylvania (2013-2018), PhD dissertation. Joint work with <a href="https://www.math.upenn.edu/~ghrist/">Robert Ghrist</a> (U. Penn).*

