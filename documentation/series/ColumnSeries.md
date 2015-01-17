---
layout: page
title: ColumnSeries
---

A `ColumnSeries` shows the data set as vertical columns.

![ColumnSeries](/public/images/documentation/series/ColumnSeries.png)


### Tracker

The `TrackerFormatString` property is used to format the string shown in the [tracker](../tracker). The format string may use the following arguments:

- `{0}` the title of the series
- `{1}` the category
- `{2}` the column value
- `{PropertyX}` the value of `PropertyX` in the item (extended format string syntax)

To show the column value with one digit, use the format string `"{2:0.0}"`.

If an item was hit, it is also possible to use the extended format string syntax, e.g. `{PropertyX:0.##}`, where the value of `PropertyX` will be found by reflection of the item.

The default format string for `ColumnSeries` is `"{0}\n{1}: {2}"`

See [MSDN](http://msdn.microsoft.com/en-us/library/system.string.format(v=vs.110).aspx) for more information about format strings.

The `TrackerKey` property may be used to specify a [custom tracker](../tracker). This makes it possible to use different trackers for each series.

### Example

``` csharp
var model = new PlotModel { Title = "ColumnSeries" };
```
