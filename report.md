---
title: Google Summer of Code 2015
---

2015 marked [The Processing Foundation](http://processing.org)'s fifth year participating in [Google Summer of Code](https://developers.google.com/open-source/soc/).  Following is a summary of the 15 projects, in alphabetical order by project name, completed this summer by a terrific group of students.


### 1) [p5.js Windows Port](https://github.com/processing/p5.js-editor) by [Guy de Bree](https://github.com/Bruehausu), mentored by [Sam Lavigne](https://github.com/antiboredom)

![p5.js Editor Screenshot](http://i.imgur.com/tL0GUAm.png)

For my Google Sumer of Code I developed a Windows port for the p5.js IDE, and fixed bugs for said editor. It’s now on the p5.js website! While it still has bugs, you can try it out on [the downloads page](http://p5js.org/download/). ([source code](https://github.com/processing/p5.js-editor))

### 2) New Kinect libraries [openKinect](https://github.com/shiffman/OpenKinect-for-Processing) and [KinectPV2] (https://github.com/ThomasLengeling/KinectPV2) by [Thomas Sanchez Lengeling](http://codigogenerativo.com/), mentored by [Elie Zananiri](http://dpt.co/)


![Examples of the libraries updates](http://codigogenerativo.com/wp-content/uploads/Kinect_final.png)

The goal of the project was to expand and update the existing Kinect libraries; OpenKinect-for-Processing and KinectPV2. The openKinect library now supports the new Kinect v2 for Mac and Windows and Kinect v1 for Windows and Linux. For the KinectPV2, functionalities include: skeleton tracking, face detection, process frame raw data, point cloud extraction and contour extraction. Source Code on github: [OpenKinect-for-Processing](https://github.com/shiffman/OpenKinect-for-Processing) and [KinectPV2](https://github.com/ThomasLengeling/KinectPV2).

### 3) [Processing.py 3.0 Update](https://github.com/Luxapodular/processing.py) by [Luca Damasco](https://github.com/Luxapodular), mentored by [Golan Levin](https://github.com/golanlevin)

![Processing.py Mock Image](http://i.imgur.com/mVybW32m.png)

Prior to the start of the Google Summer of Code, Processing’s Python mode would not work at all with Processing 3.0 do to some extensive back end changes. Fortunately, this summer saw the revitalization and updating of Python Mode! Users may now write Processing 3.0 Sketches using Python syntax in the new editor. Due to a few outstanding bugs, it has not yet been officially released, but feel free to try it out by building the [Processing.py Source](https://github.com/Luxapodular/processing.py) on your own machine. In addition to once again making Python Mode functional, I have edited over 1000 lines of reference code as well as ported 9 new tutorials! [Feel free to check them out and leave feedback!](https://github.com/Luxapodular/processing-py-site) 

### 4) [Web IDE for p5.js](https://github.com/therewasaguy/p5js-webIDE) by [Jason Sigal](http://jasonsigal.cc), mentored by [Daniel Shiffman](http://shiffman.net/)

![p5 web ide screenshot](http://i.imgur.com/yKAxxMD.png)

A browser-based code editor, designed specifically for the p5.js community. The project adapts the p5.js Desktop IDE (originally by Sam Lavigne, GSOC '14) for the web, with inspiration/insight from Gene Kogan's p5 Sandbox. The goal is to make it easy to create, browse, share, and remix creative code sketches directly from the browser. Every project gets a unique URL and version control (through GitHub Gists). Logged-in users can access their previous sketches, and all users can access curated p5.js examples. Create an account and start sketching! Demo at [p5ide.herokuapp.com](http://p5ide.herokuapp.com/).

### 5) Processing for ARM & Raspberry Pi by [Gottfried Haider](http://gottfriedhaider.com/), mentored by Ben Fry

Getting Processing to play well with the Raspberry Pi and similar ARM-powered computers was the focus of this project. Initial upbringing was completed and merged into Processing. The remaining bits (OpenGL support and a library for accessing the build-in hardware peripherals) currently live [in this git repository](https://github.com/gohai/processing/commits/arm), but are to be merged soon as well.

### 6) [p5.SVG](https://github.com/zenozeng/p5.js-svg) and [p5.PDF](https://github.com/zenozeng/p5.js-pdf) by [Zeno Zeng](https://github.com/zenozeng), mentored by [Danne Woo](https://github.com/dannewoo)

The main goal of p5.SVG is to provide a SVG runtime for p5.js, so that we can draw using p5's powerful API in \<svg\>, save things to svg file and manipulating existing SVG file without rasterization.

Source code on GitHub: https://github.com/zenozeng/p5.js-svg

As for p5.PDF, it's a simple PDF export module for p5.js based on browser's print to pdf function.

Source code on GitHub: https://github.com/zenozeng/p5.js-pdf

### 7) [internationalization of p5.js website](https://github.com/mayaman/p5js-website) & [collection of sketches for the p5.js community statement video](https://github.com/mayaman/p5jsCommunitySketches) by [Maya Man](https://github.com/mayaman/), mentored by [Johanna Hedva](http://www.johannahedva.com/)

![webiste (english)](http://i.imgur.com/jBwtWP3.png)
![webiste (spanish)](http://i.imgur.com/J1wwOx3.png)

This summer, I worked primarily on two separate projects. First, I rebuilt the p5.js (currently built in php) using Node.js, Assemble, Grunt, Handlebars, & YAML to support internationalization (easy tranlations from English to foreign languages // button styling to be adjusted & tranlsations to be completed at upcoming translat-a-thons). Second, I collected and currated sketches contributed from people around the world to play in the background our p5.js community statement video. Check out the projects on my github (source code below)!

[i18n site source code](https://github.com/mayaman/p5js-website)

[community sketches source code](https://github.com/mayaman/p5jsCommunitySketches)

### 8) [Video and Audio streaming library](https://github.com/nconfrey/GSoC)
**Thanks to [Andres Coulbri](https://github.com/codeanticode/) and [Gottfried Haider](https://github.com/gohai) for their exceptionally helpful code and examples. Thanks also to my mentor Dan Shiffman for direction and help throughout all the weeks.**
This project is broken up into roughly three useful parts. It originally focused on streaming media over the network, primarily video and audio streams, but evolved to include revamping Processing's video core video framework. I planned to write networking code in Java, but the project evolved to consist of learning and developing C to Java conversion through Java Native Interface and Java Native Access. Along the way I also picked up skills in video codecs, network packet payloading, and audio encoding.

The first part of the project was modifications and extensions to the existing Processing network library.

The second part was upgrading Processing's video capability to use GStreamer 1.0 instead of the depreciated GStreamer 0.10 which Processing was previously relying. Finally, the Processing community can access the most recent version of GStreamer, and with it, the most recent plugins. While the code itself is highly tailored towards videostreaming and video playback, the same JNI technique can be used to access the wealth of GStreamer resources, from CD ripping all the way to audio analysis. Processing users will now have much more power in the areas of video and audio. I have also left exposed a `public static void pipelineLaunch(String pipe)` function, which parses a GStreamer pipeline string and then launches and runs the pipeline.

The third part of the project was creating a streaming library that allows Processing users to stream local videos and songs/audio files to other sketches and other computers.
#Use Cases
Currently, the videoStreaming Processing library can do the following:
* Stream audio from one sketch to another in any of the common formats (.mp3, .wav etc.)
* Stream video from one sketch to another in most of the common formats (.mp4 and .3gp work, .mov still needs more testing)
* Stream the webcam from one computer to another using Processing
