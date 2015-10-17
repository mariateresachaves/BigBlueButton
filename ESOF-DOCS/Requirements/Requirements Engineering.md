##1. Requirements Engineering

<!-- serve só para contextualizar -->

##1.1. Description

Software development begins by specifying the respective project requirements. These are statements that describe what the system must do, how it must behave, the properties it must exhibit, the qualities it must possess, and the constraints that the system and its development must satisfy. Requirements engineering emphasizes the use of systematic and repeatable techniques that ensure the completeness, consistency, and relevance of the system requirements. 

The *IEEE* defines a requirement as:    

1. a condition or capability needed by a user to solve a problem or achieve an objective,
2. a condition or capability that must be met or possessed by a system or system component to satisfy a contract, standard, specification, or other formally imposed document,
3. a documented representation of a condition or capability as in definition 1 or 2.    
*[Institute of Electrical and Electronic Engineers. IEEE Standard Glossary of Software Engineering Terminology (IEEE Std 610.12-1990). New York, NY: Institute of Electrical and Electronics Engineers, 1990.]*


Requirements engineering comprises the following:
* **Requirements elicitation:** is the process of discovering, reviewing, documenting, and understanding the user's needs and constraints for the system.
* **Requirements analysis:** is the process of refining the user's needs and constraints.
* **Requirements specification:** is the process of documenting the user's needs and constraints clearly and precisely.
* **Requirements verification:** is the process of ensuring that the system requirements are complete, correct, consistent, and clear.
* **Requirements management:** is the process of scheduling, coordinating, and documenting the requirements engineering activities (that is, elicitation, analysis, specification, and verification).

<img src="https://github.com/mariateresachaves/bigbluebutton/blob/master/ESOF-DOCS/Requirements/images/requirements_new.png" width="800" height="400">

Requirements engineering is very complex because of the three roles involved in producing even a single requirement,
the **user**, the **developer** (who will design and implement the system), and the **author** (who will document the requirements). Requirements address a fundamental communications problem. This problem ir further complicated by the number and diversity of system users. In practice, any system stakeholder has needs and expectations, i.e. requirements, for the system.  The clear definition of the requirements is of vital importance because of their pervasive quality. They continuously affect the development and maintenace phases throughout a system's development. For example, in the testing phase, the requirements provide a quality statement in wich is possible to define the standard of correctness against which to test.

##1.2. Techniques

In order to collect/discover their requirements there are useful **techniques** that help to clarify what the client really wants:

* **Interviews:** various issues are explored with stakeholders, or is based on a pre-determined list of questions or mixing both;

* **Facilitated meetings (brainstorming, focus groups, etc.)**:
      * **Brainstorming** is a method of quickly generating many creative ideas from a group of people.
      * **A focus group** is an interactive session with a carefully selected group of people designed to capitalize on the synergy of a group. The focus group report records of what was learned, including both agreements and disagreements among the participants.

* **Surveys/Questionnaires:** Surveys allow you to collect information from many people in a relatively short period. A survey can be an effective way to collect quantitative information; however, writing the questions requires great skill and care to avoid ambiguity that could compromise the utility of the results.

* **Goal analyses:** Goal analysis comprehends the exploration of information sources for goal identification followed by organization and classification of goals, namely:
      * Explore the available information;
      * Identify activities, such as identifying stakeholders, identifying agents and their responsibilities from the information provided by the previous explore activities;
      * Organize activities and organize goals according to goal dependency relations.

* **Social observation and analysis** - Observation is watching people as they go about their jobs. Observation can be an effective way to gain a realistic and detailed understanding of how work is done in the production environment; however, it is time consuming and may disrupt work.

* **(User-interface) Prototypes:** An initial version of a system which is available early so that the users can experiment with the system and point out its strengths and weaknesses of the implemented requirements.

* **Scenarios, user stories, use cases (real-life usage examples):** A use case describes a scenario in which a user interacts with the system being defined to achieve a specific goal or accomplish a particular task. Use cases are described in terms of the user's work terminology, not computerese. By focusing on essential use cases, stripped of implementation constraints or alternatives, the analyst can derive software requirements that will enable the user to achieve his objectives in each specific usage scenario. 


##1.3. Stakeholders

The role of system stakeholder is played by any of the various people or systems involved in or affected by a system's development. This group includes:
* **executives**: (who know the organization's business goals and constraints);
* **end users** (who know how the products will be used);
* **marketers** (who know the market demands);
* **technical managers** (who know the available personnel);
* **developers** (who know the available tools and technology). 

The success of requirements engineering depends on the identification and solicitation of the appropriate community of stakeholders. Reconciling the diverse needs and expectations of the various system stakeholders necessitates tradeoffs,this means, decisions have to be made to sort out potentially conflicting requirements from different stakeholders.

##1.4. Inappropriate requirements

The failure to capture the right requirements is the major risk with requirements engineering. If the requirements are in any way compromised they will be unable to produce systems that satisfy the customers and fulfill the market expectations. 
Inappropriate requirements can result from the following:
    
* **Insufficient generality:** Insufficient generality in the requirements leads to a design that is too brittle to deal with the change actually experienced over the lifetime of the software.    

* **Excessive generality:** Overly general requirements lead to excessive effort in producing both core assets (to provide that generality) and specific products (which must turn that generality into a specific instantiation).    

* **Wrong variation points:** Incorrect determination of the variation points, results in inflexible software and the inability to respond rapidly to customer needs and market shifts.    

* **Failure to account for qualities other than behavior:** Software requirements should capture requirements for quality attributes such as performance, reliability, and security.

