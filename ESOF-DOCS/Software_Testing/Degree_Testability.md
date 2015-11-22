#15. Degree of Testability

##15.1. BigBlueButton Testability

In order to ensure that a program works as expected the developers implement and use tests. BigBlueButton has a specific way to guarantee the implemented features produce the expected output. This includes **Unit Testing**, **Integration Testing** and **Stress Testing**. 

###15.1.1. Testing the Gem

To test the gem BBB makes **Unit Tests** using **rspec** which are found in the folder spec/. A tester doesn't need a real BigBlueButton server to run these tests. They all use mocks and stubs to simulate the behaviour of a real server. BBB also makes **Integration Tests** using **cucumber** (and **rspec**) which are found under the folder features/. In this case the tester needs a real server to run them. This server also needs support to the Android mobile client.

To run the tests the tester uses the following commands (Ruby):
```ruby
$ bundle exec rake spec      # runs all unit tests
$ bundle exec rake cucumber  # runs all integration tests
$ bundle exec rake           # runs everything
```

###15.1.2. Testing the Mobile Client

The <a href="http://cdot.senecacollege.ca/">**Seneca CDOT**</a> of Seneca College, like many other instituitions and organizations, collaborates with open source community, business, and other instituitions. Currently, they take part of the BBBs core developement team and as a contribution they tested the Mobile Client using **Unit Tests**.  

The list of steps is shown below:  

  * **First**, it is needed to code a listener method that verifies the values that the signal is dispatched. The verification can be done simply with <code>assertThat(...)</code>. Then a 'verification' method must be added as a listener to the signal that we want to check.  
  
  * **Second**, the tester must dispatch a custom event in this verification method, that will be used in the next step.  
  
  * **Third**, in the test case, it is used <code>Async.proceedOnEvent(...)</code> to listen for the custom event that is dispatched from the verification method. The <code>Async.proceedOnEvent(...)</code> will cause the unit test to fail if the event that is being listened for does not get dispatched.  
  
  * If the signal does not get dispatched, then the verification method will never get called, and will never dispatch the event that the <code>Async</code> is waiting for, causing the unit test to fail.  
  
  * If the signal is dispatched, but with the wrong values, it will cause the <code>assertThat(...)</code> checks to fail. Any further checks on the class should also be done here, because signal are dispatched asynchronously.

The **Mobile Client** was initially structured using the **Model-View-Controller (MVC)** design pattern. As time went on the code base got scattered in a way that is not entirely in keeping with the design pattern. The **Mobile Client's** code is divided into four main parts: models, views, core, and commands. The meanings of "model" and "view" are the same as in the **MVC** design pattern.

These tests are still being implemented and no conclusions can be done at this moment.

<!-- How "testable" is the program

The "core" component is where most of the code that communicate with a BigBlueButton server ended up. I don't think this part of the application should be unit tested for two main reasons. First, most of the code in the "core" is simple, and repeats the same pattern over and over again. Second, unit testing this part of the application may make it more "brittle". This is because any time the message format for communication between client and server changes (not an infrequent occurrence), the unit tests will also need to be redesigned or they will fail.

How to improve the testability of software components



Controllability: The degree to which it is possible to control the state of the component under test (CUT) as required for testing.

Observability: The degree to which it is possible to observe (intermediate and final) test results.

Isolateability: The degree to which the component under test (CUT) can be tested in isolation.

Separation of concerns: The degree to which the component under test has a single, well defined responsibility.

Understandability: The degree to which the component under test is documented or self-explaining.

Heterogeneity: The degree to which the use of diverse technologies requires to use diverse test methods and tools in parallel. -->

