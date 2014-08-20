---
layout: page
title: Export to PNG
---

The PNG exporters are implemented in the platform specific libraries (OxyPlot.Wpf, OxyPlot.WindowsForms etc.).

Write a PNG file:

``` csharp
using (var stream = File.Create(fileName))
{
    var pngExporter = new PngExporter();
    pngExporter.Export(plotModel, stream, 600, 400, Brushes.White);
}
```

Copy to clipboard:

``` csharp
using (var stream = new MemoryStream())
{
    var pngExporter = new PngExporter();
    pngExporter.Export(plotModel, stream, 600, 400, Brushes.White);
}

// TODO : write content of stream to clipboard
```
