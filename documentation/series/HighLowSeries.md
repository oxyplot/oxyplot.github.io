---
layout: page
title: HighLowSeries
---

A `HighLowSeries` shows a set of points. The points can also have a size and color value.

![HighLowSeries](/public/images/documentation/series/HighLowSeries.png)


### Tracker

The `TrackerFormatString` property is used to format the string shown in the [tracker](../tracker). The format string may use the following arguments:

- `{0}` the title of the series
- `{1}` the title of the x-axis
- `{2}` the x-value
- `{3}` the high value
- `{4}` the low value
- `{5}` the open value
- `{6}` the close value
- `{PropertyX}` the value of `PropertyX` in the item (extended format string syntax)

To show the close value with one digit, use the format string `"{6:0.0}"`.

If an item was hit, it is also possible to use the extended format string syntax, e.g. `{PropertyX:0.##}`, where the value of `PropertyX` will be found by reflection of the item.

The default format string for `HighLowSeries` is `"{0}\n{1}: {2}\nHigh: {3:0.###}\nLow: {4:0.###}\nOpen: {5:0.###}\nClose: {6:0.###}"`

See [MSDN](http://msdn.microsoft.com/en-us/library/system.string.format(v=vs.110).aspx) for more information about format strings.

The `TrackerKey` property may be used to specify a [custom tracker](../tracker). This makes it possible to use different trackers for each series.


### Example

``` csharp
var model = new PlotModel { Title = "HighLowSeries" };
```
