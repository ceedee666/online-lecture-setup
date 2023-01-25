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

### Changes after the pandemic

In the semesters after the pandemic I stopped doing pure live streams of my lectures. Instead I only have
the following to scenarios:

- Prerecording a lecture video for YouTube
- Hybrid classroom lecture (i.e. giving a lecture in the classroom and simultaneously streaming and/or recording it).

## Software

The software tools I use for recording lectures and live streaming from the classroom differ. Therefore I'll provide
a short description of the use case of each software tool.

### Mac OS

Some of these software is also available for Windows and/or Linux. However, I only tested the software on Mac OS (current
Ventura release).

| Software                                                | Use Case Description                                         |
| ------------------------------------------------------- | ------------------------------------------------------------ |
| [AirServer](https://www.airserver.com/)                 | Stream the iPad screen to the Macbook. Used during lectures. |
| [ScreenBrush](https://imagestudiopro.com/screenbrush/)  | Draw arrows, boxes etc. on screen.                           |
| [Camtasis](https://www.techsmith.com/video-editor.html) | Screen recording and video editing.                          |
| [Companion](https://bitfocus.io/companion)              | Enable Elgato Streamdeck to execute macros on the ATEM       |

### iOS & iPadOS Software

| Software                                                                        | Use Case Description                                         |
| ------------------------------------------------------------------------------- | ------------------------------------------------------------ |
| [GoodNotes](https://www.goodnotes.com/)                                         | Present pdf documents and slides and draw and write on them. |
| [MoviePro](https://apps.apple.com/de/app/moviepro-pro-video-camera/id547101144) | Use iPhone as a recording camera                             |
| [MoviePro Remote](https://apps.apple.com/de/app/moviepro-remote/id1195616020)   | Remote for MoviePro to adjust the camera                     |

### Web

| Software                           | Use Case Description                      |
| ---------------------------------- | ----------------------------------------- |
| [Miro](https://www.miro.com)       | Cooperative white board used in lectures. |
| [YouTube](https://www.youtube.com) | Publication of pre-recorded lectures.     |
| [Github](https://www.github.com)   | Code sharing.                             |

## Hardware

The hardware setup for live streaming from the classroom differs significantly from the setup used for recording.
Therefore the hardware setup is differentiated between the two cases below.

### Hardware for recording

| Hardware                                                                                            | Use Case Description                  |
| --------------------------------------------------------------------------------------------------- | ------------------------------------- |
| MacBook Pro connected to an external monitor                                                        |                                       |
| iPad Pro and Apple Pencil                                                                           |                                       |
| iPhone 13                                                                                           | Camera for video recording            |
| [ATEM Mini Pro ISO](https://www.blackmagicdesign.com/products/atemmini)                             | Video recording and live video mixer. |
| [Trust GXT258](https://www.trust.com/en/product/23465-gxt-258-fyru-usb-4-in-1-streaming-microphone) | USB microphone                        |
| Two [Elgato Key Light Air](https://www.elgato.com/en/key-light-air)                                 |                                       |
| [Elgato Green Screen](https://www.elgato.com/en/green-screen)                                       |                                       |
| [Elgato Multi Mount](https://www.elgato.com/en/master-mount)                                        |                                       |

### Hardware for live streaming

| Hardware                                                                | Use Case Description                                                     |
| ----------------------------------------------------------------------- | ------------------------------------------------------------------------ |
| MacBook Pro connected to an external monitor                            |                                                                          |
| iPad Pro and Apple Pencil                                               |                                                                          |
| iPhone 13                                                               | Camera for video recording                                               |
| [RØDE Wireless Go](https://rode.com/en/microphones/wireless/wirelessgo) | Wireless microphone. Although I would now go for the Rode Wireless Go 2. |

## Setup

### Prerequisites for live streaming

I do not live stream on YouTube any more. This description is left here only for reference.

In order to live stream lectures on YouTube it is necessary to create a channel. The creation of a new
channel is described [here](https://support.google.com/youtube/answer/1646861). Besides this, the channel also
needs to be verified. The verification of a channel is described [here](https://support.google.com/youtube/answer/171664).

### Hardware Setup for Recording

The central component of my setup is the MacBook. Using different USB-4 adapters the MacBook is connected to the

- External monitor (DELL UltraSharp U3415W Monitor)
- USB microphone (Trust GXT258)
- iPhone mounted on top of my monitor

In my current setup the microphone in front of the external monitor, a little to the left. The camera is placed on top of the monitor directly in front of me.
All these components are positioned using the Elgato Multi Mount. The MacBook is located to
my right. Directly in front of me on the desk is my iPad.

The following images shows an overview of the whole setup.

![Hardware Setup](https://github.com/ceedee666/online-lecture-setup/blob/master/IMG_8007.png?s=400)

### Software Setup for Live Streaming from Classroom

I record and stream lectures using WebEx. Although I hate the software I have to use it as it is provided by the university.
I share the MacBook screen and record it.

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

### Software Setup for Recording

#### Companion

....

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

- [Zoom](zoom.us/) breakout rooms to enable group discussions and collaboration.
- [Miro](https://miro.com/app/) as a collaborative white board.
- [Padlet](https://padlet.com/) as a collaboration tool when the extensive features of Miro ar not required.
- [Tweetback](https://tweedback.de/) for live chat and discussions. Near zero setup. Very useful to allow questions in large lectures.
- [Quizizz](https://quizizz.com/) for live quizzes and homework.

The semester schedule of my [lecture on information systems](https://drumm.sh/is) gives a nice overview how all these tools work together to
create engaging online lectures.
