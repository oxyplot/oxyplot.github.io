---
layout: page
title: ScatterSeries
---

A `ScatterSeries` shows a set of points. The points can also have a size and color value.

``` csharp
var model = new PlotModel { Title = "ScatterSeries" };
var scatterSeries = new ScatterSeries { MarkerType = MarkerType.Circle };
var r = new Random(314);
for (int i = 0; i < 100; i++)
{
    var x = r.NextDouble();
    var y = r.NextDouble();
    var size = r.Next(5, 15);
    var colorValue = r.Next(100, 1000);
    scatterSeries.Points.Add(new ScatterPoint(x, y, size, colorValue));
}

model.Series.Add(scatterSeries);
model.Axes.Add(new LinearColorAxis { Position = AxisPosition.Right, Palette = OxyPalettes.Jet(200) });
```
