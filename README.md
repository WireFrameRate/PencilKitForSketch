# PencilKit For Sketch
Sketch library that provides Apple PencilKit UI resources.

**Current Version: 3.0**


## Introduction
The primary component of the PencilKit UI is the Toolpicker that appears at the botton of the canvas (by default). The ToolPicker can also be dragged, in which it transitions to a circle containing the currently-selected tool, or minimized to a slightly smaller circle. Dragging allows the Toolpicker to be docked onto the side of the screen in a vertical position.

This library contains four primary symbols: Horizontal Toolpicker, vertical Toolpicker, minimized Toolpicker, and and in-motion Toolpicker. Each is implemented in light- and dark-mode. All other symbols in this library are overrides for the Toolpicker.

Areas of the Toolpicker are:
* Control Buttons: Undo, Redo, and More. Library provides enabled and disabled states for light- and dark-mode.
* Tools: Pen, Marker, Pencil, Eraser, Selection, and Ruler. Library provides selected and deselected states for light- and dark-mode. Drawing tools also provide a text override for opacity.
* Color Palette: Six buttons with overrides for color and selected state. The buttons are universal (light- and dark-mode use the same symbol).


## Usage in Prototypes
In iPadOS, there is always one tool selected in the toolpicker by default. It is only possible to select one tool at a time. If a drawing tool is selected (pen, marker, pencil), then the corresponding color should be selected.  In version 3.0 and later, the Pen, Marker, and Pencil tools have overrides that allow customization of tip color and size.

If your prototype includes a marked-up canvas, the Undo button override should be set to the enabled symbol. The More button should typically always be enabled.

![Light mode horizontal Toolpicker](https://github.com/WireFrameRate/PencilKitForSketch/raw/master/img/toolpicker_light_horizontal.png "Light mode horizontal Toolpicker")

![Dark mode horizontal Toolpicker](https://github.com/WireFrameRate/PencilKitForSketch/raw/master/img/toolpicker_dark_horizontal.png "Dark mode horizontal Toolpicker")

For the in-motion and minimized states, the tool should match the selected tool in the maximized Toolpicker. The mimimized and in-motion symmbols should alway use the "Selected" tool symbols.

![Light mode dragging Toolpicker](https://github.com/WireFrameRate/PencilKitForSketch/raw/master/img/toolpicker_light_inmotion.png "Light mode dragging Toolpicker") ![Dark mode dragging Toolpicker](https://github.com/WireFrameRate/PencilKitForSketch/raw/master/img/toolpicker_dark_inmotion.png "Dark mode dragging Toolpicker")

![Light mode minimized Toolpicker](https://github.com/WireFrameRate/PencilKitForSketch/raw/master/img/toolpicker_light_minimized.png "Light mode minimized Toolpicker") ![Dark mode minimized Toolpicker](https://github.com/WireFrameRate/PencilKitForSketch/raw/master/img/toolpicker_dark_minimized.png "Dark mode minimized Toolpicker")

Finally, for several tools there are popup menus to access more settings like tip size, opacity, etc. 

![Popups overview](https://github.com/WireFrameRate/PencilKitForSketch/raw/master/img/popup_menus.png "Popup Menus")

## Apple Pencil Gen2
Finally, the library provides a vector-based render of the generation 2 Apple Pencil.

![Apple Pencil Gen2](https://github.com/WireFrameRate/PencilKitForSketch/raw/master/img/pencil_gen2.png "Apple Pencil Gen2")


## Installation Options
The library can be downloaded and installed locally, or installed as a remote library. If you download and install locally, you will have to manually check for and install updated. If you install as a remote library, you will recieve automatic updates when new library versions are published to GitHub.

[Click here to download](https://github.com/WireFrameRate/PencilKitForSketch/raw/master/PencilKit.sketch)

Copy and paste the following into your browser address bar to install the remote library:

```
sketch://add-library?url=https%3A%2F%2Fgithub.com%2FWireFrameRate%2FPencilKitForSketch%2Fraw%2Fmaster%2FPencilKit.rss
```


## Future Updates
* Color selector popup will be added.
* "More" popup window will be added.
* Tool popups
* Ruler on canvas.



