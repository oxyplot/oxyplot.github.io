---
layout: post
title: Continuous integration
---

OxyPlot is now built at [AppVeyor]. This change has simplified
the build system significantly and removed the need for a local build
server. AppVeyor provides a great service that does both [continuous
integration] and deployment for all platforms except the Xamarin
ones.

The build is configured in the `appveyor.yml` file and handles both the
`develop` and `master` branches.

The [StyleCop], [Gtk#] and [Lynx Toolkit] prerequisities are now
installed by [chocolatey].

The NuGet packages will be updated by each build. The Xamarin.Android
and Xamarin.iOS packages are not included in the AppVeyor build, and are
still built locally on a Mac. It would be great if we could get a
similar build and deployment solution also for these projects...

The Silverlight "[Example browser]" will also be updated by each build.

Builds on the `develop` branch will get a pre-release suffix `-alpha` in
the version numbers. This will make it possible to select between
"Stable Only" and "Include Prerelease" versions in the NuGet manager.

Another great feature is that every pull request on GitHub will
automatically trig a build on AppVeyor. A broken build will be shown on
the pull request page!!

[AppVeyor]: http://appveyor.com/
[continuous integration]: http://en.wikipedia.org/wiki/Continuous_integration
[oxyplot-ci]: https://ci.appveyor.com/project/objorke/oxyplot
[StyleCop]: http://stylecop.codeplex.com/
[Gtk#]: http://www.mono-project.com/docs/gui/gtksharp/
[Lynx Toolkit]: https://github.com/objorke/lynx-toolkit/
[chocolatey]: http://chocolatey.org/
[Example browser]: http://resources.oxyplot.org/examplebrowser/