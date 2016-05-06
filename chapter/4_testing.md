## Testing

For every development process tessting is very important. Imagine one developer implements a funciton and another modifies it without complete knowledge how it should process. It is very comon to destroy the asserted result. To minimize such unwanted behaviour it is commen to introduce some automated tests. Testing is not easy stuff but modern testing frameworks help a lot.

### Introduction

There are some different kinds of testing

![testing_pyramide](../images/testing_pyramide.jpg "testing-pyramide" "width:300px;float:right;padding-right:100px;")

#### Test concepts

![](../images/testing_workflow.jpg "WorkFlow" "float:right;padding-left:10px;")
- [Acceptance-Test-Driven-Development (ATDD)](#ATDD).
- [Behaviour-Driven-Development (BDD)](#BDD).
- [Test-Driven-Development (TDD)](#TDD).

#### ATDD (Acceptance Test Driven Development)

![](../images/ATDD-overview.jpg "ATDD"  "width:300px;float:right;padding-left:10px;")
- User, testers, product-owner, developers, .. together develop testing criteria.
- Defining those acceptance tests leads to a better understanding for the task.


#### BDD (Behaviour Driven Development)

![](../images/TDDWithBDD.png "TDDWithBDD" "width:300px;float:right;padding-left:10px;")
- Combines general TDD patterns with domain-Driven-Design (DDD).
- Test is a feature, the features are defined by the stakeholder (product owner).
- Given-When-Then.

#### TDD (Test Driven Development)

![](../images/tdd_cycle.jpeg "TDD" "width:300px;float:right;padding-left:10px;")
- Test first priciple.
- Also called Test-Driven-Design.
- Improves design and software quality.
- Tests are defined in small steps.

#### Frameworks

##### Testing

| language    | unit testing framework |
|-------------|------------------------|
| csharp/mono | NUnit                  |
| cpp         | google test            |
| JS/coffee   | jasmine                |
| JAVA        | JUnit                  |
| Python      |						   |
| Ruby        |                        |

##### Mocking

| language    | mocking framework |
|-------------|-------------------|
| csharp/mono | NSubstitute       |
| cpp         | google mock       |
| JS/coffee   |    |
| JAVA        | moquito           |
| Python      |     |
| Ruby        |  |

##### BDD/ATDD Frameworks

For behaviour testing there is Gherking with Cucumber
https://github.com/AndreasAugustin/Gherkin-Demos

### xUnit

There is a standard called xUnit for testing. The x stands for different programming languages. Following the standard has the advangage that every developer is (should be) able to understand the written tests. So tests are also some kind of documentation.

### Get your hands dirty

- TODO(augustin) add testing srver (reports)
- Start implementing some code in your project with TDD principles.
- Add running those tests to your .travis.yml and/or appveyor.yml.


### Examples

Open one language folder in the examples section.
TODO(augustin) add examples

	$ git checkout chapter_3
