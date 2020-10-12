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

Some of these software is also available for Windows and/or Linux. However, I only tested the software on OS X (Catalina release). 

* [OBS](https://obsproject.com/)
* [AirServer](https://www.airserver.com/)
* [ScreenBrush](https://imagestudiopro.com/screenbrush/)
* [CamTwist](http://camtwiststudio.com/)
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
* Green screen (I bought this kit on [Amazon](https://www.amazon.de/-/en/gp/product/B01MTB3T7Y))
* [Trust GXT258](https://www.trust.com/en/product/23465-gxt-258-fyru-usb-4-in-1-streaming-microphone) USB microphone
* [Logitech StreamCam](https://www.logitech.com/en-us/product/streamcam)

## Setup

### Prerequisites for live streaming

In order to live stream lectures on YouTube it is necessary to create a channel. The creation of a new
channel is described [here](https://support.google.com/youtube/answer/1646861). Besides this, the channel also
needs to be verified. The verification of a channel is described [here](https://support.google.com/youtube/answer/171664).

### Hardware Setup

The central component of my setup is the MacBook. Using different USB-4 adapters the MacBook is connected to the

* External monitor (DELL UltraSharp U3415W Monitor)
* USB microphone
* Logitech StreamCam mounted on top of my monitor

In my current setup the microphone and the tripod are placed in front of the external monitor. The MacBook is located to
my left. Directly in front of me on the desk is my iPad.

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

#### CamTwist & Zoom

I also wanted the possibility to use my OBS sceens in a Zoom meeting. This is possible using the CamTwist software.
CanTwist creates a virtual web cam that can be used as an input source in Zoom. The latest version of Zoom (5.x)
doesn't recognise virtual wab cams anymore. In order to use a virtual web cam the following commands 
need to be executedin a terminal

```bash
xcode-select --install
sudo codesign --remove-signature /Applications/zoom.us.app/
```

### Software Setup for Recording 

#### Camtasia
I created a template project to simplify the creation of a new recording. The template contains the intro and outro of the video 
as well as some standard screen elements. 

For the screen recording I use a standard 1920×1080px area. As a preparation for the recording I resize all the tools I need to show to 
fit into this recording area. In combination with the large external monitor, this enables me to use the remaining screen area to show e.g. my 
script for the recording. 

#### Miro 
I use Miro for all the parts where I want to build some visualisation on the screen. I usually prepare the visualisation before. During the recording I use the Miro app on my iPad to move parts of the visualisation into the Miro board area that I record. This enables me to not use my un-decipherable hand writing 😉
