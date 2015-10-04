#BigBlueButton

##1. Introduction

## 1.1. Project Overview
BigBlueButton is an open source web conferencing system for online learning.
It looks forward to help students and teachers to collaborate through a web platform. They may share audio, video, presentation (with whiteboard markup), chat and the presenter's desktop in real-time. The users can assume different roles according to their purpose: a **viewer** (student) can chat and send or receive audio and video; a **moderator** can mute or unmute other viewers, lock down viewers, or make anyone (including themselves) the **presenter** that can upload slides and annotate them for all to see.

## 1.2. Road Map
BigBlueButton's **Road Map** is largely driven by its target market: on-line learning. The focus of BBB is to the deliver a world-class product and provide the remote students a high quality learning experience. In order to achieve the proposed goals, BBB works on:
  * Stability - doing extensive testing for each release and providing a demo server for weeks without reboot
  * Usability - 
  * Modularity - 
  * Code Quality - 
  * Scalability - 
  * API - 

---Continuar----

## 1.3. Project Development

With the help of Denis Zgonjanin, an undergraduated student in Systems and Computer Engineering at Carleton, Richard implemented an early version of BigBlueButton using some open source components. 

After the early version, Richard, Denis and Fred Dixon became the core developers and launched the BigBlueButton 0.32. From this moment, it became an open source project.

The following figure illustrates the timeline between the 0.32 and the 0.61 versions.

![Timeline between 0.32 and 0.61 versions](images/time1.png)

Then the core developers created a demonstration at demo.bigbluebutton.org to enable anyone to try out the product, increasing the project's interest. Later, the core developers added desktop sharing and built-in VoIP. For easier usage and setup, they also created Ubuntu packages and a downloadable BigBlueButton VM.

![Timeline between 0.62 and 0.70 versions](images/time2.png)

After that, a proposal was made to add an application programming interface (API) to BigBlueButton for integration with 3rd party applications. Later on the development, the project started to have wikis, mailing lists, code repository and a growing community. Despite these efforts and improvements, BigBlueButton's growth and overall size were still relatively small - a boost was needed.

With the acceptance at Google Summer of Code, the project soon started to have a great receptivity and a newer version was launched with built-in whiteboard, making other open source projects to adopt BigBlueButton for integrated real-time collaboration.

![Timeline between 0.71 and beta-2 versions](images/time3.png)

At this moment the project did not have too much features and its simplicity was highly appreciated by universities and colleges. However, in terms of usability, the most pressing issue was the audio. A lot of work was done by the developers concerning the flow of packets and optimization of code, looking for ways to improve the built-in audio.

After solving this issue, the community suggested that BigBlueButton should have features like record and playback, but in order to do so, the architecture had to be redesigned to both capture events and process them for playback. The architecture rework began and the project was later used my Mozilla Foundation on the broadcasting and record of live classes.

The developers then released the 0.8 version and the record and playback was now available to the community, increasing the platform's main accesses and substantial improvements. The later version focused on upgrade these last features (record and playback), simplifying the interface and adding accessibility for students with disabilities.

![Timeline between beta-3 and RC1 versions](images/time4.png)

The project's last release is now the 0.9 version - the twelfth release - and is currently on the testing phase for the 1.0 release.
