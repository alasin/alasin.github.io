---
layout: page
title: Projects
permalink: /projects/
---

**GSoC '15 - Cloud removal from satellite imagery for GeoTrellis**

[GeoTrellis](http://geotrellis.io/) is an open-source, scala-based geospatial data processing framework.
Clouds and cloud shadows often obscure parts of images acquired by satellites or other space-borne sensors. However, useful image data could be extracted from other relatively non-cloudy images of the same geographical location that can be used to 'fill' these obscure parts. When combined together with the right algorithms, these images can offer a cloud-free (or nearly cloud-free) view of that area.

This project aimed to enable GeoTrellis to remove clouds from a large set of imagery. Combined with it's power to process large amount of raster data, it would enable users to run this process over any amount of imagery, in a scalable way. Scala was a completely new language for me before the start of the project, but my mentor [Rob](http://www.azavea.com/about-us/staff-profiles/rob-emanuele/), was a great guide throughout the project.

We tested our algorithms on [this](https://www.google.com/maps/place/Ompah,+ON,+Canada/@45.0291377,-76.7892811,13630m/data=!3m1!1e3!4m5!3m4!1s0x4cd24d3c2a575b1b:0x13e80edfa856300!8m2!3d45.0081417!4d-76.8357792) geographical location as it's cloudy and snowy here most part of the year.

<u>Some input images:</u>

[![image1](/public/images/image0_thumb.png)](/public/images/image0.png)
[![image2](/public/images/image1_thumb.png)](/public/images/image1.png)
[![image3](/public/images/image2_thumb.png)](/public/images/image2.png)
[![image4](/public/images/image3_thumb.png)](/public/images/image3.png)
[![image5](/public/images/image4_thumb.png)](/public/images/image4.png)
[![image6](/public/images/image5_thumb.png)](/public/images/image5.png)

<u>Resultant image:</u>

[![image6](/public/images/cloudlessimage_thumb.png)](/public/images/cloudlessimage.png)


**Digital Archive for Paintings - A text and content-based image retrieval system**

Shekhawati paintings in Rajasthan have adorned the walls of havelis and houses since 17th century. This project aimed at creating a digital archive for these paintings and murals where we can search for digital paintings based on their annotations and image features. I did this Digital Humanities research project under the supervision of [Prof. Sundar S. Balasubramaniam](http://www.bits-pilani.ac.in/pilani/sundarb/profile) and [Prof. Geetha B.](http://universe.bits-pilani.ac.in/goa/geethab/Profile).

A simple tag and content-based image retrieval system was built for the web platform to facilitate image search through the database.

<u>Some snapshots:</u>

[![image1](/public/images/t_search_thumb.png)](/public/images/t_search.png)
[![image2](/public/images/i_search_thumb.png)](/public/images/i_search.jpg)


You can find the project code on [Github](https://github.com/alasin/Digital-Archive-CBIR).


**Optimizing human-machine task assignments for computer vision**

This project was done as a part of [Aspiring Researcher Challenge](https://aspiringresearchers.soe.ucsc.edu/). My team worked with [Prof. James Davis](https://users.soe.ucsc.edu/~davis/index.html) on optimizing human-machine task assignments for Computer Vision. As a team, we built an AI-human object localizer using computer vision classifiers and complementary human input when required in the form of an interactive web interface. Partial results were published in the form of a [work-in-progress poster](http://arxiv.org/abs/1509.07543) at AAAI HCOMP 2015.

Code and results can be found [here](https://github.com/alasin/DenseMatrix-AR) and [here](https://github.com/gcr/arc-evaluator).


**Ship-mounted camera simulator**

Efficacy of camera systems cannot be determined accurately without testing its performance on real-time scenarios. Since datasets from oceans, deserts and other terrains cannot be easily obtained, there is a need to simulate these scenarios so that the software can be tested in these virtual environments and necessary changes could be made to it.
The simulated environment needs to account for the periodic and non-periodic environmental changes and be customizable as per the software needs.

This project dealt with creating such a virtual ocean environment which allows user to test camera systems with different zoom levels, field-of-view and focal lengths on a single virtual platform. It also allows user to customize the ocean scene (wave height, wind speed, reflections etc.) depending upon the user’s requirements.
It can, therefore, serve as a preliminary test for testing the camera performance, measuring tracking accuracy and marking targets under a variety of otherwise unforeseeable scenarios.

<a href="https://www.dropbox.com/s/3nmmpzhayfcsweg/Terrain_simulator.mp4?dl=0" target="_blank">Click here</a> for a demo video.


**Rolling shutter rectification and image stabilization using IMU**

Rolling shutter artifacts are fairly common in CMOS sensors, which are used in almost all smartphone cameras today. Add camera shake to that and you'll have an unstabilized video recording with rolling shutter distortion. During my internship at Tonbo Imaging, I made a prototype stabilized camera using an Invensense IMU that uses the gyrosensor measurements to stabilize the video in real-time and remove rolling shutter artifacts. Since gyrosensor records the change in angular momentum of the device in *X*, *Y* and *Z* directions, integrating the values over a *dt* time gives us the change in angular displacement which can be used to *shift* and rectify the image pixels accordingly. The algorithm was tested for thermal cameras as well, in which normal software stabilization fails owing to the lack of features. The algorithms were later ported on to Android as an app which used the inbuilt gyrosensor for required measurements.


**Real-time multiple image fusion and panorama generation**

The project involved fusing multiple visible camera images with IR images digitally and stitching them together for an enhanced driver vision system. The algorithms worked at >25 FPS on an embedded board for four video streams (2 visible + 2 IR). The work was extended to work for 24 camera streams (12 visible + 12 IR) with the complete panorama output being streamed out in real-time.

<u>Sample Images</u>

[![image1](/public/images/left-thumb.png)](/public/images/left.png)
[![image2](/public/images/right-thumb.png)](/public/images/right.png)

<u>Result</u>

[![image3](/public/images/pano-thumb.png)](/public/images/pano.png)


**Real-time motion detection and object tracking**

Developed efficient algorithms for blob detection, registration and prediction for a generalized object tracker. The system was deployed on an embedded device where it worked >25 FPS for a 512x512 image.


**GSoC '14 - KF5 port of KDE Games**

This project was mostly about porting the [KDE Games](https://games.kde.org/) module to the new KDE Frameworks. The motivation behind the project was to keep KDE Games bit rot-free and maintained with respect to the latest libraries, as all the KDE applications were being ported. I specifically chose to work on KDE Games because I really enjoyed them playing on my Kubuntu distribution and had previously contributed to [KBounce](https://en.wikipedia.org/wiki/KBounce), the former being the reason for the latter. I also ported three standalone games including KBounce to the new frameworks as part of the project.

<u>Github links</u>:<br>
[libkdegames](https://github.com/KDE/libkdegames)<br>
[KBounce](https://github.com/KDE/kbounce)<br>
[KMines](https://github.com/KDE/kmines)<br>
[KNavalBattle](https://github.com/KDE/knavalbattle)<br>


**Automated image manipulation and calibration framework for a novel lensometry algorithm**

Worked with [Dr. Tim Poston](https://en.wikipedia.org/wiki/Tim_Poston) on a novel lensometry algorithm. I developed automatic calibration and registration procedures for relating a ground-truth color image with a photograph of the same image taken through a lens. The relation described the color changes and the mathematical  pattern and deviation these color changes follow when passed through a lens.

**TIFF Image Compressor**

The project involved creating a Java based application to compress large medical Images of .TIF format using different lossless image compression algorithms (LZW, Packbits etc.) and comparing the efficiencies of those algorithms based on the compression ratio obtained.

Code is available [here](https://github.com/alasin/TIFFCompressor).


**iJADE based weather monitoring system**

I studied the Multi Agent System architecture and it’s application to a Weather Monitoring System which studies
the given weather data, processes it and makes prediction using Neuro-Fuzzy algorithms. As part of the project, I created a Java/JADE based prototype agent that automatically logs and compares yearly rainfall data over the past 5 years.
