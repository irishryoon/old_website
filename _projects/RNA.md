---
layout: page
title: RNA structure sampling & clustering
description: a project with a background image
img: assets/img/SAMIII_conformation2.png
importance: 2
category: research
---
A RiboNucleic Acid (RNA) can form complex structure through intra-molecular base-pairing. Some classes of RNAs can regulate biological functions by changing its conformations. An example is illustrated below.   


<div class="row">
    <div class="col-sm mt-3 mt-md-0">
        {% responsive_image path: assets/img/SAMIII_conformation1.png title: "example image" class: "img-fluid rounded z-depth-1" %}
    </div>
    <div class="col-sm mt-3 mt-md-0">
        {% responsive_image path: assets/img/SAMIII_conformation2.png title: "example image" class: "img-fluid rounded z-depth-1" %}
    </div>
</div>
*<span style = "font-size:0.8em">The SAM-III riboswitch folds into two distinct secondary structures. It regulates gene expression by exposing or sequestering the SD sequence, which controls translation.</span>* 

Identifying multiple structures of a RNA can bring therapeutic advancements for RNA viruses. A popular approach is to sample low-energy structures from the nearest neighbor thermodyanmic model. Most algorithms follow the general flow of <b>sampling</b>, <b>clustering</b>, and reporting <b>cluster representatives</b>.

I worked on improving the <b>clustering</b> aspect of an RNA structure prediction algorithm called <a href="https://github.com/gtDMMB/RNAStructProfiling">profiling</a>. The current method resulted in too many clusters with negligible biological difference. I proposed algorithmic ways to identify clusters that should be merged based on structural similarity. The enhanced version of profiling is under development by Georgia Tech <a href="https://github.com/gtDMMB">Discrete Mathematics and Molecular Biology</a> group.

I also examined the prospect of using current methods to identify new multimodal RNAs. I found that there is a class of RNAs (kinetic riboswitches) that is difficult to detect from current sampling methods. I proposed a simple co-transcription simulation method to identify multimodality of such RNAs. The results have been published in this <a href="https://www.researchgate.net/publication/337314911_Towards_an_understanding_of_RNA_structural_modalities_a_riboswitch_case_study">paper.</a> 

*Georgia Tech (2018-2019), joint work with <a href="https://sites.google.com/site/christineheitsch/">Christine Heitsch</a> (Georgia Tech) and <a href="https://ribosnitch.bio.unc.edu/">Alain Laederach</a> (UNC).*