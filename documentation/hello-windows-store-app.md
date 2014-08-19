---
layout: page
title: Windows Store App example
---

This example shows how to create a Windows Store app where the content of the plot is defined in code.

### Create project
Start Visual Studio and select "FILE -> New -> Project..." to create a new Windows Store app:

![New project](/public/images/documentation/windows-store-app-new-project.png)

### Add references

You need references to the OxyPlot and OxyPlot.Metro assemblies. The easiest way to do this is to right click on the "References" item in the Solution Explorer and select "Manage NuGet Packages..." (this requires that the "NuGet Package Manager" extension is installed):

![Add reference](/public/images/documentation/windows-store-app-add-reference.png)

In the "Manage NuGet packages" dialog, search for "OxyPlot" in the top-right search textbox. 
Select the "OxyPlot.Metro" package and click install:

![Install package](/public/images/documentation/windows-store-app-install-package.png)

You can also use the [Package Manager Console](http://docs.nuget.org/docs/start-here/using-the-package-manager-console) to install the package:

```
PM> Install-Package OxyPlot.Metro
```

### Create a view model

Add a class that creates a `PlotModel` and a `FunctionSeries`.

``` csharp
@include ..\Source\Examples\DocumentationExamples\HelloWorld\WindowsStoreApp1\MainViewModel.cs
```

### Create the view

Define the namespace in the `Window` element, set the `DataContext` and add a `PlotView` control:

``` xml
@include ..\Source\Examples\DocumentationExamples\HelloWorld\WindowsStoreApp1\MainPage.xaml
```

The application should now look like this:

![Screen shot](/public/images/documentation/windows-store-app-example1.png)

The source code can be found in `Documentation\Examples\WindowsStoreApp1`.
