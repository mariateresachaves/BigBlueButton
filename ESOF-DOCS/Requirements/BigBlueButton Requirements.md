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
 

##2.2. Requirements Analysis

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

##2.3. Critical Analysis

<!-- Problemas que tivemos em fazer o levantamento de requesitos, Técnicas usadas e porque que não usamos outras -->
