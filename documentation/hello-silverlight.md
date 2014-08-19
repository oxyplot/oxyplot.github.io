---
layout: page
title: Silverlight example
---

This example shows how to create a Silverlight application where the content of the plot is defined in code.

### Create project
Start Visual Studio and select "FILE -> New -> Project..." to create a new Silverlight application:

![New project](/public/images/documentation/silverlight-new-project.png)

### Add references

You need references to the OxyPlot and OxyPlot.Silverlight assemblies. The easiest way to do this is to right click on the "References" item in the Solution Explorer and select "Manage NuGet Packages..." (this requires that the "NuGet Package Manager" extension is installed):

![Add reference](/public/images/documentation/silverlight-add-reference.png)

In the "Manage NuGet packages" dialog, search for "OxyPlot" in the top-right search textbox. 
Select the "OxyPlot.Silverlight" package and click install:

![Install package](/public/images/documentation/silverlight-install-package.png)

You can also use the [Package Manager Console](http://docs.nuget.org/docs/start-here/using-the-package-manager-console) to install the package:

```
PM> Install-Package OxyPlot.Silverlight
```

### Create a view model

Add a class that creates a `PlotModel` and a `FunctionSeries`.

``` csharp
@include ..\Source\Examples\DocumentationExamples\HelloWorld\SilverlightApplication1\MainViewModel.cs
```

### Create the view

Define the namespace in the `Window` element, set the `DataContext` and add a `PlotView` control:

``` xml
@include ..\Source\Examples\DocumentationExamples\HelloWorld\SilverlightApplication1\MainPage.xaml
```

The application should now look like this:

![Screen shot](/public/images/documentation/silverlight-example1.png)

The source code can be found in `Documentation\Examples\SilverlightApplication1`.
