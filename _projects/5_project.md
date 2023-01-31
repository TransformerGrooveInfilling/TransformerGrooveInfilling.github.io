---
layout: page
title: Real-Time Plugin (VST)
description: VST Plugin (Demo and Samples)
importance: 1
category: VST Plugin
---


## Source Code
We have prepared a VST wrapper for deploying the trained models. The VST can be found [here](https://github.com/AnonUserGit/InfillingTransformerRealTime_VST). 


## Tutorial

Here is a video describing how the plugin works


<iframe width="560" height="315" src="https://www.youtube.com/embed/wiLnZNYUAbM" title="VST Tutorial" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" allowfullscreen></iframe>



## Example Generation Using the Plugin

We have selected 3 types of samples from (freesound.org)[https://freesound.org/). 

1. Percussive Loops
2. Vocal Loops
3. Other Types

The VST was used with these samples to generate infilling suggestions. 


`IMPORTANT` The parameters of the plugin were adjusted to obtain the samples. 

In the videos:
	
- `IH` refers to Infilling of HiHats (model is trying to add hiatus to the audio loop)
- `IKS` refers to Infilling of Kick Snares (model is trying to add kicks and snares to the audio loop)
- `IRL` refers to Infilling of Random Events (using low version of the randomly masked model)
- `IRH` refers to Infilling of Random Events (using high version of the randomly masked model)


#### Percussive Loops

<iframe width="560" height="315" src="https://www.youtube.com/embed/Z9aIBfVUX5k" title="Percussive Inputs" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" allowfullscreen></iframe>


#### Vocal Inputs

<iframe width="560" height="315" src="https://www.youtube.com/embed/10RkT089cbA" title="Vocal Inputs" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" allowfullscreen></iframe>


#### Other Inputs

<iframe width="560" height="315" src="https://www.youtube.com/embed/EO8-uIbWGUI" title="Other Inputs" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" allowfullscreen></iframe>