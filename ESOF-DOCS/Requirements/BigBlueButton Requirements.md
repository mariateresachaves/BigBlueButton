##2. BigBlueButton Requirements

##2.1. New Requirements

In the BigBlueButton community, the process of elicitation for new requirements works in a different way of the tipically used in software engineering. 
The **development team canvasses suggestions** for  new requirements in the **forum user community**. When someone from the development team finds a proposal worthwhile, they pitch a new issue in *Github*. The proposition has then to be **accepted by the project manager**. If this proposal entails major alterations to the project, the lead architect has to give his approval. In the event of being accepted, the new feature is added as a **milestone to the next release**.

Contrary to custom, the **requirements are designed by the developers**. While taking into consideration the users requests and suggestions, the development team is the one responsible for the discussion and documentation of how to implement, integrate the new feature and for the revision of the request. After everything has been outlined, the development phase can begin.

Below there's a schematic of the boundary between the requirements development and requirements management of this project.

<p align="center">
  <img src="images/requirementsManagement.png" width="500" height="350">
  <span class="caption">
        <p align="center"><b>Fig. 1</b> - Requirements Development and Management</p>
        </span>
</p>

The choice of development for new features in the new release is decided by the core development team. 
When planning a release, they look at the outstanding issues in the following order:
* What are the most important items on the BBB road map?
* What refactoring/features do the core committers believe are necessary to improve the code base/maintainability/usability of the product?
* What features are the community asking to implement (process described above)?

For that reason there are features, like the whiteboard, that were implemented immediately, but others, like the polling, took several years to be developed because there were more immediate priorities.
 
##2.2. Specification

<!-- Descrever os requesitos -->

The purpose of BigBlueButton is to bring access an high-quality online learning experience to every student with a web browser. There will be 3 kinds of users: 1) the *viewers*, who will usually be the students; 2) the professors or *presenters* who will be teaching; 3) the *moderators*, who will be in charge of maintaining the overall welfare of the presentation. In order to do this, certain requirements were needed for BigBlueButton to be able to achieve its purpose. 

* The *viewers* have to be able to get a clean and sleek interface, so that they can easily interact with the application. They also need means to participate in a presentation, whether if he wants to have a more laid-back, passive attitude (by giving means of just be able to listen and view the presentations, *Fig.2*) or a more active participation by providing the viewer with chat possibilities *(Fig.3)* and also to interact with the presenter and the presentation itself, by showing if the viewer is content, confused or wants to raise his hand to participate *(Fig.4)*.

<p align="center">
  <img src="https://github.com/mariateresachaves/bigbluebutton/blob/master/ESOF-DOCS/Requirements/images/screen1.png" width="450" height="350">
  <span class="caption">
        <p align="center"><b>Fig. 2</b> - Initial choice for speaking or listening only</p>
        </span>
</p>

<p align="center">
  <img src="https://github.com/mariateresachaves/bigbluebutton/blob/master/ESOF-DOCS/Requirements/images/screen5.png" width="450" height="350">
  <span class="caption">
        <p align="center"><b>Fig. 3</b> - Viewer can chat with the public, for all to see (left) or he can choose someone to private chat with (right)</p>
        </span>
</p>

<p align="center">
  <img src="https://github.com/mariateresachaves/bigbluebutton/blob/master/ESOF-DOCS/Requirements/images/screen7.png" width="250" height="350">
  <span class="caption">
        <p align="center"><b>Fig. 4</b> - Viewer can signal various emotions, in this case, the viewer is confused with the presentation</p>
        </span>
</p>




* The *presenters* need to be able to easily transmit their knowledge to the viewers, whether by chat, audio and/or video messages, or even with the possibility of desktop sharing *(Fig.5)*. It is also imperative to give them the possibility to upload demonstrative files of the subject they are presenting to help contextualizing, and also to edit them in real-time, in the case they want to make some extra annotations or to emphasize some particular detail in their uploads *(Fig.6)*. The polling option is also available, which can be useful for interactive exercises with the audience *(Fig.7)*.

