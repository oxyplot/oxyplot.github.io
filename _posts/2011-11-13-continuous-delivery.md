---
layout: post
title: Continuous delivery
---

The build server is now based on [TeamCity][teamcity] and everything is automated:

- it builds all solutions
- it runs all [NUnit][nunit] tests and finds code coverage
- it pushes [NuGet][nuget] packages

[teamcity]: https://www.jetbrains.com/teamcity/
[cd]: https://en.wikipedia.org/wiki/Continuous_delivery
[nunit]: https://www.nunit.org/
[nuget]: https://www.nuget.org/
