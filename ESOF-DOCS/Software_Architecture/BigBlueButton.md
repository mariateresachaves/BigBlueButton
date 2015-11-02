#2. BigBlueButton Architecture

BigBlueButton is a complex system, that consist of many different components that are working together as one big network. 
##2.1 User Interaction With System (RTMP, HTTP, NGNIX)
The user interacts with the system through a web browser with **Flash Player** pre-installed. The BBB's interface is also done in Flash. The architects of BBB probably chose it because is one of those languages that allows very easly to send/receive audio and video streams.

When the user communicates with the system, this sends the request to the web server using **RTMP** or **HTTP** protocols. In the BBB system, **RTMP** is used to tranfer the video, audio and data using **Flash Player** from the user to the web server.  **HTTP** encapsulates the data in **RTMP** and tunnels it to the web server using porto 80. On the other end is a web server called **Nginx**.

**Nginx** plays a very important role as it sends the information received from the user to one of the two proxies: **bbb-web** or **bbb-aps**. The mission of **Nginx** is to guide **RTMP** requests to bbb-aps and **HHTP** to **bbb-web**.



<p align=center>
  <a href="https://github.com/mariateresachaves/bigbluebutton/blob/master/ESOF-DOCS/Software_Architecture/Software%20Architecture.md#1-software-architecture"><< Software Architecture </a>
  &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;
  <a href="https://github.com/mariateresachaves/bigbluebutton/blob/master/ESOF-DOCS/Software_Architecture/Index.md">Index</a>
  &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;
  <a href="https://github.com/mariateresachaves/bigbluebutton/blob/master/ESOF-DOCS/Software_Architecture/Logical%20View.md#3-logical-view">Logical View >></a>
</p>
