
## CI Server


### Self host (or cloud)

- [Jenkins](https://jenkins.io/)  ![jenkins](../images/jenkins.png)
  -  Configuration by web interface
  -  Open source
  -  Lots of Plugins
  -  Slave based
  -  Con: Plugins are often not maintained and buggy

- [TeamCity](https://www.jetbrains.com/teamcity/) ![teamcity](../images/teamcity.png)
  - JetBrains (supported)
  - Configuration by web interface
  - Slave based
  - Free for 20 build configurations, 3 build agents and full featured

- [Bamboo](https://de.atlassian.com/software/bamboo) ![bamboo](../images/bamboo.png)
  - Attlasian (supported)
  - Configuration by web interface?


### GitHub addon (cloud)

- [Travis](https://travis-ci.org/) ![travis](../images/travis.png)
  - Configuration by YAML file
  - Container based
  - OSX/Linux
  - Free (public open source projects)


- [Appveyor](https://travis-ci.org/) ![appveyor](../images/appveyor.png)
  - Configuration by YAML file
  - Naturally VS projects with NUGET (possible to script other languages)
  - Windows
  - Free for public open source projects


For the lessons we will stick with Travis ans Appveyor because it is perfectly integrated into GitHub and cloud based. It is also very helpfull for your development process to choose a build tool and some dependency management. Here is a small list about possiblble tools (Gradle can also be a nice choice):

| Language 	| Tool(s) 			|
|-----------|-------------------|
| Csharp   	| MSBuild with NUget|
| Mono     	| xBuild with Nuget |
| NodeJS   	| gulp + bower      |
| Cpp      	| CMake				|
| Ruby	   	| Gem + rake		|
| Java     	| Maven				|
| Python 	| Pip				|

### Get your hands dirty

- First decide for a programming language. It is possible to create CI jobs for mixed languages (for mentioned CI server) in one project, but I prefer not mixing programming languages in my projects. This also leads to a better architecture in your project because it needs to be tested and built without other domains. Also it is nicer for versioning the project. For bundling it is possible to use GIT modules.
- Think about which operating systems you like to support.
- Decide for a build tool.
- Create a GitHub repository and clone it to your local environment. Add a project. Here we will stick with simple testing demos.
- According to your OS decision
  - Linux/OSX
  	- At GitHub click on your icon and on integrations. Choose Travis and follow the instructions.
  	- Add permissions at [TRAVIS](https://travis-ci.org/) to read your repository.
  	- Locally at your repository add a .travis.yml to the base folder. Language guide: https://docs.travis-ci.com/user/language-specific/ Hint: if you use csharp as language (mono) then the BOM in .travis.yml need to be removed.
  	- Validate .travis.yml https://docs.travis-ci.com/user/travis-lint/
  - Windows
    - At GitHub click on your icon and on integrations. Choose Appveyor and follow the instructions.
  	- Add permissions at [Appveyor](https://ci.appveyor.com/) to read your repository.
  	- Locally at your repository add a appveyor.yml to the base folder.
- Add badges about the building status to your README.md

Of course it is possible to support Linux/OSX and Windows

