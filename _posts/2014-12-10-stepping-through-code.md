---
layout: post
title: Stepping through OxyPlot code while debugging
---

It is now possible to step through the OxyPlot code while debugging your software. This is available in the latest prerelease and will be available in the next official version. Below is an image that shows the actual OxyPlot code without local source files of OxyPlot:

[GitLink example]: /public/images/gitlink-example.png

The advantage of this feature is that the end-developers can get a better understanding of the inner workings of OxyPlot. This is great to encourage pull requests or to find out why something is not working as expected.

To enable stepping through the source code, it is no longer required to set up the SymbolSource.org symbol source. The only thing a developer has to do is the enable the source server support checkbox as shown in the image below.

[GitLink settings]: /public/images/gitlink-settings.png