<p align="center">
  <img src="https://github.com/mariateresachaves/bigbluebutton/blob/master/ESOF-DOCS/Requirements/images/screen6.png" width="670" height="295">
  <span class="caption">
        <p align="center"><b>Fig. 5</b> - As a presenter, one can enable/disable own audio and video and share his desktop with any person he sees fit</p>
        </span>
</p>

<p align="center">
  <img src="https://github.com/mariateresachaves/bigbluebutton/blob/master/ESOF-DOCS/Requirements/images/screen2.png" width="415" height="350">
  <span class="caption">
        <p align="center"><b>Fig. 6</b> - The presenter can write anything over the slides he uploaded. He also has options to draw squares, rectangles or even free drawings</p>
        </span>
</p>

<p align="center">
  <img src="https://github.com/mariateresachaves/bigbluebutton/blob/master/ESOF-DOCS/Requirements/images/screen9.png" width="415" height="350">
  <span class="caption">
        <p align="center"><b>Fig. 7</b> - Various polls can be done, including with custom choice options</p>
        </span>
</p>

* The *moderators* have to be able to choose who they want the presenter to be *(Fig.8)*, and giving them their respective capabilities. They also need to be able to mute and unmute both the viewers and presenters, to avoid various situations like many users talking at the same time, or background noise from a specific user. They also need to get the possibility to lock down a user, for example, in a case where this user shows abusive behavior. *(Fig.9)* In addition, he can also see the displayed reactions of the viewers, which will always appear at the top of the users list and act upon them *(Fig.10)*.

<p align="center">
  <img src="https://github.com/mariateresachaves/bigbluebutton/blob/master/ESOF-DOCS/Requirements/images/screen4.png" width="675" height="405">
  <span class="caption">
        <p align="center"><b>Fig. 8</b> - The moderator can make someone the new presenter (including himself)</p>
        </span>
</p>

<p align="center">
  <img src="https://github.com/mariateresachaves/bigbluebutton/blob/master/ESOF-DOCS/Requirements/images/screen8.png" width="670" height="295">
  <span class="caption">
        <p align="center"><b>Fig. 9</b> - The moderator can mute/unmute and lock other users</p>
        </span>
</p>

<p align="center">
  <img src="https://github.com/mariateresachaves/bigbluebutton/blob/master/ESOF-DOCS/Requirements/images/screen3.png" width="675" height="405">
  <span class="caption">
        <p align="center"><b>Fig. 10</b> - The moderator/presenter will see, at the top of the list, if any user asks for permission to intervene in the presentation. He can then unmute or turn video chat on</p>
        </span>
</p>

##2.3. Requirements Analysis

<!-- Tabela com os requisitos + características -->

| Name   |      Description    |
|----------|:-------------:|
| Audio |  BBB should have audio for all users with no perceptual delay between them |
| Presentation |  Full-screen mode of the presentation, which includes notifications for new chat messages or of people joining in or out  |
| Whiteboard | For free drawings and annotations |
| Chat | Public and private chat |
| Desktop sharing | The presenter can share his desktop, if the viewers are interested |
| Polling | Various poll options like Yes/No, True/False, A/B/C/D or even custom ones |
| Breakout Rooms | Group various viewers in a room for an activity, in private |
| Shared Notes | Users in a room can collaborate in creating a document |
| Video | For webcam video chat |
| Record and playback | It is possible to record a session for later playback and usage |
| Synchronized playback of external media | In case the presenter uploads a video or audio file, every user should see and hear the file at the same time. It would also be controlled by the presenter (when he wants to start, pause or stop the video)

##2.4. Critical Analysis

<!-- Problemas que tivemos em fazer o levantamento de requesitos, Técnicas usadas e porque que não usamos outras -->
