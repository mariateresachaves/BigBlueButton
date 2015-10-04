# 2. Development Process

## 2.1. Incremental Process

BigBlueButton it's a project comprised of a continuously growing community where developers, users, educational institutions, and commercial companies are all collaborating towards a more sophisticated software, but always bearing in mind the quality of the product. For that purpose, one of the main priorities taken in consideration when choosing the development process, was stability. To achieve the desired stability, BigBlueButton designed a development process based on multiple releases, wherein each step is built in a Waterfall cycle. To further guarantee the stability provided by the software, months are spent testing each release candidate before issueing a release. The motto of the BigBlueButton development process is *Release on quality, not dates*.

The development process is structured in 6 steps:

1. Planning
2. Design
3. Development
4. Beta Testing
5. Release Candidate
6. General Release

<img src="http://agile-development-tools.com/wp-content/uploads/2010/10/iterative-development1.png">

During the **planning** phase, the committers decide the main features to be added for the new release by reviewing the BigBlueButton Road Map and all issues concerned with stability and usability. 
After outline the plan for the new release, the next phase starts, the **design** phase, when each feature is assigned a Issue Tracker. This allows the community to track the progress of the project and consists on a recorded of the defects and enhancements made during the new release.

After laid out the plan and desing, the **development** phase can begin. During this time, the commiters hold usually bi-weekly meetings to discuss the development of the project. Each commiter works on a fork of the BigBlueButton Master provided by *Github*. When a new feature is ready to be committed, the committer sends a pull request to merge the work into the Master branch. The merging is then reviewed by another committer who is familiar with that specific area of the product. Any major change has to be reviewed by the BigBlueButton's CTO (*Chief technology officer*) and the person responsible for that pull request has to provid documentation to facilitate the reviewers work. The work of the reviewrs is very important to maintain the two first priorities of the development of BigBlueButton, stability and usability, and if the pull request doesn't meet the expectations and will affect adversely with one of these priorities, it will be denied. If it is approved, the new feature is tested by the developers in the latest build. 

The **Beta Testing** phase starts after the core development is finished, all the obvius bugs are fixed and documentation for the release, installation and setting up the development enviroment is provided. During this phase, all the BigBlueButton community has access to the new features and there will be several beta testings until the community stops reporting major bugs. Also at this stage, the documentation is reviewed and the installation package is updated to correct any errors that may occur in the upgrade from the previous version. Finnaly, a *Release Candidate* is submitted. During this phase the core commiters supervise the mailing lists, twitter and the response of the members for any bug that will impact the general release. After fixing the issues, a new release candidate is provided. Each release candidate can last up to a month. If in a period of two weeks, no new issue is reported for the last release candidate, the **general release** is announced by the committers.

## 2.2. Advantages and disadvantages

One of the main advantages of this process in comparison with the Waterfall process, lies in the fact that, the last one will only have some commercial value when the project ends, as there is nothing pratical to be presented before this stage. The incremental process makes it possible to initially have a prototype of the project, verify the received feedback and some possible ajustments to be made, and continue to develop it based on this experience. By doing this process in a cyclical way, we guarantee that it goes according to project's target audience, and that when the final version is launched, it will be complete, with all the necessary ajustments already made.

The incremental process it's not agile compared to other development processes often used in open source projects. After the planning and designing of each release and the starting of the development stage, this process doesn't allow any changes to the previously agreed issues. It's necessary to wait to a future realese to add any new ideas to the project.
Usually the structural integrity of the code starts to crumble, and with each new addition the code can start to be obsolete.
