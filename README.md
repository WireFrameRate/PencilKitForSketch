# PencilKit Design Library
Design library that provides Apple PencilKit UI resources.  Supports Sketch, Figma, and InVision Studio.

**Current Version: 5.0**


## Introduction
The primary component of the PencilKit UI is the Toolpicker that appears at the botton of the canvas (by default). The ToolPicker can also be dragged, in which it transitions to a circle containing the currently-selected tool, or minimized to a slightly smaller circle. Dragging allows the Toolpicker to be docked onto the side of the screen in a vertical position.

This library contains four primary symbols: Horizontal Toolpicker, vertical Toolpicker, minimized Toolpicker, and and in-motion Toolpicker. Each is implemented in light- and dark-mode. All other symbols in this library are overrides for the Toolpicker.

Areas of the Toolpicker are:
* Control Buttons: Undo, Redo, and More. Library provides enabled and disabled states for light- and dark-mode.
* Tools: Pen, Marker, Pencil, Eraser, Selection, and Ruler. Library provides selected and deselected states for light- and dark-mode. Drawing tools also provide a text override for opacity.
* Color Palette: Six buttons with overrides for color and selected state. The buttons are universal (light- and dark-mode use the same symbol).

### What's new in version 5.0
iPadOS 14 added a new tool - the Text tool - to the toolpicker.  PencilKit Design Library has been updated to include the new tool.  In iPadOS, when you select the Text tool, the color palette is also replaced with a new set of tools.  The pallet has been made a nested, overridable symbol so that your design prototypes can quickly be updated to reflect selection of the Text Tool.  Like the previous Toolpicker symbols, the new iPadOS14 toolpickers shouldl be scaled depending on screen size.  See the table below for details.

![Light mode horizontal Toolpicker in iPadOS 14](https://github.com/WireFrameRate/PencilKitForSketch/raw/master/img/toolpicker-horizontal-light-ios14.png "Light mode horizontal Toolpicker in iPadOS 14")

![Dark mode horizontal Toolpicker in iPadOS 14](https://github.com/WireFrameRate/PencilKitForSketch/raw/master/img/toolpicker-horizontal-dark-ios14.png "Dark mode horizontal Toolpicker in iPadOS 14")

One of the buttons in the new Text Pallet is Font Format, which opens a new popup.  Like the previous popups, this should NOT be scaled for different screen sizes.

![Light mode Font Format Popup in iPadOS 14](https://github.com/WireFrameRate/PencilKitForSketch/raw/master/img/light-font-popup.png "Light mode Font Format Popup in iPadOS 14")

![Dark mode Font Format Popus in iPadOS 14](https://github.com/WireFrameRate/PencilKitForSketch/raw/master/img/dark-font-popup.png "Dark mode Font Format Popup in iPadOS 14")

While it's not new in iPadOS 14, we have added a new symbol to the library: The navigation bar Apple's Notes app.  It is available in Light and Dark modes.  Please note, it should NOT be scaled for the different screen sizes.  Simply adjust the width to fit the screen.

![Light mode Drawing Navbar in iPadOS 14](https://github.com/WireFrameRate/PencilKitForSketch/raw/master/img/light-navbar.png "Light mode horizontal Toolpicker in iPadOS 14")

![Dark mode Drawing Navbar in iPadOS 14](https://github.com/WireFrameRate/PencilKitForSketch/raw/master/img/dark-navbar.png "Dark mode horizontal Toolpicker in iPadOS 14")

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
### Sketch:
The library can be downloaded and installed locally, or installed as a remote library. If you download and install locally, you will have to manually check for and install updated. If you install as a remote library, you will recieve automatic updates when new library versions are published to GitHub.

[Click here to download](https://github.com/WireFrameRate/PencilKitForSketch/raw/master/PencilKit.sketch)

Copy and paste the following into your browser address bar to install the remote library:

```
sketch://add-library?url=https%3A%2F%2Fgithub.com%2FWireFrameRate%2FPencilKitForSketch%2Fraw%2Fmaster%2FPencilKit.rss
```

### InVision Studio:
To install in Studio, download [PencilKit.studio](https://github.com/WireFrameRate/PencilKitForSketch/raw/master/PencilKit.studio).  From a Studio project, click the '+' button next to Libraries.  Locate and select PencilKit.studio to install.

## Future Updates
* Color selector popup will be added.
* "More" popup window will be added.
* Tool popups
* Ruler on canvas.



