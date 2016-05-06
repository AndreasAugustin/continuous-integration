## Code analysis

In a big team it is also necessary to have some coding guidelines. One example are the google coding guidelines:
https://github.com/google/styleguide
There you can also find some settings for IDEs. For verifying that every developer cares about those coding standards you can use some lint tools.

### Lint tools

| language    | lint tool  |
|-------------|------------|
| cpp         | cpplint    |
| java        | checkstyle |
| csharp/mono | stylecop   |
| python      | pylint     |
| JS		  | jslint     |
| coffee      | coffeelint |

Those lint tools create a xml file with some information about vilations. Often those can be pusblished in a nice human readable form with CI Server. Also most IDEs are able to give validation information at development time.

Sadly those tools are not supported by appveyor and travis (yet).
For JAVA; C/Cpp https://docs.travis-ci.com/user/coverity-scan/ https://scan.coverity.com

TODO(augustin) add some lint tools integrated with travis/appvayor


### Dependency Versioning

It is often a good idea to keep the dependencies up to date (if possible). There are some version checker out there, which can keep track about the versions of your project. One example is VersionEye
https://www.versioneye.com/

### Code review

TODO(augustin)

### Get your hands dirty

- Add a lint tool to your project and let it run TODO(augustin) think about lint tools
- Add your project to versioneye and a badge to your README.md


### Examples

Open one language folder in the examples section.
TODO(augustin) add examples

	$ git checkout chapter_2







