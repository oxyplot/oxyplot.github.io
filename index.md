---
layout: home
published: true
---

![Example plot]

OxyPlot is a cross-platform plotting library for .NET. 

The code is licensed under the MIT license. This is a very permissive and corporate friendly license. See [opensource.org](http://opensource.org/licenses/MIT) and [tl;dr](https://tldrlegal.com/license/mit-license) for more details.

The core library is a [Portable Class Library] that can be used on different platforms. Custom controls are implemented for WPF, Windows 8, Windows Phone, Windows Phone Silverlight, Windows Forms, Silverlight, GTK#, Xwt, Xamarin.iOS, Xamarin.Android, Xamarin.Forms and Xamarin.Mac.

- The documentation is located at [https://oxyplot.readthedocs.io/]
- The latest stable release can be found at [NuGet][NuGet packages]
- The latest pre-release can be found at [MyGet][MyGet packages]

### Supported platforms

See the [supported platforms] section in the documentation.

### Features

OxyPlot contains many different types of axes and series. If you need some functionality that is not included in the library, you can also create a derived class and override the rendering implementation.

The plots can be exported to file formats like [png], [pdf] and [svg].

See the [features] section for more information. 

### Getting started

1. Use the [NuGet] package manager to add the latest [stable][NuGet packages] or [pre-release][MyGet packages] package for your platform. 
2. Add a `PlotView` control to your user interface. 
3. Create a `PlotModel`
4. Bind or assign the `PlotModel` to the `Model` property of the control.

See the [getting started] section for more information about each platform. 

### Xamarin Forms

Make sure you reference and initialize the OxyPlot platform renderers, otherwise you will see nothing. See [getting started with Xamarin Forms] for more information. 

### Examples

Example code can be found in the [Source/Examples] folder in the [repository]. 

### Documentation

The documentation can be found at [docs.oxyplot.org]. Note that it is under construction. Please contribute!

### Questions

Use the discussion forum at [oxyplot.userecho.com] if you have questions regarding the library. You can also try the [chat room], [Stack Overflow] or the [Xamarin forum].

### Issues

Feature requests and bugs should be added to the [issues] section at GitHub. Please do not use the issues section for questions.

### Announcements

News about the library can be found under [announcements]. There is also an [atom feed] for the posts.

### Contribute

This project is continuously evolving and any kind of help is greatly appreciated. See the [contributions] page for more information about how to get involved.

### Thanks

The project is supported by

- [Jetbrains]
  - [ReSharper]
  - [dotCover]
- [NDepend]
  - [NDepend v6][NDepend]
- [Red Gate Software]
  - [ANTS]
- [Xamarin]
  - [Xamarin Studio][Xamarin]
- [OzCode]
  - [OzCode VS extension]
- [UserEcho]

[Example plot]: /public/images/normal-distributions.png
[NuGet]: http://www.nuget.org/
[NuGet packages]: {{ site.nuget }}
[MyGet packages]: {{ site.myget }}
[Portable Class Library]: http://msdn.microsoft.com/en-us/library/vstudio/gg597391(v=vs.100).aspx
[pdf]: https://oxyplot.readthedocs.io/en/latest/export/export-pdf.html
[png]: https://oxyplot.readthedocs.io/en/latest/export/export-png.html
[svg]: https://oxyplot.readthedocs.io/en/latest/export/export-svg.html

[features]: https://oxyplot.readthedocs.io/en/latest/introduction/features.html
[contributions]: https://github.com/oxyplot/oxyplot/blob/develop/.github/CONTRIBUTING.md
[getting started]: https://oxyplot.readthedocs.io/en/latest/getting-started/
[getting started with Xamarin Forms]: https://oxyplot.readthedocs.io/en/latest/getting-started/hello-xamarin-forms.html
[supported platforms]: https://oxyplot.readthedocs.io/en/latest/introduction/
[announcements]: /announcements
[atom feed]: http://oxyplot.org/atom.xml
[https://oxyplot.readthedocs.io/]: https://oxyplot.readthedocs.io/en/latest/

[repository]: https://github.com/oxyplot/oxyplot
[Source/Examples]: https://github.com/oxyplot/oxyplot/tree/master/Source/Examples
[contributors]: https://github.com/oxyplot/oxyplot/graphs/contributors
[issues]: https://github.com/oxyplot/oxyplot/issues/

[oxyplot.userecho.com]: https://oxyplot.userecho.com/
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
