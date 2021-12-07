---
layout: page
title: hospital bed shortage prediction
description: Predicting hospital bed shortage due to COVID-19
img: assets/img/covid.png
importance: 4
category: data science
---

Check out this <a href="https://covid19-hospital.herokuapp.com/">COVID-19 hospital app</a> I built!  

The app predicts the dates during which hospitals in the US are expected to experience bed shortage due to COVID-19. 

<div class="row">
    <div class="col-sm mt-3 mt-md-0">
        {% responsive_image path: assets/img/app_image.png title: "example image" class: "img-fluid rounded z-depth-1" %}
    </div>
</div>

The app uses COVID-19 data from the <a href="https://github.com/CSSEGISandData/COVID-19">Johns Hopkins CSSE repository</a> to fit a SIR model. It also uses state-level demographic information and hospital capacity to predict the number of COVID-19 patients that will require hospital and ICU beds. 

For details on the model, please read this <a href="https://medium.com/@irishryoon/predicting-hospital-bed-shortage-in-the-us-due-to-covid-19-2d860ecdaba2">medium post.</a> 

You can play around with the <a href="https://gist.github.com/irishryoon/fe2c769ccca1028dbda2e4a5f060fb7e"> code</a> on Google Colab.


*Note: The app uses data that was available on March 26, 2020*
