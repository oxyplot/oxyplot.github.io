---
layout: post
title: NuGet packages
---

We have stopped pushing pre-release packages from the CI build to nuget.org (on request from nuget.org).
The official nuget feeds will from now on only be used for stable releases.

Pre-release packages from every CI build are now pushed to myget.org.  
The OxyPlot packages are listed on [https://www.myget.org/feed/Packages/oxyplot](https://www.myget.org/feed/Packages/oxyplot)

To use these packages, you must add the myget feed as a package source.  
The feed sources can be found at: [https://www.myget.org/feed/Details/oxyplot](https://www.myget.org/feed/Details/oxyplot)

![myget.org source]

Remember to check "Include prerelease" or add the "-pre" flag to install the myget packages.

![myget.org package manager]

![myget.org package console]

[myget.org source]: /public/images/posts/2016-05-24-myget-source.png
[myget.org package manager]: /public/images/posts/2016-05-24-myget-package-manager.png
[myget.org package console]: /public/images/posts/2016-05-24-myget-package-manager-console.png
