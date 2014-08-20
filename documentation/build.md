---
layout: page
title: Building OxyPlot
---

### Requirements

- .NET 3.5 or later
- Build tool with support for Portable Class Libraries (Visual Studio 201x, MonoDevelop, Xamarin Studio, MsBuild)
- StyleCop (only required for builds on Windows)

The OxyPlot solutions can be opened in

- VS 2010 (with the [Portable Library Tools][portable-tools] extension)
- VS 2012 (with the latest update)
- VS 2013
- MonoDevelop
- Xamarin Studio (for GTK#, Android, iOS and OSX apps)

VS Express does not support Portable Class Libraries, and cannot be used to build OxyPlot. But, you can use VS Express to build applications that reference the OxyPlot assemblies!

Depending on what platform you want to build, you may need to install extra SDKs or target framework profiles

- [.NET 3.5](http://www.microsoft.com/en-us/download/details.aspx?id=22)
- [.NET 4.0](http://www.microsoft.com/nb-no/download/details.aspx?id=17851)
- [.NET 4.5](http://www.microsoft.com/nb-no/download/details.aspx?id=30653)
- [Portable library tools 2.0](http://visualstudiogallery.msdn.microsoft.com/b0e0b5e9-e138-410b-ad10-00cb3caf4981/)
- [Microsoft .NET Portable Library Reference Assemblies 4.6](http://www.microsoft.com/en-us/download/details.aspx?id=40727)
- [StyleCop](http://stylecop.codeplex.com/)
- [Silverlight 4 SDK](http://www.microsoft.com/en-us/download/details.aspx?id=7335)
- [Silverlight 5 SDK](http://www.microsoft.com/en-us/download/details.aspx?id=28359)
- [Windows Store App](http://msdn.microsoft.com/en-us/windows/desktop/bg162891.aspx)
- [GTK#](http://www.mono-project.com/GtkSharp)
- [Xamarin.iOS](http://xamarin.com/ios)
- [Xamarin.Android](http://xamarin.com/android)
- [Xamarin.Mac](http://xamarin.com/mac)

### Obtain the source code

OxyPlot is using [Git][git] distributed version control system (DVCS). To obtain the code, it is recommended to install one of the following Git clients

- [GitHub for Windows][github-for-windows]
- [TortoiseGit][tortoise-git] (Windows shell extension)
- [SourceTree][source-tree] (for Windows and Mac, also supports Git)
- [Git][git] (command line)

Clone the repository from `https://github.com/oxyplot/oxyplot.git`.

```
git clone https://github.com/oxyplot/oxyplot.git
```

If you don't want to use Git, you can also obtain the complete source code from the [repository page][repo]. Click the "Download Zip" button.

### Build

It should be possible to open the solution and build without any additional steps.
You can also build the source code by scripts in the `Build/` folder.

### Build output

The build output of the *Release* configurations are placed in the `Output/` folder. The output of the *Debug* configurations are placed under the `Source/*/bin/Debug` folders. 

### Additional information

OxyPlot is currently being built by [Visual Studio 2013](http://www.microsoft.com/visualstudio) on a Windows 8.1 virtual machine (running in [VirtualBox](https://www.virtualbox.org). The build system is based on [TeamCity](http://www.jetbrains.com/teamcity/) and trigs the build on every code check-in. When all code is compiled and all unit tests have passed, the build machine is automatically pushing [NuGet](http://nuget.org) packages.

The build steps are described in the `Build/BuildSteps.txt` file.

![Build machine screen shot](/public/images/documentation/build-machine.png)

[repo]: https://github.com/oxyplot/oxyplot
[git]: http://git-scm.com/
[tortoise-git]: https://code.google.com/p/tortoisegit/
[source-tree]: http://www.sourcetreeapp.com/|SourceTree
[github-for-windows]: https://windows.github.com/
[portable-tools]: http://visualstudiogallery.msdn.microsoft.com/b0e0b5e9-e138-410b-ad10-00cb3caf4981
