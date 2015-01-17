---
layout: page
title: Features
---

// TODO //

### Plot types

- XY (horizontal and vertical axes)
- Cartesian (same scale on X and Y axis)
- Polar
- Pie chart

### Axes

// TODO

It is possible to extend with custom axis types.

### Series

// TODO

Different types of series can be added to the same plot.

It is possible to extend with custom series types.

### Annotations

// TODO

It is possible to extend with custom annotation types.

### Output file formats

The plots can be exported to the following raster and vector file formats:

- [png](./export-png)
- [svg](./export-svg)
- [pdf](./export-pdf)

### Limitations

- the plot controls are not subscribing to `INotifyPropertyChanged` and `INotifyCollectionChanged` events. You must manually refresh the plots when changing your data.
- no animations
- no gradient or hatch brushes
