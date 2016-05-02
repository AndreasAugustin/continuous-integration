## Testing

For every development process tessting is very important. Imagine one developer implements a funciton and another modifies it without complete knowledge how it should process. It is very comon to destroy the asserted result. To minimize such unwanted behaviour it is commen to introduce some automated tests. Testing is not easy stuff but modern testing frameworks help a lot.

There are some different kinds of testing

![testing_pyramide](../images/testing_pyramide.jpg "testing-pyramide" "width:300px;float:right;padding-right:100px;")

- Testing Frameworks

| language    | unit testing framework |
|-------------|------------------------|
| csharp/mono | NUnit                  |
| cpp         | google test            |
| JS/coffee   | jasmine                |
| JAVA        | JUnit                  |
| Python      |						   |
| Ruby        |                        |

- Mocking Frameworks

| language    | mocking framework |
|-------------|-------------------|
| csharp/mono | NSubstitute       |
| cpp         | google mock       |
| JS/coffee   |    |
| JAVA        | moquito           |
| Python      |     |
| Ruby        |  |

- BDD/ATDD Frameworks
	For behaviour testing there is Gherking with Cucumber
    https://github.com/AndreasAugustin/Gherkin-Demos

### xUnit

There is a standard called xUnit for testing. The x stands for different programming languages. Following the standard has the advangage that every developer is (should be) able to understand the written tests. So tests are also some kind of documentation.

