#15. Degree of Testability

##15.1. BigBlueButton Testability

In order to ensure that a program works as expected the developers implement and use tests. BigBlueButton has a specific way to guarantee the implemented features produce the expected output. This includes **Unit Testing**, **Integration Testing** and **Stress Testing**. 

###15.1.1. Testing the gem

To test the gem BBB makes **Unit Tests** using **rspec** which are found in the folder spec/. A tester doesn't need a real BigBlueButton server to run these tests. They all use mocks and stubs to simulate the behaviour of a real server. BBB also makes **Integration Tests** using **cucumber** (and **rspec**) which are found under the folder features/. In this case the tester needs a real server to run them. This server also needs support to the Android mobile client.

To run the tests the tester uses the following commands (Ruby):
```ruby
$ bundle exec rake spec      # runs all unit tests
$ bundle exec rake cucumber  # runs all integration tests
$ bundle exec rake           # runs everything
```


<!-- How "testable" is the program



How to improve the testability of software components



Controllability: The degree to which it is possible to control the state of the component under test (CUT) as required for testing.

Observability: The degree to which it is possible to observe (intermediate and final) test results.

Isolateability: The degree to which the component under test (CUT) can be tested in isolation.

Separation of concerns: The degree to which the component under test has a single, well defined responsibility.

Understandability: The degree to which the component under test is documented or self-explaining.

Heterogeneity: The degree to which the use of diverse technologies requires to use diverse test methods and tools in parallel. -->

