---
layout: page
title: Windows.Forms example
---

### Create project
Start Visual Studio and select "FILE -> New -> Project..." to create a new Windows Forms application:

![New project](/public/images/documentation/windows-forms-new-project.png)

### Add references

You need references to the OxyPlot and OxyPlot.WindowsForms assemblies. The easiest way to do this is to right click on the "References" item in the Solution Explorer and select "Manage NuGet Packages..." (this requires that the "NuGet Package Manager" extension is installed):

![Add reference](/public/images/documentation/windows-forms-add-reference.png)

In the "Manage NuGet packages" dialog, search for "OxyPlot" in the top-right search textbox. 
Select the "OxyPlot.WindowsForms" package and click install:

![Install package](/public/images/documentation/windows-forms-install-package.png)

You can also use the [Package Manager Console](http://docs.nuget.org/docs/start-here/using-the-package-manager-console) to install the package:

```
PM> Install-Package OxyPlot.WindowsForms
```

### Add a plot view

TODO (add component to toolbox?)

### Create the plot model

``` csharp
namespace WindowsFormsApplication1
{
    using System;
    using System.Windows.Forms;

    using OxyPlot;
    using OxyPlot.Series;

    public partial class Form1 : Form
    {
        public Form1()
        {
            this.InitializeComponent();
            var myModel = new PlotModel { Title = "Example 1" };
            myModel.Series.Add(new FunctionSeries(Math.Cos, 0, 10, 0.1, "cos(x)"));
            this.plot1.Model = myModel;
        }
    }
}
```

The application should now look like this:

![Screen shot](/public/images/documentation/windows-forms-example1.png)

The source code can be found in the [HelloWorld\WindowsFormsApplication1](https://github.com/oxyplot/documentation-examples/tree/master/HelloWorld/WindowsFormsApplication1) folder in the [documentation-examples](https://github.com/oxyplot/documentation-examples) repository.