#Open Source Project Study - BigBlueButton

##Overview

BigBlueButton is an open source web conferencing system for online learning.
It looks forward to help students and teachers to collaborate through a web platform. They may share audio, video, presentation (with whiteboard markup), chat and the presenter's desktop in real-time. The users can assume different roles according to their purpose: a **viewer** (student) can chat and send or receive audio and video; a **moderator** can mute or unmute other viewers, lock down viewers, or make anyone (including themselves) the **presenter** that can upload slides and annotate them for all to see.

##Table of Contents        

####The Development Software Process
[1. Introduction](https://github.com/mariateresachaves/bigbluebutton/blob/master/ESOF-DOCS/Initial-Report/Introduction.md#1-introduction)     
&nbsp;&nbsp;&nbsp;&nbsp;[1.1. Project Overview](https://github.com/mariateresachaves/bigbluebutton/blob/master/ESOF-DOCS/Initial-Report/Introduction.md#11-project-overview)  
&nbsp;&nbsp;&nbsp;&nbsp;[1.2. Road Map](https://github.com/mariateresachaves/bigbluebutton/blob/master/ESOF-DOCS/Initial-Report/Introduction.md#12-road-map)    
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[1.2.1. Core Features](https://github.com/mariateresachaves/bigbluebutton/blob/master/ESOF-DOCS/Initial-Report/Introduction.md#121-core-features)  
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[1.2.2. General Requirements](https://github.com/mariateresachaves/bigbluebutton/blob/master/ESOF-DOCS/Initial-Report/Introduction.md#122-general-requirements)  
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[1.2.3. Clients](https://github.com/mariateresachaves/bigbluebutton/blob/master/ESOF-DOCS/Initial-Report/Introduction.md#123-clients)   
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[1.2.4. Areas for investigation](https://github.com/mariateresachaves/bigbluebutton/blob/master/ESOF-DOCS/Initial-Report/Introduction.md#124-areas-for-investigation)  
&nbsp;&nbsp;&nbsp;&nbsp;[1.3. Project Development](https://github.com/mariateresachaves/bigbluebutton/blob/master/ESOF-DOCS/Initial-Report/Introduction.md#13-project-development)  
[2. Development Process](https://github.com/mariateresachaves/bigbluebutton/blob/master/ESOF-DOCS/Initial-Report/Development%20Process.md#2-development-process)  
&nbsp;&nbsp;&nbsp;&nbsp;[2.1. Incremental Process](https://github.com/mariateresachaves/bigbluebutton/blob/master/ESOF-DOCS/Initial-Report/Development%20Process.md#21-incremental-process)  
&nbsp;&nbsp;&nbsp;&nbsp;[2.2. Advantages and disadvantages](https://github.com/mariateresachaves/bigbluebutton/blob/master/ESOF-DOCS/Initial-Report/Development%20Process.md#22-advantages-and-disadvantages)  
[3. Critical Analysis](https://github.com/mariateresachaves/bigbluebutton/blob/master/ESOF-DOCS/Initial-Report/Critical%20Analysis.md#3-critical-analysis)  
&nbsp;&nbsp;&nbsp;&nbsp;[3.1. Current state](https://github.com/mariateresachaves/bigbluebutton/blob/master/ESOF-DOCS/Initial-Report/Critical%20Analysis.md#31-current-state)  
&nbsp;&nbsp;&nbsp;&nbsp;[3.2. Positive Aspects](https://github.com/mariateresachaves/bigbluebutton/blob/master/ESOF-DOCS/Initial-Report/Critical%20Analysis.md#32-positive-aspects)  
&nbsp;&nbsp;&nbsp;&nbsp;[3.3. Enhancements](https://github.com/mariateresachaves/bigbluebutton/blob/master/ESOF-DOCS/Initial-Report/Critical%20Analysis.md#33-enhancements)
    
####Requirements
[4. Requirements Engineering](https://github.com/mariateresachaves/bigbluebutton/blob/master/ESOF-DOCS/Requirements/Requirements%20Engineering.md#1-requirements-engineering)  
&nbsp;&nbsp;&nbsp;&nbsp;[4.1. Description](https://github.com/mariateresachaves/bigbluebutton/blob/master/ESOF-DOCS/Requirements/Requirements%20Engineering.md#11-description)  
&nbsp;&nbsp;&nbsp;&nbsp;[4.2. Techniques](https://github.com/mariateresachaves/bigbluebutton/blob/master/ESOF-DOCS/Requirements/Requirements%20Engineering.md#12-techniques)  
&nbsp;&nbsp;&nbsp;&nbsp;[4.3. Stakeholders](https://github.com/mariateresachaves/bigbluebutton/blob/master/ESOF-DOCS/Requirements/Requirements%20Engineering.md#13-stakeholders)    
&nbsp;&nbsp;&nbsp;&nbsp;[4.4. Inappropriate Requirements](https://github.com/mariateresachaves/bigbluebutton/blob/master/ESOF-DOCS/Requirements/Requirements%20Engineering.md#14-inappropriate-requirements)    
[5. BigBlueButton Requirements](https://github.com/mariateresachaves/bigbluebutton/blob/master/ESOF-DOCS/Requirements/BigBlueButton%20Requirements.md#2-bigbluebutton-requirements)  
&nbsp;&nbsp;&nbsp;&nbsp;[5.1. New Requirements](https://github.com/mariateresachaves/bigbluebutton/blob/master/ESOF-DOCS/Requirements/BigBlueButton%20Requirements.md#21-new-requirements)  
&nbsp;&nbsp;&nbsp;&nbsp;[5.2. Requirements Analysis](https://github.com/mariateresachaves/bigbluebutton/blob/master/ESOF-DOCS/Requirements/BigBlueButton%20Requirements.md#22-requirements-analysis)  
&nbsp;&nbsp;&nbsp;&nbsp;[5.3. Critical Analysis](https://github.com/mariateresachaves/bigbluebutton/blob/master/ESOF-DOCS/Requirements/BigBlueButton%20Requirements.md#23-critical-analysis)  
[6. Requirements Specification](https://github.com/mariateresachaves/bigbluebutton/blob/master/ESOF-DOCS/Requirements/Requirements%20Specification.md#3-requirements-specification)  
&nbsp;&nbsp;&nbsp;&nbsp;[6.1. Requirements Overview](https://github.com/mariateresachaves/bigbluebutton/blob/master/ESOF-DOCS/Requirements/Requirements%20Specification.md#31-requirements-specification)  
&nbsp;&nbsp;&nbsp;&nbsp;[6.2. Use Case Diagram](https://github.com/mariateresachaves/bigbluebutton/blob/master/ESOF-DOCS/Requirements/Requirements%20Specification.md#32-use-case-diagram)  
[7. Domain Model](https://github.com/mariateresachaves/bigbluebutton/blob/master/ESOF-DOCS/Requirements/Domain%20Model.md#4-domain-model)  


####Software Architecture
[8. Software Architecture](https://github.com/mariateresachaves/bigbluebutton/blob/master/ESOF-DOCS/Software_Architecture/Software%20Architecture.md#1-software-architecture)  
&nbsp;&nbsp;&nbsp;&nbsp;[8.1. Overview](https://github.com/mariateresachaves/bigbluebutton/blob/master/ESOF-DOCS/Software_Architecture/Software%20Architecture.md#11-overview)  
&nbsp;&nbsp;&nbsp;&nbsp;[8.2. 4+1 View Model](https://github.com/mariateresachaves/bigbluebutton/blob/master/ESOF-DOCS/Software_Architecture/Software%20Architecture.md#12-4--1-view-model)  
[9. BigBlueButton](https://github.com/mariateresachaves/bigbluebutton/blob/master/ESOF-DOCS/Software_Architecture/BigBlueButton.md#2-bigbluebutton-architecture)  
&nbsp;&nbsp;&nbsp;&nbsp;[9.1. User Interaction with the System (RTMP, HTTP, NGNIX)](https://github.com/mariateresachaves/bigbluebutton/blob/master/ESOF-DOCS/Software_Architecture/BigBlueButton.md#21-user-interaction-with-the-system-rtmp-http-ngnix)  
&nbsp;&nbsp;&nbsp;&nbsp;[9.2. bbb-web](https://github.com/mariateresachaves/bigbluebutton/blob/master/ESOF-DOCS/Software_Architecture/BigBlueButton.md#22-bbb-web)  
&nbsp;&nbsp;&nbsp;&nbsp;[9.3. VoIP and Asterik](https://github.com/mariateresachaves/bigbluebutton/blob/master/ESOF-DOCS/Software_Architecture/BigBlueButton.md#23-voip-and-asterik)  
&nbsp;&nbsp;&nbsp;&nbsp;[9.4. red5](https://github.com/mariateresachaves/bigbluebutton/blob/master/ESOF-DOCS/Software_Architecture/BigBlueButton.md#24-red5)  
&nbsp;&nbsp;&nbsp;&nbsp;[9.5. bbb-apps](https://github.com/mariateresachaves/bigbluebutton/blob/master/ESOF-DOCS/Software_Architecture/BigBlueButton.md#25-bbb-apps)  
[10. Logical View](https://github.com/mariateresachaves/bigbluebutton/blob/master/ESOF-DOCS/Software_Architecture/Logical%20View.md#3-logical_view)  
&nbsp;&nbsp;&nbsp;&nbsp;[10.1. Logical View Introduction](https://github.com/mariateresachaves/bigbluebutton/blob/master/ESOF-DOCS/Software_Architecture/Logical%20View.md#31-logical-view-introduction)  
&nbsp;&nbsp;&nbsp;&nbsp;[10.2. UML Package Diagram](https://github.com/mariateresachaves/bigbluebutton/blob/master/ESOF-DOCS/Software_Architecture/Logical%20View.md#32-uml-package-diagram)  
[11. Implementation View](https://github.com/mariateresachaves/bigbluebutton/blob/master/ESOF-DOCS/Software_Architecture/Implementation%20View.md#4-implementation_view)  
&nbsp;&nbsp;&nbsp;&nbsp;[11.1. Implementation View Introduction](https://github.com/mariateresachaves/bigbluebutton/blob/master/ESOF-DOCS/Software_Architecture/Implementation%20View.md#41-implementation-view-introduction)   
&nbsp;&nbsp;&nbsp;&nbsp;[11.2. UML Components Diagram](https://github.com/mariateresachaves/bigbluebutton/blob/master/ESOF-DOCS/Software_Architecture/Implementation%20View.md#42-uml-component-diagram)  
[12. Deployment View](https://github.com/mariateresachaves/bigbluebutton/blob/master/ESOF-DOCS/Software_Architecture/Deployment%20View.md#5-deployment_view)  
&nbsp;&nbsp;&nbsp;&nbsp;[12.1. Deployment View Introduction](https://github.com/mariateresachaves/bigbluebutton/blob/master/ESOF-DOCS/Software_Architecture/Deployment%20View.md#51-deployment-view-introduction)   
&nbsp;&nbsp;&nbsp;&nbsp;[12.2. UML Deployment Diagram](https://github.com/mariateresachaves/bigbluebutton/blob/master/ESOF-DOCS/Software_Architecture/Deployment%20View.md#52-uml-deployment-diagram)  
[13. Process View](https://github.com/mariateresachaves/bigbluebutton/blob/master/ESOF-DOCS/Software_Architecture/Process%20View.md#6-process_view)    


####Software Testing
[14. Software Testing](https://github.com/mariateresachaves/bigbluebutton/blob/master/ESOF-DOCS/Testability/Software_Testability.md#1-software-testability)  
&nbsp;&nbsp;&nbsp;&nbsp;[14.1. Overview](https://github.com/mariateresachaves/bigbluebutton/blob/master/ESOF-DOCS/Testability/Software_Testability.md#11-overview)

