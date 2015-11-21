#3. Test Statistics Analysis

BigBlueButton's testing phase is extensive, and one of the core development parts of the project. In this section we'll list some of the testing methods used by BigBlueButton's developers.

One of the important tests is the **stress test**, which consists in having an increasingly large number of users logging in the application and using it to see what is the server response to it. One of these tests results is shown in Fig.2

<p align="center">
  <img src="images/stress_test.png" width="80%" height="80%">
  <span class="caption">
        <p align="center"><b>Fig. 2</b> Results of an audio stress test</p>
  </span>
</p>

In this test, the server was getting more and more users using the audio capabilities of the application, until it got overloaded when it reached about 80 users, moment where the audio started degrading, with CPU reaching 90% of it's processing power. The number of users then dropped to 60, and the audio quality was good, once again. Some users were then asked to turn on their webcams, but the CPU got very little additional load, maintaining the audio with a good quality. Users were then asked to use desktop sharing, which caused a crash of the application, thus creating another issue open for investigation.
