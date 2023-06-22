---
title: "COVID-19 Neural Net"
excerpt: "Project for my *Pattern Recognition* course. 
<br/><img src='/images/covid_training.gif' style='width:500px;height:260px;'>"
collection: portfolio
permalink: /portfolio/covid-neural-net/
---

A critical step in the fight against COVID-19 is effective detection of infected patients so that those 
infected can receive immediate treatment and care, as well as being isolated to mitigate the spread of 
the virus. The main detection method used to detect COVID-19 cases is the reverse transcriptase-polymerase 
chain reaction (RT-PCR).

An alternative detection method that has also been used for the detection of COVID-19 has been the radiography 
examination, where radiologists take and analyze chest radiography images (for example, CXR chest radiograph or 
CT scan) to look for visual indicators associated with COVID-19.

We used a pre-trained [MobileNetV2](https://keras.io/api/applications/mobilenet/#mobilenetv2-function)
and *data augmentation*, as the original dataset [COVID-19 CT segmentation dataset
](http://medicalsegmentation.com/covid19/) is very small. We also used *bagging* to see if we could improve the 
performance of the model. 

The code with more explanations is in my GitHub [Pattern-Recognition-COVID](https://github.com/davidguzmanr/Pattern-Recognition-COVID).

<img src='/images/covid_training.gif' style='width:500px;height:260px;' class='center'>