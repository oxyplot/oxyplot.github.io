---
layout: page
title: WPF example
---

This example shows how to create a WPF application where the content of the plot is defined in code.

### Create project

Start Visual Studio and select "FILE -> New -> Project..." to create a new WPF application:

![New project](/public/images/documentation/wpf-new-project.png)

### Add references

You need references to the OxyPlot and OxyPlot.Wpf assemblies. The easiest way to add these is to right click on the "References" item in the Solution Explorer and select "Manage NuGet Packages..." (this requires that the "NuGet Package Manager" extension is installed):

![Add reference](/public/images/documentation/wpf-add-reference.png)

In the "Manage NuGet packages" dialog, search for "OxyPlot" and select the "OxyPlot.Wpf" package:

![Install package](/public/images/documentation/wpf-install-package.png)

You can also use the [Package Manager Console](http://docs.nuget.org/docs/start-here/using-the-package-manager-console) to install the package:

```
PM> Install-Package OxyPlot.Wpf
```

### Create a view model

Add a class that creates a `PlotModel` with a `FunctionSeries`.

``` csharp
namespace WpfApplication1
{
    using System;

    using OxyPlot;
    using OxyPlot.Series;

    public class MainViewModel
    {
        public MainViewModel()
        {
            this.MyModel = new PlotModel { Title = "Example 1" };
            this.MyModel.Series.Add(new FunctionSeries(Math.Cos, 0, 10, 0.1, "cos(x)"));
        }

        public PlotModel MyModel { get; private set; }
    }
}
```

### Create the view

Define the namespace in the `Window` element, set the `DataContext` and add a `PlotView` control:

``` xml
<Window x:Class="WpfApplication1.MainWindow"
        xmlns="http://schemas.microsoft.com/winfx/2006/xaml/presentation"
        xmlns:x="http://schemas.microsoft.com/winfx/2006/xaml" xmlns:oxy="http://oxyplot.codeplex.com"
        xmlns:local="clr-namespace:WpfApplication1"
        Title="Example 1 (WPF)" Height="350" Width="525">
    <Window.DataContext>
        <local:MainViewModel/>
    </Window.DataContext>
    <Grid>
        <oxy:PlotView Model="{Binding MyModel}"/>
    </Grid>
</Window>
```

The application should now look like this:

![Screen shot](/public/images/documentation/wpf-example1.png)

The source code can be found in the [documentation-examples](https://github.com/oxyplot/documentation-examples) repository in the folder [HelloWorld\WpfApplication1](https://github.com/oxyplot/documentation-examples/tree/master/HelloWorld/WpfApplication1).