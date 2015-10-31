#1. Software Architecture 

##1.1. Overview

Software architecture is the process of building a structured solution of **what** features are needed and **how** the system must behave (*Fig.1*). In order to do that, usually there is a software architect which leads a team of developers and engineers, making sure all the pieces come together to make fully functioning software.

<p align="center">
  <img src="images/softwareArchitecture.png" width="35%" height="35%">
  <span class="caption">
        <p align="center"><b>Fig. 1</b> Software Architecture</p>
  </span>
</p>

<br>

<table border="2px">
  <td>A classic definition for <strong>Software Architecture</strong> according to <i>IEEE</i> is:<br><br>
  &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;" Software Architecture is the fundamental organization of a <strong>system</strong>, embodied in its <strong>components</strong>, their <strong>relationships</strong> to each other and the <strong>environment</strong>, and the principles governing its design and evolution. "</td>
</table>

<br>

In other words, the architecture will include how the system is separated in modules/packages, the way how they will interact with each other and everything the system interacts with, in order to be achieved the desired structured architecture. If this is fulfilled it's easier to change it when new requirements come up, unlike other architectures which are constantly in change due to design errors. To minimize the probability of falling into this error there are aspects as performance, security, safety, availability, maintainability and portability (*Fig.2*) to ensure that the software system is well structured.

<p align="center">
  <img src="images/softwareArchitectureAspects.png" width="45%" height="45%">
  <span class="caption">
        <p align="center"><b>Fig. 2</b> Software Architecture aspects</p>
  </span>
</p>

##1.2. 4+1 View Model

This model allows the various [Stakeholders](https://github.com/mariateresachaves/bigbluebutton/blob/master/ESOF-DOCS/Requirements/Requirements%20Engineering.md#13-stakeholders) to find what they want to know about the software architecture. Systems engineers approach it from the Physical View, then the Process View. End-users, customers, data specialists from the Logical View. Project managers, software configuration staff see it from the Development View.

<p align="center">
  <img src="images/4p1ViewModel.png" width="40%" height="40%">
  <span class="caption">
        <p align="center"><b>Fig. 3</b> 4+1 View Model</p>
  </span>
</p>

As shown in the previous image (*Fig.3*), this model is composed by Logical View, Implementation View, Deployment View, Process View and Use Case View. Below there's a brief definition for each one of the Views:  
  * **Logical View** - shows the key abstractions in the system as objects or object classes, or their packages;

  <p align="center">
    <img src="images/packageDiagram.png" width="30%" height="30%">
    <span class="caption">
          <p align="center"><b>Fig. 4</b> Example of Logical View (UML package diagram)</p>
    </span>
  </p>

  * **Implementation View** - shows how the software is decomposed (into software components) for development;
   
  <p align="center">
    <img src="images/componentDiagram.png" width="50%" height="50%">
    <span class="caption">
          <p align="center"><b>Fig. 5</b> Example of Implementation View (UML component diagram)</p>
    </span>
  </p>

  * **Deployment View** - shows the system hardware and how software components are distributed across the hardware nodes;

  <p align="center">
    <img src="images/deploymentDiagram.png" width="50%" height="50%">
    <span class="caption">
          <p align="center"><b>Fig. 6</b> Example of Deployment View (UML deployment diagram)</p>
    </span>
  </p>

  * **Process View** - shows how, at run-time, the system is composed of interacting processes;

  <p align="center">
    <img src="images/activityDiagram.png" width="50%" height="50%">
    <span class="caption">
          <p align="center"><b>Fig. 7</b> Example of Process View (UML activity diagram)</p>
    </span>
  </p>

  * **Use Case View (+1)** - Relates the other views.

  <p align="center">
    <img src="images/useCaseDiagram.png" width="40%" height="40%">
    <span class="caption">
          <p align="center"><b>Fig. 7</b> Example of Process View (UML activity diagram)</p>
    </span>
  </p>

<!-- FOOTER -->

<p align=center>
  <a href="https://github.com/mariateresachaves/bigbluebutton/blob/master/ESOF-DOCS/Requirements/Requirements%20Engineering.md"><< Requirements</a>
  &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;
  <a href="https://github.com/mariateresachaves/bigbluebutton/blob/master/ESOF-DOCS/Software_Architecture/Index.md">Index</a>
  &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;
  <a href="https://github.com/mariateresachaves/bigbluebutton/blob/master/ESOF-DOCS/Software_Architecture/BigBlueButton.md">BigBlueButton Architecture >></a>
</p>
