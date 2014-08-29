---
layout: home
published: true
---

[![Build status](https://ci.appveyor.com/api/projects/status/mlaqnruo6ic3oe60)](https://ci.appveyor.com/project/objorke/oxyplot)

![Example plot](/public/images/normal-distributions.png)

OxyPlot is a cross-platform plotting library for .NET. 

The code is licensed under the MIT license. This means that the library can be used in commercial applications, and modified as much as you want.

The core library is a [Portable Class Library][pcl] which is shared between different user interface platforms. Custom controls are implemented for WPF, Windows 8, Windows Phone, Windows Forms, Silverlight, GTK#, Xamarin.iOS and Xamarin.Android.

- OxyPlot can be tested online with the [Silverlight Example Browser][example-browser]
- The documentation is located at [oxyplot.org/documentation][docs]
- The latest binaries can be found in the [NuGet packages][nuget-packages]


### Supported platforms

See the [supported platforms][supported-platforms] section in the documentation.

### Features

OxyPlot contains many different types of axes and series. And if you need some functionality that is not included in the library, you can always create a derived class and override the rendering implementation.

The plots can be exported to file formats like [png][export-png], [pdf][export-pdf] and [svg][export-svg].

### Getting started

1. Use the [NuGet][nuget] package manager to add the [OxyPlot package][nuget-packages] for your platform. 
2. Add a `PlotView` control to your user interface. 
3. Create a `PlotModel`
4. Bind or assign the `PlotModel` to the `Model` property of the control.

See the [getting started][getting-started] section for more information for each platform. 

### Examples

Example code can be found in the [Source/Examples][repo-examples] folder in the repository. There is also an online [example browser][example-browser] based on Silverlight.

### Documentation

The documentation can be found at [oxyplot.org/documentation][docs]. Note that it is under construction and this task has high priority. Please contribute!

### Questions

Use the discussion forum at [discussion.oxyplot.org][forum] if you have questions regarding the library. You can also use [Stack Overflow][so] or the [Xamarin forum][xamarin-forum].

### Announcements

News about the library can be found under [announcements][announcements]. There is also an [atom feed][feed] for the posts.

### Contribute

This project is continuously evolving and any kind of help is greatly appreciated. See the [contributions][contributions] page for more information.

### Thanks

The project is supported by

- [Jetbrains][jetbrains]
  - [Resharper][resharper]
  - [dotCover][dotcover]
  - [TeamCity][teamcity]
- [NDepend][ndepend]
  - [NDepend v5][ndepend]
- [Red Gate Software][redgate]
  - [ANTS][ants]
- [Xamarin][xamarin]
  - [Xamarin Studio][xamarin]
- [OzCode][ozcode]
  - [OzCode VS extension][ozcode-extension]
- [UserEcho][userecho]

[nuget]: http://www.nuget.org/
[nuget-packages]: http://www.nuget.org/packages?q=oxyplot
[pcl]: http://msdn.microsoft.com/en-us/library/vstudio/gg597391(v=vs.100).aspx
[export-pdf]: /documentation/export-pdf
[export-png]: /documentation/export-png
[export-svg]: /documentation/export-svg

[docs]: /documentation
[support]: /support
[contributions]: /documentation/contributions
[getting-started]: /documentation/getting-started
[supported-platforms]: /documentation/supported-platforms
[announcements]: /announcements
[feed]: http://oxyplot.org/atom.xml

[repo]: https://github.com/oxyplot/oxyplot
[repo-examples]: https://github.com/oxyplot/oxyplot/tree/master/Source/Examples
[contributors]: https://github.com/oxyplot/oxyplot/graphs/contributors

[example-browser]: http://resources.oxyplot.org/examplebrowser/

[forum]: http://oxyplot.userecho.com/
[so]: http://stackoverflow.com/questions/tagged/oxyplot?sort=newest
[xamarin-forum]: http://forums.xamarin.com/search?Search=oxyplot
[twitter]: https://twitter.com/search?q=oxyplot
[twitter-hashtag]: https://twitter.com/search?q=%23oxyplot&src=hash

[xamarin-component]: http://components.xamarin.com/
[xamarin-mac]: http://xamarin.com/mac
[mono-mac]: http://www.mono-project.com/MonoMac

[jetbrains]: http://www.jetbrains.com/
[resharper]: http://www.jetbrains.com/resharper/
[dotcover]: http://www.jetbrains.com/dotcover/index.html?topDC
[teamcity]: http://www.jetbrains.com/teamcity
[ndepend]: http://www.ndepend.com/
[redgate]: http://www.red-gate.com/
[ants]: http://www.red-gate.com/products/dotnet-development/ants-performance-profiler/
[xamarin]: http://www.xamarin.com/
[ozcode]: http://www.oz-code.com/
[ozcode-extension]: http://visualstudiogallery.msdn.microsoft.com/36925113-cdce-4953-a5d6-fb3d2912dad7
[userecho]: http://www.userecho.com/

[jetbrains-img]: http://www.jetbrains.com/img/banners/Codebetter.png
