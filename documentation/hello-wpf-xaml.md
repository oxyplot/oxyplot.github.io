---
layout: page
title: WPF example (XAML)
---

This example shows how to create a WPF application where the content of the plot is defined in XAML.

### Create project
Start Visual Studio and select "FILE -> New -> Project..." to create a new WPF application:

![New project](/public/images/documentation/wpf-new-project.png)

### Add references

You need references to the OxyPlot and OxyPlot.Wpf assemblies. The easiest way to add these is to right click on the "References" item in the Solution Explorer and select "Manage NuGet Packages..." (this requires that the "NuGet Package Manager" extension is installed):

![Add reference](/public/images/documentation/wpf-add-reference.png)

In the "Manage NuGet packages" dialog, search for "OxyPlot" and select the "OxyPlot.Wpf" package:

![Install package](/public/images/documentation/wpf-install-package.png)

You can also use the [http://docs.nuget.org/docs/start-here/using-the-package-manager-console|Package Manager Console] to install the package:

```
PM> Install-Package OxyPlot.Wpf
```

### Create a view model

Then create a class that defines the data to be plotted.

``` csharp
@include ..\Source\Examples\DocumentationExamples\HelloWorld\WpfApplication2\MainViewModel.cs
```

### Create the view

Define the namespace in the `Window` element, set the `DataContext` and add a `PlotView` control:

``` xml
@include ..\Source\Examples\DocumentationExamples\HelloWorld\WpfApplication2\MainWindow.xaml
```

The application should now look like this:

![Screen shot](/public/images/documentation/wpf-example2.png)

The source code can be found in `Documentation\Examples\WpfApplication2`.
