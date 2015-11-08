#4. Implementation View
##4.1 Implementation View Introduction

The **Implementation View** consists  in one or more **Component Diagrams** representing the organization of the components of the system. Each diagram is used to model physical aspects of the system like executables, libraries, files or documents, by showing software components and the dependencies among them. **Apps-akka** is the main application that connects all the BigBlueButton's different applications together to provide real-time collaboration in the meeting, providing the list of users, chat, whiteboard and presentations in a meeting. **FsESL Akka** provides the voice conferencing capability in BigBlueButton. Preferably, users can join the conference using a headset and can obtain higher quality audio by joining through Mozilla Firefox or Google Chrome, which connects them via WebRTC. It also be integrated with VOIP providers so that users who are not able to join using the headset will be able to call in using their phone. The **HTML5 client** and **HTML5 server** are built using Meteor. **BBB-web** provides the integration endpoint for third-party applications to control the BigBlueButton server. BigBlueButton integrates Moodle, Wordpress, Canvas, Sakai, and other third-party integrations, allowing teachers to setup BigBlueButton rooms within their course and students to access the rooms and their recordings.

The main purposes of component diagrams are:

* Visualize the components of a system.
* Describe the organization and relationships of the components.

##4.2 UML Component Diagram

As stated in section 2, the **Client** is a Flash application which runs inside the the user's browser and connects to Red5 using RTMP  or HTTP protocols. The last one tunnels the data to <a href="https://en.wikipedia.org/wiki/Nginx"> **Nginx** </a>.  **Red5** is the media server that suports live video streaming and works as an intermediate between the **client** and **apps-akka** 
<p align="center">
  <img src="https://github.com/mariateresachaves/bigbluebutton/blob/master/ESOF-DOCS/Software_Architecture/images/component_diagram_1.png">
  <span class="caption">
        <p align="center"><b>Fig. 1</b> - Component Diagram</p>
        </span>
</p>

//falta descrição de cada ponto.
//to be continued...

<p align=center>
  <a href="https://github.com/mariateresachaves/bigbluebutton/blob/master/ESOF-DOCS/Software_Architecture/Logical%20View.md#3-logical_view"><< Logical View</a>
  &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;
  <a href="https://github.com/mariateresachaves/bigbluebutton/blob/master/ESOF-DOCS/Software_Architecture/Index.md">Index</a>
  &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;
  <a href="https://github.com/mariateresachaves/bigbluebutton/blob/master/ESOF-DOCS/Software_Architecture/Deployment%20View.md">Deployment View >></a>
</p>
