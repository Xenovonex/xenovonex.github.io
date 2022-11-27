---
layout: default
title: Master Thesis
---

[Back to Master projects](./master.md)
## MSc. Thesis: Sharpening the Future of Occupancy Grid Map Prediction Methods: An Investigation into Loss Functions and Semantic Segmentation Multi-Task learning for More Accurate OGM Predictions
#### Date of Thesis Defence: 13 June 2022
<img src="/assets/img/pipeline_av.png" alt="pipeline_av" width="600"/>\
A diagram example of the Autonomous Navigation Process. The sensors and actuators
(black) measure and act on the environment (green), respectively. The cognitive processing steps
(dark and light blue) interpret the sensor data and make vehicle control decisions based on those
interpretations. This thesis focuses on the Motion Prediction cognitive processing step (light blue).

### Author
Rutger Dirks
### Thesis Committee
H.J. Boekema (daily supervisor), Prof. Dr. D.M. Gavrila (supervisor), Dr. J.F.P. Kooij, Dr. E.A.I. Pool (previous supervisor)
### Degree granting institution
[Delft University of Technology](https://www.tudelft.nl/en/about-tu-delft/facts-and-figures/tu-delft-in-international-rankings)
### Programme
Mechanical Engineering | Vehicle Engineering | Cognitive Robotics

# [LINK TO THESIS](http://resolver.tudelft.nl/uuid:efb50fdd-c246-4e55-8193-5cf78072ec29)

## Abstract
"For an Autonomous Vehicle (AV) to traverse safely in traffic, It is vital it can anticipate the behavior of
surrounding traffic participants using motion prediction. Current motion prediction approaches can be
categorized into object-centered and object-agnostic methods and are primarily based on deep learning.
The former relies on a human-engineered pipeline of object detection and tracking, of which the errors
can accumulate in the motion predictions. The latter does not rely on this pipeline; however, it lacks
the ability to learn object representations causing blurriness and object disappearances for longer-term
predictions which forms a safety hazard.
This thesis proposes two methods to improve the performance of the object-agnostic sequence-tosequence
Occupancy Grid Map (OGM) prediction networks, trained on the Waymo Open Perception
dataset. The first method uses inter-pixel loss functions, i.e. the SSIM and Sinkhorn losses, instead of
the ubiquitously used per-pixel losses, to train the PredRNN++ Occupancy Grid Map (OGM) prediction
network. Inter-pixel losses take into account the spatial relations between grid cells during the evaluation
of OGMs, whereas per-pixel losses evaluate each grid cell’s value independently. The quantitative
results demonstrate that using inter-pixel losses can improve short term predictions with a prediction
horizon of T = 5 for the Mean Squared Error (MSE) by 4.3%, Image Similarity (IS) by 7.8%, Average
Precision (AP) by 0.3%, metrics. For the longer term, T = 15, the predictions improve for the MSE
by 5.0%, IS by 20.5%, AP by 0.1%, and Accuracy by 0.6%. Furthermore, the use of inter-pixel losses
reduces blurriness and object disappearances. The second method is based on multi-task learning.
By training the PredRNN++ to perform the prediction task together with the semantic segmentation
task on the predicted OGMs, it is expected to learn object representations which it uses to improve the
prediction quality. The quantitative results show that multi-task learning does not improve the OGM
predictions. However, some qualitative results show that multi-task learning reduces blurriness and
object disappearances." 

(R.F. Dirks, 2022, _"Sharpening the Future of Occupancy Grid Map Prediction Methods: An Investigation into Loss Functions and Semantic Segmentation Multi-Task learning for More Accurate OGM Predictions"_, TU Delft Mechanical, Maritime and Materials Engineering)

<img src="/assets/img/dl_pipeline.png" alt="pipeline_dl" width="600"/>\
The Deep Learning Pipeline that is researched in the thesis.

## Subject
* Motion Prediction
* Deep Learning
* Loss Functions
* Multi-task learning
* Occupancy Grid Map
* Sinkhorn Loss
* Structural Similarity Index Measure
* Semantic Segmentation
* Research
