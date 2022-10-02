---
layout: page
title: Philadelphia Bail Fund
description: 
img: assets/img/philly.png
importance: 4
category: data science
---
From 2020 to 2021, I volunteered as a data scientist for <a href="https://codeforphilly.org/">Code for Philly</a>, specifically the <a href="https://www.phillybailfund.org/">Philadelphia Bail Fund</a>. The volunteers and I wanted to understand how the bail system of Philadelphia was affecting the citizens. The following lists a few questions that we wanted to address.

* Which neighborhoods are most heavily impacted by the bail system?
* How do the defendant's race and gender impact the bail amount?
* Is there consistency across magistrates (the person who sets the bail)? That is, do two different magistrates set a similar bail amount for similar cases? 

The volunteers and I gathered new criminal filing records from the municipal court. We then performed various statistical analyses to address the above questions. One challenge of this analysis was that many variables were correlated, and we needed to control for the correlations. For example, if one magistrate is likely to handle more severe offenses than another, then one would have to take such differences into account when comparing the bail amounts set by the two magistrates. 
 
To that end, we used **topic modeling** on the criminal filing records to group cases into similar offense types and severity. We then performed a **matched study** to study if two magistrates set similar bail amounts given similar offense severity. We found that there is still a high variance in the bail amounts set across magistrates even after controlling for the difference in the offense type and severity. 

For more info, please visit the following app: <a href="https://codeforphilly-pbf-analysis-app-hzafyl.streamlitapp.com/">PBF app</a>  
Code: <a href="https://github.com/CodeForPhilly/pbf-analysis">github</a>  
