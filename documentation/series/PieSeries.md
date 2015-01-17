---
layout: page
title: PieSeries
---

A `PieSeries` renders a pie chart. Only one pie series is supported per `PlotModel`.

![PieSeries](/public/images/documentation/series/PieSeries.png)


### Tracker

The `TrackerFormatString` property is used to format the string shown in the [tracker](../tracker). The format string may use the following arguments:

- `{0}` the title of the series
- `{1}` the label of the pie slice
- `{2}` the value of the pie slice
- `{3}` the percentage of the pie slice
- `{PropertyX}` the value of `PropertyX` in the item (extended format string syntax)

To show the values with one digit, use the format string `"{2:0.0}"`.

If an item was hit, it is also possible to use the extended format string syntax, e.g. `{PropertyX:0.##}`, where the value of `PropertyX` will be found by reflection of the item.

The default format string for `PieSeries` is `"{1}: {2:0.###} ({3:P1})"`

See [MSDN](http://msdn.microsoft.com/en-us/library/system.string.format(v=vs.110).aspx) for more information about format strings.

### Example

``` csharp
var model = new PlotModel { Title = "PieSeries" };
```
