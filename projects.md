---
layout: page
title: Projects
permalink: /projects/
---

**GSoC '14 - KF5 port of KDE Games**

This project was mostly about porting the [KDE Games](https://games.kde.org/) module to the new KDE Frameworks. The motivation behind the project was to keep KDE Games bit rot-free and maintained with respect to the latest libraries, as all the KDE applications were being ported. I specifically chose to work on KDE Games because I really enjoyed them playing on my Kubuntu distribution and had previously contributed to [KBounce](https://en.wikipedia.org/wiki/KBounce), the former being the reason for the latter. I also ported three standalone games including KBounce to the new frameworks as part of the project.
<br>Github links:<br>
[libkdegames](https://github.com/KDE/libkdegames)<br>
[KBounce](https://github.com/KDE/kbounce)<br>
[KMines](https://github.com/KDE/kmines)<br>
[KNavalBattle](https://github.com/KDE/knavalbattle)<br>

**GSoC '15 - Cloud removal from satellite imagery for GeoTrellis**

[GeoTrellis](http://geotrellis.io/) is an open-source, scala-based geospatial data processing framework.
Clouds and cloud shadows often obscure parts of images acquired by satellites or other space-borne sensors. However, useful image data could be extracted from other relatively non-cloudy images of the same geographical location that can be used to 'fill' these obscure parts. When combined together with the right algorithms, these images can offer a cloud-free (or nearly cloud-free) view of that area.<br>
This project aimed to enable GeoTrellis to remove clouds from a large set of imagery. Combined with it's power to process large amount of raster data, it would enable users to run this process over any amount of imagery, in a scalable way. Scala was a completely new language for me before the start of the project, but my mentor [Rob](http://www.azavea.com/about-us/staff-profiles/rob-emanuele/), was a great guide throughout the project.<br>
We tested our algorithms on [this](https://www.google.com/maps/place/Ompah,+ON,+Canada/@45.0291377,-76.7892811,13630m/data=!3m1!1e3!4m5!3m4!1s0x4cd24d3c2a575b1b:0x13e80edfa856300!8m2!3d45.0081417!4d-76.8357792) geographical location as it's cloudy and snowy here most part of the year.

*Some input images:*<br>
[![image1](/public/images/image0_thumb.png)](/public/images/image0.png)
[![image2](/public/images/image1_thumb.png)](/public/images/image1.png)
[![image3](/public/images/image2_thumb.png)](/public/images/image2.png)
[![image4](/public/images/image3_thumb.png)](/public/images/image3.png)
[![image5](/public/images/image4_thumb.png)](/public/images/image4.png)
[![image6](/public/images/image5_thumb.png)](/public/images/image5.png)

*Resultant image:*<br>
[![image6](/public/images/cloudlessimage_thumb.png)](/public/images/cloudlessimage.png)

**Digital Archive for Paintings - A text and content-based image retrieval system**

**Optimizing human-machine task assignments for computer vision**

**Rolling shutter rectification and image stabilization using IMU**

**Ship-mounted camera simulator**

**Real-time multiple image stitching and panorama generation**

**Real-time motion detection and object tracking**

**iJADE based weather monitoring system**

**Automated image manipulation and calibration framework for a novel lensometry algorithm**

**TIFF Image Compressor**
