#3. Critical Analysis
BigBlueButton has a very active community. With 57 contributors on GitHub and a core development team of 6 people who is responsible for the core features development and overall quality of the project. The contributors of BBB are constantly helping and supporting each other and new developers. The forum and mailing list are constantly monitored and any new issue is quickly answered. Everyone who wants to contribute is welcome to the team and a very detailed documentation is provided to help the new developers. The BigBlueButton client is written in ActionScript and the server components are written in a combination of Java, Grails, and Scala.

The contributors to the BigBlueButton project are developers at the company co-founded by the original developer, students, faculty of the university (who are also lead users of the system), and members of other businesses who are developing complementary products. Code, project plans, as well as bugs and feature requests are shared. Currently, any registered
contributor can contribute equally to the project.

Through the analysis of the GitHub repository, we can see that BigBlueButton reached its peak in contributions in late 2014 and 2015, which proves the impact that the project is presently having on the community. We can also see the extensive testing period for this project demonstrated by the far away dates in-between releases. For example, the last version (0.9) got a release candidate in September 2014, but was only accepted at the very end of April 2015. This proves what the original authors wanted, by extensively testing their releases to assure maximum quality on their product. The same happens in all previous releases.

While BigBlueButton initially did not create releases frequently enough so as to maximize development velocity, automated builds are now created after each successful commit (that passes tests).


The repository of the BigBlueButton project is managed in the following way: whenever a new feature begins to develop or when a issue is reported, they are developed/fixed in their corresponding branch (e.g. *polling-module*). When these are ready, they are merged with the *development* branch, where it is further extensively tested. It is also where it is integrated along with all the other already existing features. When these new features finished testing without any issue, they are then merged into the *master* branch, thus creating a new release.

To balance the need of users for stability with the need to explore new directions, the BBB project has separate streams for the production version, which is used to teach online classes and therefore requires the behavior of the system to be stable, and streams for new feature development development that will eventually be introduced into the stable stream.

Currently, the developers are working on the beta testing phase for the 1.0 release. The features stated on their documentation for the 1.0 release were already implemented, with the last one being the reconnection of the lost users during a live conference. 
