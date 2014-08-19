---
layout: page
title: Plot controllers
---

// TODO //

### Default bindings

The default input bindings in the PlotController are:

|| Action || Gesture |
| Pan~* | Right mouse button |
| Zoom~* | Mouse wheel |
| Zoom by rectangle | Ctrl+Right mouse button |
| Reset~* | Right mouse button double-click |
| Show 'tracker' | Left mouse button |
| Reset axes | 'A' |
| Copy bitmap | Ctrl+C |
| Copy code | Ctrl+Alt+C |
| Copy properties | Ctrl+Alt+R |

You can zoom/pan/reset a single axis by positioning the mouse cursor over the axis before starting the zoom/pan.

### Customizing the bindings

Create a new PlotController:

``` csharp
var myController = new PlotController();
```

Set the controller in the Plot control

``` csharp
plot.Controller = myController;
```

Bind an input gesture to a command

``` csharp
myController.BindMouseDown(OxyMouseButton.Left, PlotCommands.Pan);
```

Unbind an input gesture
``` csharp
myController.UnbindMouseDown(OxyMouseButton.Right);
```

Unbind all commands

``` csharp
myController.UnbindAll();
```

- Creating new commands
- Creating new manipulators
