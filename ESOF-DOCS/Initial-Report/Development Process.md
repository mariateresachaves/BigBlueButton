# 2. Development Process

## 2.1. Incremental Process

BigBlueButton is a project comprised of a continuously growing community where developers, users, educational institutions, and commercial companies are all collaborating towards a more sophisticated software, but always bearing in mind the quality of the product. For that purpose, one of the main priorities taken into consideration when choosing the development process, was stability. To achieve this, BigBlueButton designed a development process based on multiple releases, wherein each step is built in a Waterfall cycle. To further guarantee provided software stability, months are spent testing each release candidate before issuing a release. The motto of BigBlueButton development process is *Release on quality, not dates*.

The development process is described by the following figure:

<img src="http://agile-development-tools.com/wp-content/uploads/2010/10/iterative-development1.png">

During the **Planning** phase, the committers decide the main features to be added in the new release by reviewing the BigBlueButton Road Map and all issues concerned with stability and usability.

After outlining the plan for the new release, the **Design** phase starts when each feature is assigned a Issue Tracker. This allows the community to track the project's progress and consists on a recording of the defects and enhancements made during the new release.

The **Development** phase begins after laying out the plan and design. During this time, the commiters usually hold bi-weekly meetings to discuss the project's development. Each commiter works on BigBlueButton's Master fork provided by *Github*. When a new feature is ready, the committer sends a pull request to merge the work into the Master branch. The merging is then reviewed by another committer who is familiar with that specific product's area. Any major change must be reviewed by the BigBlueButton's CTO (*Chief Technology Officer*) and the person responsible for that pull request must provide documentation to help with the reviewers work. This is very important to maintain the two first BigBlueButton's development priorities: stability and usability. If the pull request doesn't meet the expectations or affects one of these priorities, it is denied. Otherwise the new feature is tested in the latest build.

The **Beta Testing** phase begins after the core development is finished, all the bugs are fixed, and the corresponding documentation, installation and the development enviroment setting up are provided. The BigBlueButton's community has access to new features and there are several beta testings until the community stops reporting major bugs. Also, the documentation is reviewed and the installation package is updated to fix any bugs that may occur during the upgrade from the previous version. Finally, a *Release Candidate* is submitted and the core commiters monitor the mailing lists, twitter and the members' response for any bug that may cause impact to the general release. After fixing the issues, a new release candidate is provided. Each release candidate can last up to a month. If in a two weeks period, no new issue is reported concerning the last release candidate, the **General Release** is announced to the community.

## 2.2. Advantages and disadvantages

One of the main advantages of the incremental process in comparison with the Waterfall, lies in the fact that the last one will only have some commercial value when the project ends, as there is nothing practical to be presented before this stage. The incremental process makes it possible to initially have a prototype, verify the received feedback and some possible adjustments, and continue developing based on this experience. By doing this cyclically, we guarantee that when the final version is released it goes according to the expected target audience and with all the necessary adjustments.

One of the main incremental process disadvantages is that it's not agile compared to other ones often used in open source projects. After the planning, designing of each release and the starting of the development stage, this process doesn't allow any changes to the previously agreed issues. Taking that into account, it's necessary to wait for a future release to add new features. Lastly, the code structural integrity may start to crumble and, by performing changes, the code might become obsolete.
