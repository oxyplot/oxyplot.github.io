---
layout: post
title: Continuous delivery
---

The build server is now based on [TeamCity][teamcity] and everything is automated:

- it builds all solutions
- it runs all [NUnit][nunit] tests and finds code coverage
- it pushes [NuGet][nuget] packages

[teamcity]: http://www.jetbrains.com/teamcity/
[cd]: http://en.wikipedia.org/wiki/Continuous_delivery
[nunit]: http://www.nunit.org/
[nuget]: http://www.nuget.org/
