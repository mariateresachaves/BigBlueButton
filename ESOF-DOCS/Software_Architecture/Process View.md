#6. Process View

##6.1. Process View Introduction
To provide a basis for understanding the process organization of the system, sotware architecture uses a view called the **Process View**. This view deals with the dynamic aspects of the system, explains the system processes and how they communicate, and focuses on the runtime behavior of the system. The process view addresses concurrency, distribution, integrators, performance, and scalability and others. UML Diagrams to represent a process view include **sequence** diagrams. 

##6.2. Sequence Diagram

There are several involved servers for fulfilling the requests from the **Client**. The sequence of the exchanged messages to *Join a Meeting* is described below.

<p align="center">
  <img src="https://github.com/mariateresachaves/bigbluebutton/blob/master/ESOF-DOCS/Software_Architecture/images/process_view.png">
  <span class="caption">
        <p align="center"><b>Fig. 14</b> - Activities Sequence Diagram</p>
        </span>
</p>


The coordinator is the **Management Server** (MS). The MS server’s message exchange with the BBB server should be either through BigBlueButton’s API (e.g. getMeeting, create and join meeting API calls) or by using Red5’s Remote Shared Objects (e.g. the “meeting destroyed” message).


<p align=center>
  <a href="https://github.com/mariateresachaves/bigbluebutton/blob/master/ESOF-DOCS/Software_Architecture/Deployment%20View.md"><< Deployment View</a>
  &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;
  <a href="https://github.com/mariateresachaves/bigbluebutton/blob/master/ESOF-DOCS/Software_Architecture/Index.md">Index</a>
  &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;
</p>
