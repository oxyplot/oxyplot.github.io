---
layout: page
title: RectangleBarSeries
---

A `RectangleBarSeries` shows rectangles defined by minimum and maximum x and y values.

![RectangleBarSeries](/public/images/documentation/series/RectangleBarSeries.png)


### Tracker

The `TrackerFormatString` property is used to format the string shown in the [tracker](../tracker). The format string may use the following arguments:

- `{0}` the title of the series
- `{1}` the title of the x-axis
- `{2}` the minimum x-value (X0)
- `{3}` the maximum x-value (X1)
- `{4}` the title of the y-axis
- `{5}` the minimum y-value (Y0)
- `{6}` the maximum y-value (Y1)
- `{PropertyX}` the value of `PropertyX` in the item (extended format string syntax)

To show the minimum x and y values with one digit, use the format string `"{2:0.0},{5:0.0}"`.

If an item was hit, it is also possible to use the extended format string syntax, e.g. `{PropertyX:0.##}`, where the value of `PropertyX` will be found by reflection of the item.

The default format string for `RectangleBarSeries` is `"{0}\n{1}: {2} {3}\n{4}: {5} {6}"`

See [MSDN](http://msdn.microsoft.com/en-us/library/system.string.format(v=vs.110).aspx) for more information about format strings.

The `TrackerKey` property may be used to specify a [custom tracker](../tracker). This makes it possible to use different trackers for each series.


### Example

``` csharp
var model = new PlotModel { Title = "RectangleBarSeries" };
```
