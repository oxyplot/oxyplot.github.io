---
layout: page
title: LineSeries
---

A `LineSeries` is used to render data as a polyline in the plot. It is also possible to render markers at each point of the polyline.

![LineSeries](/public/images/documentation/series/LineSeries.png)

### Visibility

The visibility of the series can be controlled by the `IsVisible` property. The default value is `true`. If set to `false`, the series will not be rendered.

### Title

The `Title` property defines the title to show in the plot [legend](../legend). The default value is `null` (not shown in legend).

### Background

If the `Background` property is set to a color, the area defined by the X and Y axes will be filled with the specified color. The default value is `Undefined` (not showing a background).

### Axes

By default, the `LineSeries` will use the default horizontal and vertical axes in the parent `PlotModel`. If there are more than one horizontal/vertical axis, the axes can be specified by the `XAxisKey` and `YAxisKey` properties. This requires the `Key` property to be set on the desired axes.

### Data

Use the `Points` collection to add data to the `LineSeries`:

``` cs
lineSeries1.Points.Add(new DataPoint(0, 0));
lineSeries1.Points.Add(new DataPoint(100, 40));
```

Alternatively, you can specify a collection in the `ItemsSource` property.

- If the `Mapping` property is set, each element in the collection will be transformed
- If the collection is a list of `DataPoint`, it will be used with no mapping
- If the `DataFieldX` and `DataFieldY` properties are set, each element of the collection will be reflected to create a data point

### Tracker

The `TrackerFormatString` property is used to format the string shown in the [tracker](../tracker). The format string may use the following arguments:

- `{0}` the title of the current series
- `{1}` the title of the x-axis
- `{2}` the x-value
- `{3}` the title of the y-axis
- `{4}` the y-value
- `{PropertyX}` the value of `PropertyX` in the nearest item (extended format string syntax)

To show the x and y values with one digit, use the format string `"{3:0.0},{5:0.0}"`.

If an item was hit, it is also possible to use the extended format string syntax, e.g. `{PropertyX:0.##}`, where the value of `PropertyX` will be found by reflection of the item.

The default format string for `LineSeries` is `"{0}\n{1}: {2}\n{3}: {4}"`

See [MSDN](http://msdn.microsoft.com/en-us/library/system.string.format(v=vs.110).aspx) for more information about format strings.

The `CanTrackerInterpolatePoints` property should be set to `false` if the tracker should not interpolate values between the points. The default value is `true`.

The `TrackerKey` property may be used to specify a [custom tracker](../tracker). This makes it possible to use different trackers for each series.

### Color

The `Color` defines the color of the line. The default value is `Automatic`. In this case the color will be set automatically from the colors specified in the `DefaultColors` collection of the parent `PlotModel`.

### Line style

The `StrokeThickness` property defines the thickness of the line. The default value is `2`.

The `LineStyle` property defines the style of the line. The default value is `Undefined`, where the style will be set automatically.
The `Dashes` property can be used to override the `LineStyle` with a custom dash array.

The `LineJoin` property specifies how to join the line. The default value is `Bevel` which has the best performance. `Miter` and `Round` can also be used, note the differences on sharp corners. 

### Markers

Use the `MarkerType` to specify the shape of the markers. The default is `None`. If the type is set to `Custom`, a custom outline should be specified in the `MarkerOutline` property.

The size of the markers is specified in by `MarkerSize`. The default value is `3` [device independent units](../units).

The colors of the markers is specified in the `MarkerStroke` and `MarkerFill` properties. The thickness of the outline is specified in `MarkerStrokeThickness`. The default value is `1` [device independent unit](../units).

### Interpolation

The `Smooth` property can be used to render the points as a smooth curve. When set to `true`, the points will define control points for a [canoncial spline](http://www.charlespetzold.com/blog/2009/01/canonical-splines-in-wpf-and-silverlight.html). 

### Labels

If the `LabelFormatString` is set, labels will be rendered on each data point. The default value is `null`. The format string can contain the following parameters:

- `{0}` the x-value
- `{1}` the y-value
- `{PropertyX}` where `PropertyX' is the name of a property in the actual item

The `LabeLMargin` property defines the distance from the point to the label.

### Legend on line

To add a legend on the line, set the `LineLegendPosition` to `Start` or `End`. The default value is `None`.

### Broken lines

Data points that contains `NaN` will create breaks in the line. The default behaviour is not to render the segments over these breaks. If the `BrokenLineThickness` is set, the segments will be rendered with `BrokenLineColor` and `BrokenLineStyle`.

### Performance

The `MinimumSegmentLength` property defines the minimum length of a line segment that will be rendered. The default value is `2` [device independent unit](../units).

The `MarkerResolution` property can be used to decimate the markers. The value is given in  [device independent unit](../units). The default is `0` (disabled).

The `Decimator` delegate can be used to reduce the actual rendered points.

### Examples

``` csharp
var model = new PlotModel { Title = "LineSeries" };
var lineSeries = new LineSeries();
lineSeries.Points.Add(new DataPoint(0, 0));
lineSeries.Points.Add(new DataPoint(10, 4));
lineSeries.Points.Add(new DataPoint(30, 2));
lineSeries.Points.Add(new DataPoint(40, 12));
model.Series.Add(lineSeries);
```

![LineSeries](/public/images/documentation/series/LineSeries-Example1.png)

The line can be changed to a smooth curve by interpolating with a canonical spline:

``` csharp
lineSeries.Smooth = true;
```

![LineSeries](/public/images/documentation/series/LineSeries-Example2.png)

Then add markers by setting

``` csharp
lineSeries.MarkerType = MarkerType.Circle;
```

![LineSeries](/public/images/documentation/series/LineSeries-Example3.png)
