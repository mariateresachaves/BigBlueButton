##2. BigBlueButton Requirements

##2.1. New Requirements

In the BigBlueButton community, the process of elicitation for new requirements works in a different way of the tipically used in software engineering. 
The **development team canvasses suggestions** for  new requirements in the **forum user community**. When someone from the development team finds a proposal worthwhile, they pitch a new issue in *Github*. The proposition has then to be **accepted by the project manager**. If this proposal entails major alterations to the project, the lead architect has to give his approval. In the event of being accepted, the new feature is added as a **milestone to the next release**.

Contrary to custom, the **requirements are designed by the developers**. While taking into consideration the users requests and suggestions, the development team is the one responsible for the discussion and documentation of how to implement, integrate the new feature and for the revision of the request. After everything has been outlined, the development phase can begin.

Below there's a schematic of the boundary between the requirements development and requirements management of this project.

<p align="center">
  <img src="images/requirementsManagement.png" width="500" height="350">
  <span class="caption">
        <p align="center"><b>Fig. 2</b> - Requirements Development and Management</p>
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

| Identifier | Name   |      Description    |
|:----------:|----------|-------------|
| R1 | Audio |  BBB should have audio for all users with no perceptual delay between them |
| R2 | Presentation |  Full-screen mode of the presentation, which includes notifications for new chat messages or of people joining in or out  |
| R3 | Whiteboard | For free drawings and annotations |
| R4 | File uploading | Various file formats can be uploaded (though .pdf is preferable), including video and audio types |
| R5 | Chat | Public and private chat |
| R6 | Desktop sharing | The presenter can share his desktop, if the viewers are interested |
| R7 | Polling | Various poll options like Yes/No, True/False, A/B/C/D or even custom ones |
| R8 | Emotion Icons | Display various emotions towards the presentation, including raising the hand |
| R9 | Different layouts | Various pre-set layouts for specific types of presentations, and also the possibility of customizing them |
| R10 | Video | For webcam video chat |
| R11 | Record and playback | It is possible to record a session for later playback and usage |
| R12 | Synchronized playback of external media | In case the presenter uploads a video or audio file, every user should see and hear the file at the same time. It would also be controlled by the presenter (when he wants to start, pause or stop the video)

##2.3. Critical Analysis

<!-- Problemas que tivemos em fazer o levantamento de requesitos, Técnicas usadas e porque que não usamos outras -->
As mentioned before, the requirements process in the BigBlueButton community is different from the usual process. There isn’t a client *per se*, but instead, the BBB goal is to deliver a  web conferencing system for online learning to a myriad of people, all with different necessities and purposes. Taking that into consideration, it’s easy to understand their different approach. This way, they are able to study the user's reactions and opinions of the new requirements. By being constantly supervising the forums they can make adjustments and respond to the different user’s necessities.    

However, this process isn’t perfect. The obvious problem is that, as they don’t do the follow up with the user who proposed the new feature, they have no idea what the user idealized for it. Also, they have to wait until a beta testing is released to get feedback from the users and to know if the new release is in accordance with what they had in mind and expected.    

Their **Road Map** is a way to cover the holes this process presents. Given that BigBlueButton was born in a university, they are well aware of the basic features expected from the users because, in the end, they are one of the target market.

In order to understand if the users were satisfied with BBB’s requirements management we posted on BBB user’s forum the following questions:  
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;*As an user, if you presented an idea for a new feature and it was accepted by the development team, does the end result met your expectations? If not, what alterations would you suggest?*  
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;*Are you satisfied with the way new requirements are presented to BBB, or would you like to be more involved in the design of the requisites for the new features?*

Unfortunately, we didn’t received any feedback and we were not able to get an immediate impression from the users.

To collect or discover new requirements we analysed **Questionnaires** and we found technical requirements such as: the number of participants must not exceed 150, depending if they are using webcam and or not, when feature X will be implemented, issues concerning with the desktop sharing, etc. We have also tried out **user interfaces** on BBB’s demo (e.g. menus, layouts, chatting room, webcam and audio, etc.) and we’ve collected some important requirements related with the platform’s basic features. Lastly, we’ve gone through various **scenarios**, **user stories** (which are provided on BBB’s documentation) and **use cases**. 

Since the access to developers is not easy we couldn't **meet** or have an **interview** to collect possible requirements. The same happens to **observing and analysing** how they actually work, making the documentation and the forum the only sources of information.

<p align=right>
  <a href="https://github.com/mariateresachaves/bigbluebutton/blob/master/ESOF-DOCS/Requirements/Index.md">Back to Index</a>
</p>
