#2. BigBlueButton Architecture

BigBlueButton is a complex system, that consist of many different components that are working together as one big network. 
##2.1 User Interaction With System (RTMP, HTTP, NGNIX)
The user interacts with the system through a web browser with **Flash Player** pre-installed. The BBB's interface is also done in Flash. The architects of BBB probably chose it because is one of those languages that allows very easly to send/receive audio and video streams.

When the user communicates with the system, this sends the request to the web server using **RTMP** or **HTTP** protocols. In the BBB system, **RTMP** is used to tranfer the video, audio and data using **Flash Player** from the user to the web server.  **HTTP** encapsulates the data in **RTMP** and tunnels it to the web server using porto 80. On the other end is a web server called **Nginx**.

**Nginx** plays a very important role as it sends the information received from the user to one of the two proxies: **bbb-web** or **bbb-aps**. The mission of **Nginx** is to guide **RTMP** requests to bbb-aps and **HHTP** to **bbb-web**.

##2.2. bbb-web

As mentioned in the previous section, when the user communicates wih BBB interface, the information is sent to a web server, that then sends the information to one of two places: **bbb-web** or **bbb-apps**.

**bbb-web** is used for every type of data except audio or video. For example, is used to schedule conferences, login/logout, retrivieng/saving data to the database and upload data.

**bbb-web** is a **Grails** application which is a **Java**  based web-app framework.
**bbb-web** stants on top a **Tomcat** servelet container. It uses **SWFtools** to convert data, form example to convert pdf or png presentations that the presenter uploads into **swf** format, otherwise the users won't be able to see the presentations. The action in <a href="http://bigbluebutton.org/sites/all/videos/join/index.html"> **Video** </a> where the user uploads a presentation and is is seen on the website is done by **bbb-web** that receives a png or pdf file and converts it to a **flash swf** format.

To create thumbnails of the presentations, BBB uses tools like <a href="http://www.imagemagick.org/script/index.php"> **Imagemagic** </a> and <a href="https://en.wikipedia.org/wiki/Ghostscript"> **GhostScript** </a>. **Imagemagic** also plays an important role substituting **SwiftTools** in case this fails to convert a presentation. 

Another important tool is <a href="http://activemq.apache.org/"> **ActiveMQ** </a>, a messaging server that, through Java scripts, sends information about converting status with **bbb-web** and **bbb-aps**. It allows to track errors and to communicate between the two components.

##2.3. VoIP and Asteriks
The user can interact with the system also through <a href="https://en.wikipedia.org/wiki/Softphone/">  **softphone** </a>  using  <a href="https://en.wikipedia.org/wiki/Voice_over_IP/">  **VoIP** </a> or a regular phone line via <a href="https://en.wikipedia.org/wiki/Public_switched_telephone_network">  **PSTN** </a>. A voice signal is sent and it's receive by <a href="http://www.asterisk.org/">  **Asterik** </a> which is a free open-source communication server that allows to manipulate voice data. In the BBB software, the voice is passetd to <a href="https://blogs.reucon.com/asterisk-java/">  **Asterik-Java** </a> (bbb-web) and it's mostly used to check if the user is muted. If not, it sends the data to **bbb-apps** and with **Asterik-Java** the information is sent to the browser so the other users can listen to it.

##2.4. red5

##2.5. bbb-apps
------Continuar-------------


<p align=center>
  <a href="https://github.com/mariateresachaves/bigbluebutton/blob/master/ESOF-DOCS/Software_Architecture/Software%20Architecture.md#1-software-architecture"><< Software Architecture </a>
  &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;
  <a href="https://github.com/mariateresachaves/bigbluebutton/blob/master/ESOF-DOCS/Software_Architecture/Index.md">Index</a>
  &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;
  <a href="https://github.com/mariateresachaves/bigbluebutton/blob/master/ESOF-DOCS/Software_Architecture/Logical%20View.md#3-logical-view">Logical View >></a>
</p>
