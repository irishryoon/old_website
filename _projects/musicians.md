---
layout: page
title: classical musicians recommender
description: 
img: assets/img/graph.png
importance: 1
category: data science
---

I built a recommendation system for classical music performers. The recommender is based on the idea that musicians with frequent collaborations likely have similar performance styles. It first creates a graph of classical musicians and their collaborations and uses node2vec embeddings to find vector representations of the musicians. Given a list of users' favorite artists, the recommender uses similarity of the vector representations to recommend artists that a user may enjoy. 

Checkout the app at <a href="https://musicians-rec.herokuapp.com">https://musicians-rec.herokuapp.com</a>  
Code: <a href="https://github.com/irishryoon/musicians_recommendation">github</a>  
Blog post: <a href="https://medium.com/@irishryoon/classical-musicians-recommender-22ee176daee8">medium</a>  
For interactive exploration of the artist graph, click below

[<center><img src="http://irisyoon.com/assets/img/graph.png" height ="400"></center>](http://irisyoon.com/musicians_recommendation/graph_80000/graph_visualization/network/)
