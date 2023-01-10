# ECE444-F2022-Lab6

This application can be accessed at https://ece44406lab.herokuapp.com/ 

This project was created following : https://github.com/mjhea0/flaskr-tdd 


## Test created for group project (group 10)

The test was created as part of a feature PR for templated pathways to test the endpoint and model. The test function created is called test_templated_pathways()

The code changes can be found here:

https://github.com/ECE444-2022Fall/project-1-web-application-design-education-pathways-group-10-x-engineers/commit/a93fa47d56c4d0d96169b95561a56b1f37ce8153 

## What are the Pros and Cons of TDD

Test driven development is a software development process which involves making test cases a neccesity before any software is deployed. The reason for this is because test driven development helps reduce many bugs that could have happened in past features as well as the current feature the user is implementing. If a developer creates a breaking change in another feature, since there is a test for that feature they would be notified if this was the case. Typically, the project should ensure that the code coverage of the project does not decrease on feature merge and no breaking changes occur. CICD would be used to run certain tests on merge or on commit depending on: the scale of the project (ie. the time it takes to build/test all the functionalities) or  scope of the changes. The primary disadvantage of test driven development is that the cost of developing a feature would increase as the developer would have to create tests as well as implement the feature. Additionally, in rare cases if a breaking change occurs to other tests but it is expected past tests may need to be changed to support new features. Test driven development can consist of Unit tests, behavior tests, integration tests, performance testing and more. Depending on the company or the project’s requirements the scale of testing would be determined.

The above paragraph can be summarized with the following bullet points:

Pros:

* Fewer breaking changes merged into the codebase
* Cheaper long term development costs
  * Fewer bugs and unexpected issues in future
* Tests can be used alongside documentation to understand the purpose of features
* Better code quality, readability and software architecture
* Tests can be of various types (ie. behaviour/unit/integration/performance tests) to test all possible use cases of the software

Cons:

* Increase in short term feature development time/costs
* Teams may use TDD inconsistently if they are not provided with suggested practices
* Long tests or too many unneccesary tests can greatly increase time to test the features and CICD run time
  * Cost increase in CICD VMs/Development time over all features instead of just 1 feature
