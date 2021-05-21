# My Setup for Online Lectures

With this document I want to provide a short reference of the setup I use to record and live stream lectures.
Over the last semester I tried quite a collection of tools and have now a setup that works very well for me.
Note, that I'm by no means an expert in recording and production of videos. Most certainly there are better
variants to everything described below.

The resulting lectures (both live streams and prerecorded) can be found on my
[YouTube channel](http://www.youtube.com/c/christiandrumm).

The videos also show the improvement of the my setup over time
as well as some of the glitches that still exists (e.g. background noise).

## Requirements

The following list contains my requirements that where the basis for selecting the tools below. In order to be able
to reuse at least parts of my existing lecture content, I need the ability to

1. Record and stream the screen of my iPad
1. Use GoodNotes and the Apple Pencil for presenting my slides
1. Switch between slides and different software tools (e.g. process modelling software, SAP GUI or an IDE)
1. Switch between different screens (e.g. video only, video and slides, slides only)
1. Draw and point on the screen (e.g. to highlight features of a software)

## Software

### Max OSX

Some of these software is also available for Windows and/or Linux. However, I only tested the software on OS X (Big Sur release). 

* [OBS](https://obsproject.com/)
* [AirServer](https://www.airserver.com/)
* [ScreenBrush](https://imagestudiopro.com/screenbrush/)
* [Camtasis](https://www.techsmith.com/video-editor.html)

### iOS & iPadOS Software

* [GoodNotes](https://www.goodnotes.com/)
* [OBS Camera](https://obs.camera/)

### Web
* [Miro](https://www.miro.com)
* [YouTube](https://www.youtube.com)
  * Live streaming of videos
  * Publication of pre-recorded videos
* [Github](https://www.github.com)
  * [Lecture transcripts](https://github.com/ceedee666/transcript_information_systems_ss20/) as markdown files

## Hardware

* MacBook Pro connected to an external monitor
* iPad Pro and Apple Pencil
* [Trust GXT258](https://www.trust.com/en/product/23465-gxt-258-fyru-usb-4-in-1-streaming-microphone) USB microphone
* [Logitech StreamCam](https://www.logitech.com/en-us/product/streamcam)
* Two [Elgaot Key Light Air](https://www.elgato.com/en/key-light-air)
* [Elgaot Green Screen](https://www.elgato.com/en/green-screen)
* [Elgato Mulit Mount](https://www.elgato.com/en/master-mount) and some extensions

## Setup

### Prerequisites for live streaming

In order to live stream lectures on YouTube it is necessary to create a channel. The creation of a new
channel is described [here](https://support.google.com/youtube/answer/1646861). Besides this, the channel also
needs to be verified. The verification of a channel is described [here](https://support.google.com/youtube/answer/171664).

### Hardware Setup

The central component of my setup is the MacBook. Using different USB-4 adapters the MacBook is connected to the

* External monitor (DELL UltraSharp U3415W Monitor)
* USB microphone (Trust GXT258)
* Logitech StreamCam mounted on top of my monitor

In my current setup the microphone in front of the external monitor, a little to the left. The camera is placed on top of the monitor directly in front of me. 
All these components are positioned using the Elgato Multi Mount. The MacBook is located to
my right. Directly in front of me on the desk is my iPad.

The following images shows an overview of the whole setup.

![Hardware Setup](https://github.com/ceedee666/online-lecture-setup/blob/master/IMG_8007.png?s=400)

### Software Setup for Live Streaming

#### OBS

For each of my lectures I created a different scene set in OBS. Each scene set currently consists of 4 scenes.

1. A title scene containing just a title image
1. A video only screen that contains a background image an the video input from the iPhone  
1. A main scene containing the display capture of the external monitor and the video input from the iPhone
1. A scene containing just the display capture of the external monitor.

In all the scenes I locked all the input source in order to not accidentally change something during the live
stream.

I only use very few filters with the input source. Currently, I only use a chrome key filter on the video input and a noise
reduction on the sound input. Both filters use the default parameters.

#### AirServer

I configured AirServer to use the external monitor as the output display. 

#### MacOS X Spaces

I heavily use the MacOS X Spaces feature. For this to work properly on an external monitor it is important to tick the
check box "Displays have separate Spaces" in the Mission Control preferences.

All the applications I want to use during a live stream are open in full screen mode
on the external monitor. The Desktop Space of the external monitor is empty. I open my slides in GoodNotes on the iPad.
Using the screen monitoring feature the iPad connects to the AirServer running on the MacBook. Once the iPad is
connected to AirServer the Desktop Space shows my slides. In particular I'm able to use all the features
of GoodNote to annotate the slides during the live stream.

With all the other application running in full screen mode switching from the slide to an application is very easy.
Using a swipe with three fingers on the touch pad of the MacBook changes to the application running in full screen mode.
Switching back to the slides is also only a three finger swipe gesture on the touch pad.

#### OBS & Zoom

I the latest version OBS can act as a virtual web cam. Therefore, the output of OBS can be directly used as an input for Zoom. 
No additional software like e.g. CamTwist is required. 
The following might still be necessary to activate the usage of virtual web cams in Zoom. I haven't tried this for quite some time. 

> In order to use a virtual web cam the following commands 
> need to be executed in a terminal
> 
> ```bash
> xcode-select --install
> sudo codesign --remove-signature /Applications/zoom.us.app/
> ```

### Software Setup for Recording 

#### Camtasia
I created a template project to simplify the creation of a new recording. The template contains the intro and outro of the video 
as well as some standard screen elements. 

For the screen recording I use a standard 1920×1080px area. As a preparation for the recording I resize all the tools I need to show to 
fit into this recording area. In combination with the large external monitor, this enables me to use the remaining screen area to show e.g. my 
script for the recording. 

#### Miro 
I use Miro for all the parts where I want to build some visualisation on the screen. I usually prepare the visualisation before. 
During the recording I use the Miro app on my iPad to move parts of the visualisation into the Miro board area that I record. 
This enables me to not use my un-decipherable hand writing 😉

# Software for Teaching

In the past month I experimented heavily with different software tools during live lectures. For me the following tools work very well:

* [Zoom](zoom.us/) breakout rooms to enable group discussions and collaboration. 
* [Miro](https://miro.com/app/) as a collaborative white board.
* [Padlet](https://padlet.com/) as a collaboration tool when the extensive features of Miro ar not required.
* [Tweetback](https://tweedback.de/) for live chat and discussions. Near zero setup. Very useful to allow questions in large lectures. 
* [Quizizz](https://quizizz.com/) for live quizzes and homework. 

The semester schedule of my [lecture on information systems](https://drumm.sh/is) gives a nice overview how all these tools work together to
create engaging online lectures.
