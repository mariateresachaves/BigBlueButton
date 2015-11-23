#LINKS:

https://groups.google.com/forum/#!topic/bigbluebutton-dev/PHzpgVqYAMM    --> resultado test stressing
http://users.ece.cmu.edu/~koopman/des_s99/sw_testing/#reference 

Stress testing to test the server -> https://code.google.com/p/bigbluebutton/wiki/StressTesting

Unit testing and integration testing to test the gem -> https://github.com/mconf/bigbluebutton-api-ruby/wiki/Testing

Stress testing to test the audio -> https://groups.google.com/forum/#!topic/bigbluebutton-dev/PHzpgVqYAMM

Testing requirements -> https://code.google.com/p/bigbluebutton/wiki/RecordPlaybackSpecification

BBB documentation about tests -> http://docs.bigbluebutton.org/support/road-map.html

Unit testing Mobile Client -> http://zenit.senecac.on.ca/wiki/index.php/BigBlueButton http://zenit.senecac.on.ca/wiki/index.php/BigBlueButton_Mobile_Client_Unit_Tests

Stress testing script -> https://github.com/bigbluebutton/bigbluebutton/tree/master/labs

Video about stress test the server -> https://www.youtube.com/watch?v=Av8a0gB-Y3I

-> http://e-standards.flexiblelearning.net.au/research/funded_projects/emerging_technology_trials/2012/big_blue_button.php

https://github.com/bigbluebutton/bigbluebutton/issues/2878 -> bug report: se escreverem algo entre aspas ("") não aparece no chat

Codigo com testes
https://github.com/mariateresachaves/bigbluebutton/blob/master/bigbluebutton-web/test/unit/org/bigbluebutton/api/ParamsProcessorUtilTest.java
https://github.com/mariateresachaves/bigbluebutton/blob/master/deskshare/app/src/test/java/org/bigbluebutton/deskshare/server/recorder/FileRecorderTest.java
https://github.com/mariateresachaves/bigbluebutton/blob/master/labs/api/recordings/test/testc.coffee
https://github.com/mariateresachaves/bigbluebutton/blob/master/labs/api/recordings/test/routetests.coffee
https://github.com/mariateresachaves/bigbluebutton/blob/master/labs/api/recordings/test/utiltests.coffee
https://github.com/mariateresachaves/bigbluebutton/blob/master/labs/api/meetings/test/routetests.coffee

#Unit testing
Unit Testing the Mobile Client
With the mobile client's development coming close to completion, the importance of unit testing is becoming increasingly important. Though not in the spirit of test driven development, the unit tests are being written after the core application. See the following link for general information about unit testing, specific information regarding the framework we are using to unit test the mobile client, and information about the current state of the coverage of the unit tests.
Documentation of the mobile client's unit testing    
http://zenit.senecac.on.ca/wiki/index.php/BigBlueButton_Mobile_Client_Unit_Tests


Members of our community periodically host stress tests for BigBlueButton, which gives others a data point on what a particular server was able to handle. Take any stress test with a grain of salt. There are many variables at play:

Server: CPU memory, disk space, and bandwidth
Usage scenarios (# of webcams and use of desktop sharing)
Upstream bandwidth from clients
Configuration of BigBlueButton
Version of BigBlueButton


We are continuously trying to incorporate more automated testing into the BigBlueButton development process, such as using TestNG.


http://e-standards.flexiblelearning.net.au/research/funded_projects/emerging_technology_trials/2012/big_blue_button.php


COMPLEXIDADE DOS TESTES: REFERIR McCabe

------------------------------------------------------------

#Testing methods

**Black-Box Testing**

-	Internal structure is not known
-	Performed by end-users (clientes) and also by testers and developers
-	Testing is based on what the end-users expected
-	It’s exhaustive
- Least time-consuming method
-	Not suited for algorithm testing
- Trial and error method

**Grey-Box Testing**

-	Limited knowledge of the internal structure
-	Performed by end-users (clients) and also by testers and developers
-	Testing is done on the basis of high-level database diagrams and data flow diagrams
-	Consume a bit of time and it’s exhaustive
- Not suited for algorithm testing
-	Data domains (e.g. data types) and internal boundaries (e.g. limit of 50 users per conference) can be tested if known

**White-Box Testing**

-	Has full knowledge of the internal structure
-	Usually done by testers and developers
-	The tester can design test data accordingly
-	Exhaustive and time-consuming
- Suited for algorithm testing
-	Data domains and internal boundaries can be better tested

#Types of testing

-	**Unit testing**
	- Testing of an individual unit or group of related units
	- Falls under the class of white-box testing 
	- Often done to test if the given input is producing the expected output

-	**Integration testing**
	- Testing in which a group of components are combined to produce output
	- The interaction between hardware and software is tested in integration testing if software and hardware components have any relation
	- It may fall under both white-box and black-box testing 

-	**Functional testing**
	- Testing to ensure that the specified functionality required works
	- Falls under the class of black-box testing

-	**System testing**
	- Testing to ensure that by putting the software in different environments it still works
	- Falls under the class of black-box testing

-	**Stress testing**
	- Testing to evaluate how system behaves under unfavorable conditions
	- Conducted at beyond limits of the specifications
	- Falls under the class of black-box testing

-	**Performance testing**
	- Testing to assess the speed and effectiveness of the system
	- Falls under the class of black-box testing

-	**Usability testing**
	- Testing is performed to the perspective of the client, to evaluate how the GUI is user friendly, how easily can the client learn, etc.
	- Falls under the class of black-box testing

-	**Acceptance testing**
	- Testing is often done by the customer to ensure that the delivered product meets the requirements and works as the customer expected
	- Falls under the class of black-box testing

-	**Regression testing**
	- Testing after modification of a system, components, or a group of related units to ensure that the modification is working correctly and is not damaging or imposing other modules to produce unexpected results
	- Falls under the class of black-box testing

-	**Beta testing**
	- Testing which is done by end-users, at team outside development, or publicly releasing full pre-version of the product which is known as beta version. 
	- Falls under the class of black-box testing
