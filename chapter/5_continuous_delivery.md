## Continuous Delivery

Often other developer are dependent on your software. There are different possibilities to deliver your software. Therefore it is often usefull to get feedback pretty soon. Because some also need some specific features, you need to invent some kind of versioning. One option is to use git commit ids, but those ids are very cryptic. Another option is to use [semantic versioning](http://semver.org/). This has the great advantage to be human readable. Now imageine you deliver some kind of software in a specific version. You go on developing and sadly you get a bug report for that delivered version. Now you need that specific version of your source code to fix that bug, because your new development is not ready to be released yet.
Therefore you should choose a GIT workflow. A intorduction for different workflows can be found [here](http://blog.endpoint.com/2014/05/git-workflows-that-work.html). Personaly I like the GIT-Flow pretty much for team development. It is also working pretty well with semantic versioning.

Of course it is possible to automate the deploy and to automatically use semantic versioning.

TODO(augustin) 





