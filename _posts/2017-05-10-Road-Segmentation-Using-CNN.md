---
layout: post
title: Road Segmentation from Aerial images using CNNs
img: images/overlay_40.png
---

A while ago, on a Master's course, I had to do a project using Convolutional Neural Networks. In the beginning it seemed to be a daunting task but it ended up being a fun and exciting project. The goal of the project was to correctly classify aerial image pixels into road and non-road pixels. Although it might seem simple in the beginning, there are several features and characteristics of images of roads that make it hard to classify them correctly.

For example, the sun might be shining in some pictures and it might be cloudy on others. The contrasts in the images are therefore different. Also, cars might be parked on the side of the roads. How can we tell if there is a road under the parked car?

![Trees Image]({{ "/images/roadseg/trees.png" | absolute_url }})
![Overlay Image]({{ "/images/roadseg/cars.png" | absolute_url }})

--<cite> Trees appear to be cutting the road and also cars classify as a road on this attempt on classifying!</cite>


Highways also proved to be hard to classify due to their different shape compared to normal roads. Parking spots are also hard to classify. The dataset provided classified parking spots as non-road. However, due to being coverend in asphalt and containing cars, the CNN kept classifying them as road.


![Highway Image]({{ "/images/roadseg/highway.png" | absolute_url }})
![Highway Image]({{ "/images/roadseg/parking.png" | absolute_url }})

--<cite> A highway horribly classified and a parking being considered a road.</cite>


The paper describing the implementation and the architecture of the network is provided in the following link.

[Download Document]({{ site.url }}/assets/RoadSegmentation.pdf)

Also I have to thank Igor Pesic and Minesh Patel for being the co-authors of the work.

