# WebVR, Aframe, and Blender 
## TechCore "Level Up" presentation
**Presenter: Devin Bayly** (pronouns he/him)

**Title: Computation Specialist**

**Department: Research Technologies**

**Team: Data & Visualization**

## Introduction
### Background


* Work with researchers and members of the university community to bring their data to life
* Interests are in visualizations on the Web with an emphasis on emerging technology
* Outreach, contribution and open web advocacy with Mozilla (pm me if you're interested in campus group) 

**Links**

* Project request form for Data & Visualization Consulting [https://rtdv-intake.glitch.me](https://rtdv-intake.glitch.me)
* baylyd@email.arizona.edu
* [DevinBayly@github](https://github.com/DevinBayly)


### Material to cover

* WebVR
    * Discussion of strengths and weaknesses
* Aframe
    * Introduction and hands on via [https://glitch.com](https://glitch.com)
* Blender
    * Incorporating modeling into WebVR
* Additional topics
    * Intermediate level scripting for Aframe
    * UV material styling in Blender
    * Social VR in Hubs by Mozilla

## WebVR

*In our current day it is increasingly important to have digital access to real world objects and experiences. It is timely you attended this workshop =D.* 

[webvr examples](https://webvr.directory/)
[super craft/medium](supermedium.com) <--building WebVR in WebVR (**inception?**)

Interesting conversation [reddit](https://www.reddit.com/r/WebVR/comments/3e2mes/what_are_the_advantages_of_webvr_over_native_vr/)

Strengths

* Built on (embarrasingly?) accessible foundations of the internet
* Open: Anyone can be an author
* Interconnected: Anyone can access a wide array of existing materials both VR content and regular web content
* Social
* Lightweight: fast iterations of development

Weaknesses

* Bottlenecks: Memory and cpu/gpu processing power is limited

**Important**

"get it right in black and white" -- Maureen Stone

Frequently it is a limitation in the design rather than the technology that ends up being an issue with Virtual Reality, therefore perhaps do your development initially in WebVR and if pitfalls occur switch

*Caveat if it is clear from start that performance bottlenecks will exist, perhaps not*


## Aframe

[Examples](https://aframe.io/aframe/examples/)


[Docs homepage](https://aframe.io/docs/1.0.0/introduction/)

[Aframe School](https://aframe.io/school/) <--excellent resource!

Aframe is

* A markup language for Virtual Reality similar to html the backbone of the web
* An Entity Component System, meaning VR elements are relatively easier to create and share than in other systems (Unity, Unreal) 
    * Geared towards beginners who want to get up and running
* A wonderful partner to [glitch.com](https://glitch.com)

To get started click this [link](http://glitch.com/~aframe) and select **remix your own**

![pic](./20200317T161605445734.png)

### Viewing and Modifying

Congrats you have just started your glitch application!

To rapidly view the changes you've made in your code click the sunglasses button with the word **Show** in it, and select **next to the code**


![](./20200317T163443881078.png)

Try modifying the color of each object

* click "index.html" in the file browser at the left side
* change `color="#4CC3D9"` to `color="...whatever you want..."`
* experiment with modifying other aspects of the shapes

* These are components but we will talk more about them if we have time

### Models and WebVR

* download some of the models from the github [khronosgroup samples](https://github.com/KhronosGroup/glTF-Sample-Models/tree/master/2.0) selecting the `.glb/glTF-Binary` file format
* upload them via the **Upload an Asset** button

![](20200317T164415324882.png)

* copy the link of the asset
* paste into url part of 
    * `      <a-entity gltf-model="url(...here...)" scale="100 100 100"></a-entity>
`
* remove the `?v=...` text at the end of the link
* put that `<a-entity` into the file

### Creating models: Blender

**Clone the github repo if you haven't already** or download files from the model folders at [https://github.com/DevinBayly/tech-core-presentation](https://github.com/DevinBayly/tech-core-presentation) using the download option
![](./20200317T165140068020.png)

Installation

* Head [here](https://www.blender.org/) to download Blender 2.8

Loading models

* From the files drop down select import
* Select which ever folder you
