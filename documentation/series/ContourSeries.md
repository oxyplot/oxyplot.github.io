---
layout: page
title: ContourSeries
---

A `ContourSeries` renders a 2D array of values as contours.

![ContourSeries](/public/images/documentation/series/ScatterSeries.png)


### Tracker

The `TrackerFormatString` property is used to format the string shown in the [tracker](../tracker). The format string may use the following arguments:

- `{0}` the title of the series
- `{1}` the title of the x-axis
- `{2}` the x-value
- `{3}` the title of the y-axis
- `{4}` the y-value
- `{5}` the title of the contour level axis
- `{6}` the contour level
- `{PropertyX}` the value of `PropertyX` in the item (extended format string syntax)

To show the contour level with one digit, use the format string `"{6:0.0}"`.

If an item was hit, it is also possible to use the extended format string syntax, e.g. `{PropertyX:0.##}`, where the value of `PropertyX` will be found by reflection of the item.

The default format string for `ContourSeries` is `"{0}\n{1}: {2}\n{3}: {4}\n{5}: {6}"`

See [MSDN](http://msdn.microsoft.com/en-us/library/system.string.format(v=vs.110).aspx) for more information about format strings.

The `TrackerKey` property may be used to specify a [custom tracker](../tracker). This makes it possible to use different trackers for each series.


### Example

``` csharp
var model = new PlotModel { Title = "ContourSeries" };
```
