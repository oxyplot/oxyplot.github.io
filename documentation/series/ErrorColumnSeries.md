---
layout: page
title: ErrorColumnSeries
---

A `ErrorColumnSeries` shows a column series with error indicators.

![ErrorColumnSeries](/public/images/documentation/series/ErrorColumnSeries.png)


### Tracker

The `TrackerFormatString` property is used to format the string shown in the [tracker](../tracker). The format string may use the following arguments:

- `{0}` the title of the series
- `{1}` the title of the x-axis
- `{2}` the value
- `{Error}` the error value
- `{PropertyX}` the value of `PropertyX` in the item (extended format string syntax)

To show the error value with one digit, use the format string `"{Error:0.0}"`.

If an item was hit, it is also possible to use the extended format string syntax, e.g. `{PropertyX:0.##}`, where the value of `PropertyX` will be found by reflection of the item.

The default format string for `ErrorColumnSeries` is `"{0}\n{1}: {2}, Error: {Error:0.###}"`

See [MSDN](http://msdn.microsoft.com/en-us/library/system.string.format(v=vs.110).aspx) for more information about format strings.

The `TrackerKey` property may be used to specify a [custom tracker](../tracker). This makes it possible to use different trackers for each series.


### Example

``` csharp
var model = new PlotModel { Title = "ErrorColumnSeries" };
```
