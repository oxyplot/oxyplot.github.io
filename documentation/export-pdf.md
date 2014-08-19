---
layout: page
title: Export to PDF
---

// TODO //

### Core Pdf writer

- Simple PDF export is included in OxyPlot core library
- Limitations (text encoding, fonts, images)

``` csharp
using (var stream = File.Create(fileName))
{
    var pdfExporter = new PdfExporter();
    pdfExporter.Export(plotModel, stream, 600, 400);
}
```

See also the section about [portable documents](./portable-documents) that can be used to create general PDF files.

### OxyPlot.Pdf

- based on the [PdfSharp](http://www.pdfsharp.net/) / [SilverPdf](https://silverpdf.codeplex.com) open-source projects
- better handling of fonts and images


