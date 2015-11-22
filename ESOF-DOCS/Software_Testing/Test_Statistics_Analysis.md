#3. Test Statistics Analysis

BigBlueButton's testing phase is extensive, and one of the core development parts of the project. The developers of BigBlueButton focus their testing on 3 groups: **unit testing**, **integration testing** and **stress testing**.

The main focus of BigBlueButton's development team are the **stress tests**, which consists in having an increasingly large number of users logging in the application and using it to see what is the server response to it. Since BigBlueButton consists of a web-conferencing platform, many users will be logged in at the same time in the same room, using all the capabilities of the software simultaneously and it's imperative that the software can handle these situations.  One of these tests results is shown in Fig.2, a graph showing the CPU usage along the time.

<p align="center">
  <img src="images/stress_test.png" width="80%" height="80%">
  <span class="caption">
        <p align="center"><b>Fig. 2</b> Results of an audio stress test</p>
  </span>
</p>

In this test, the server was getting more and more users using the audio capabilities of the application, until it got overloaded when it reached about 80 users, moment where the audio started degrading, with CPU reaching 90% of it's processing power. The number of users then dropped to 60, and the audio quality was good, once again. Some users were then asked to turn on their webcams, but the CPU got very little additional load, maintaining the audio with a good quality. Users were then asked to use desktop sharing, which caused a crash of the application, thus creating another issue open for investigation.

Other focus in the testing phase is the **unit testing**. Contrary to the spirit of test driven development, the unit tests are being written **after** the core application. The developer team adds unit tests to the core modules (voice, video, chat, presentation, and desktop sharing) to verify their functionality, and follow these guidelines:

* Don't test languages or frameworks. If a developer is using a library or framework and the documentation tells the behavior of that class or function, then it shouldn't be tested, as it is a bug in that library and not in the application;
* Don't test simple "getters" and "setters" functions;
* Each control structure adds one more unit test to the function;
* Each special case deserves a unit test. Generally, each way a function can possibly be ended, adds one more unit test to that function;
* Each event that gets dispatched adds one more unit test.

In Fig. 3, we can see a table showing some of the already tested modules in BigBlueButton.

<p align="center">
  <img src="images/Unit_tests.png" width="90%" height="90%">
  <span class="caption">
        <p align="center"><b>Fig. 3</b> Different components tested</p>
  </span>
</p>

Lastly, in the **integration tests** developers should have a complete test suite to verify stability and conformance to documentation. Unfortunately, we didn't find any results concerning integration tests, other than what is shown here.
