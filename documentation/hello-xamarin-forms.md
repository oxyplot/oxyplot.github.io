---
layout: page
title: Xamarin.Forms example
---

This example shows how to create a [Xamarin.Forms][forms] app where bot the user interface and the plot is defined in portable code.

### Create the project

Start Visual Studio and select in the blank Xamarin.Forms app template.

### Add references

Add the `OxyPlot.XamarinForms` NuGet package in both the portable and platform specific projects.

### Initialize renderers

You need to initialize the OxyPlot renderers by adding the following call just before `Xamarin.Forms.Forms.Init()`:

- iOS: `OxyPlot.XamarinFormsIOS.Forms.init();`
- Android: `OxyPlot.XamarinFormsAndroid.Forms.init();`
- WinPhone: `OxyPlot.XamarinFormsWinPhone.Forms.Init();`
Add a class that creates a `PlotModel` and a `FunctionSeries`.

### Add the `PlotView` to your form (in code)

In the portable/shared app project, add the plot view

``` csharp
public static Page GetMainPage()
{
    return new ContentPage
    {
        Content = new PlotView
        {
            Model = new PlotModel { Title = "Hello Xamarin.Forms" },
            VerticalOptions = LayoutOptions.Fill,
            HorizontalOptions = LayoutOptions.Fill,
        },
    };
}
```

### Add the `PlotView` to your form (XAML)

TODO

### Binding to a `PlotModel`

TODO

### Adding a `PlotController`

TODO

### References

The source code can be found in the [HelloWorld\XamarinFormsApp1](https://github.com/oxyplot/documentation-examples/tree/master/HelloWorld/XamarinFormsApp1) folder in the [documentation-examples](https://github.com/oxyplot/documentation-examples) repository.

[forms]: http://xamarin.com/forms