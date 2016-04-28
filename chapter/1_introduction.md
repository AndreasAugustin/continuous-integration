## Introduction


Some people like to work on the same project and face some problems:

- After a merge the project is not building anymore due to
  * Version conflicts
  * Merge conflicts
  * Different development environments

 - After a merge some of my tests are failing
   * Other developers did not run my tests

- The code of the other developer look pretty ugly
  * No or different coding standards

 A solution to prevent such problems is to invent some kind of automatism like a server which is running some standard tasks like
 - Static code analysis
 - Unit/integration tests
 - Build

![CI idea](../images/ci5.png)

A CI server can take over such tasks.

There you can automate your tasks on different virtual machines or container with different operating systems.
Those tasks can be
- Build the project
- Run tests and publish the reports
- Code analysis

The reports are often human readable and show your awesome work to stakeholder/project managers and your nice developer colleages.
