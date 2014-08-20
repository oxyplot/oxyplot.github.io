---
layout: page
title: Export to PDF
---

You have two options when you want to export your plots to PDF. You can use the `OxyPlot.PdfExporter` that is included in the portable OxyPlot core library, or the `OxyPlot.Pdf.PdfExporter` included in the OxyPlot.Pdf library. The latter depends on [PdfSharp][pdfsharp]/[SilverPdf][silverpdf] and is not portable.

### Core Pdf writer

- Simple PDF export is included in OxyPlot core library
- There are limitations on text encoding, fonts and images

``` csharp
using (var stream = File.Create(fileName))
{
    var pdfExporter = new PdfExporter();
    pdfExporter.Export(plotModel, stream, 600, 400);
}
```

See also the section about [portable documents](./portable-documents) that can be used to create general PDF files.

### OxyPlot.Pdf

- based on the [PdfSharp][pdfsharp] / [SilverPdf][silverpdf] open-source projects
- better handling of fonts and images

[pdfsharp]: http://www.pdfsharp.net/
[silverpdf]: https://silverpdf.codeplex.com
