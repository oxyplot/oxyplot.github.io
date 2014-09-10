---
layout: post
title: Continuous integration
---

The OxyPlot build is now hosted at [AppVeyor][appveyor]! This is a great service that does both [continuous integration][ci] and deployment.
See the `appveyor.yml` file for the build configuration. [StyleCop][stylecop] and [Gtk#][gtksharp] are now installed by [chocolatey][chocolatey].

All OxyPlot NuGet packages except the Xamarin packages will be updated in each build.
The Xamarin.Android and Xamarin.iOS packages are not included in the AppVeyor build, and are still built locally on a Mac. 
It would be great if we could get a similar build and deployment solution also for these projects!

The Silverlight "[Example browser][examplebrowser]" will also be updated at each build.

Builds on the `develop` branch will get a pre-release suffix `-alpha` in the NuGet packages, this will make it possible to select between "Stable Only" and "Include Prerelease" channels in the NuGet manager.

[appveyor]: http://appveyor.com/
[ci]: http://en.wikipedia.org/wiki/Continuous_integration
[oxyplot-ci]: https://ci.appveyor.com/project/objorke/oxyplot
[chocolatey]: http://chocolatey.org/
[stylecop]: http://stylecop.codeplex.com/
[gtksharp]: http://www.mono-project.com/docs/gui/gtksharp/
[examplebrowser]: http://resources.oxyplot.org/examplebrowser/