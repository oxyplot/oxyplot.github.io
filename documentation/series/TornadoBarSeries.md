---
layout: page
title: TornadoBarSeries
---

A `TornadoBarSeries` shows columns defined by a minimum, maximum and base value.

![TornadoBarSeries](/public/images/documentation/series/TornadoBarSeries.png)


### Tracker

The `TrackerFormatString` property is used to format the string shown in the [tracker](../tracker). The format string may use the following arguments:

- `{0}` the title of the series
- `{1}` the title of the category axis
- `{2}` the category
- `{3}` the title of the value axis
- `{4}` the minimum or maximum value
- `{PropertyX}` the value of `PropertyX` in the item (extended format string syntax)

To show the value with one digit, use the format string `"{4:0.0}"`.

If an item was hit, it is also possible to use the extended format string syntax, e.g. `{PropertyX:0.##}`, where the value of `PropertyX` will be found by reflection of the item.

The default format string for `TornadoBarSeries` is `"{0}\n{1}: {2}\n{3}: {4}"`

See [MSDN](http://msdn.microsoft.com/en-us/library/system.string.format(v=vs.110).aspx) for more information about format strings.

The `TrackerKey` property may be used to specify a [custom tracker](../tracker). This makes it possible to use different trackers for each series.


### Example

``` csharp
var model = new PlotModel { Title = "TornadoBarSeries" };
```
