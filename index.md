---
layout: home
published: true
---

![Example plot]

OxyPlot is a cross-platform plotting library for .NET. 

The code is licensed under the MIT license. This means that the library can be used in commercial applications, and modified as much as you want.

The core library is a [Portable Class Library] which is shared between different user interface platforms. Custom controls are implemented for WPF, Windows 8, Windows Phone, Windows Forms, Silverlight, GTK#, Xamarin.iOS and Xamarin.Android.

- OxyPlot can be tested online with the Silverlight [example browser]
- The documentation is located at [oxyplot.org/documentation]
- The latest binaries can be found in the [NuGet packages]

### Supported platforms

See the [supported platforms] section in the documentation.

### Features

OxyPlot contains many different types of axes and series. And if you need some functionality that is not included in the library, you can always create a derived class and override the rendering implementation.

The plots can be exported to file formats like [png], [pdf] and [svg].

### Getting started

1. Use the [NuGet] package manager to add the [OxyPlot package][NuGet packages] for your platform. 
2. Add a `PlotView` control to your user interface. 
3. Create a `PlotModel`
4. Bind or assign the `PlotModel` to the `Model` property of the control.

See the [getting started] section for more information for each platform. 

### Examples

Example code can be found in the [Source/Examples] folder in the [repository]. There is also an online [example browser] based on Silverlight.

### Documentation

The documentation can be found at [oxyplot.org/documentation]. Note that it is under construction and this task has high priority. Please contribute!

### Questions

Use the discussion forum at [discussion.oxyplot.org] if you have questions regarding the library. You can also try the [chat room], [Stack Overflow] or the [Xamarin forum].

### Announcements

News about the library can be found under [announcements]. There is also an [atom feed] for the posts.

### Contribute

This project is continuously evolving and any kind of help is greatly appreciated. See the [contributions] page for more information.

### Thanks

The project is supported by

- [Jetbrains]
  - [ReSharper]
  - [dotCover]
- [NDepend]
  - [NDepend v5][NDepend]
- [Red Gate Software]
  - [ANTS]
- [Xamarin]
  - [Xamarin Studio][Xamarin]
- [OzCode]
  - [OzCode VS extension]
- [UserEcho]

[Example plot]: /public/images/normal-distributions.png
[NuGet]: http://www.nuget.org/
[NuGet packages]: http://www.nuget.org/packages?q=oxyplot
[Portable Class Library]: http://msdn.microsoft.com/en-us/library/vstudio/gg597391(v=vs.100).aspx
[pdf]: /documentation/export-pdf
[png]: /documentation/export-png
[svg]: /documentation/export-svg

[oxyplot.org/documentation]: /documentation
[support]: /support
[contributions]: /documentation/contributions
[getting started]: /documentation/getting-started
[supported platforms]: /documentation/supported-platforms
[announcements]: /announcements
[atom feed]: http://oxyplot.org/atom.xml

[repository]: https://github.com/oxyplot/oxyplot
[Source/Examples]: https://github.com/oxyplot/oxyplot/tree/master/Source/Examples
[contributors]: https://github.com/oxyplot/oxyplot/graphs/contributors

[example browser]: http://resources.oxyplot.org/examplebrowser/

[discussion.oxyplot.org]: http://oxyplot.userecho.com/
[chat room]: https://gitter.im/oxyplot/oxyplot
[Stack Overflow]: http://stackoverflow.com/questions/tagged/oxyplot?sort=newest
[Xamarin forum]: http://forums.xamarin.com/search?Search=oxyplot
[twitter]: https://twitter.com/search?q=oxyplot
[twitter-hashtag]: https://twitter.com/search?q=%23oxyplot&src=hash

[xamarin-component]: http://components.xamarin.com/
[xamarin-mac]: http://xamarin.com/mac
[mono-mac]: http://www.mono-project.com/MonoMac

[Jetbrains]: http://www.jetbrains.com/
[ReSharper]: http://www.jetbrains.com/resharper/
[dotCover]: http://www.jetbrains.com/dotcover/index.html?topDC
[NDepend]: http://www.ndepend.com/
[Red Gate Software]: http://www.red-gate.com/
[ANTS]: http://www.red-gate.com/products/dotnet-development/ants-performance-profiler/
[Xamarin]: http://www.xamarin.com/
[OzCode]: http://www.oz-code.com/
[OzCode VS extension]: http://visualstudiogallery.msdn.microsoft.com/36925113-cdce-4953-a5d6-fb3d2912dad7
[UserEcho]: http://www.userecho.com/

[jetbrains-banner]: http://www.jetbrains.com/img/banners/Codebetter.png
