# PencilKitForSketch
Sketch library that provides Apple PencilKit UI resources.

## Introduction
The primary component of the PencilKit UI is the Toolpicker that appears at the botton of the canvas (by default). The ToolPicker can also be dragged, in which it transitions to a circle containing the currently-selected tool, or minimized to a slightly smaller circle. Dragging allows the Toolpicker to be docked onto the side of the screen in a vertical position.

This library contains four primary symbols: Horizontal Toolpicker, vertical Toolpicker, minimized Toolpicker, and and in-motion Toolpicker. Each is implemented in light- and dark-mode. All other symbols in this library are overrides for the Toolpicker.

Areas of the Toolpicker are:
* Control Buttons: Undo, Redo, and More. Library provides enabled and disabled states for light- and dark-mode.
* Tools: Pen, Marker, Pencil, Eraser, Selection, and Ruler. Library provides selected and deselected states for light- and dark-mode.
* Color Palette: Six buttons with overrides for color and selected state. The buttons themselves are universal (light- and dark-mode use the same symbol), however the selected state symbol has separate symbols for light- and dark-mode.


## Usage in Prototypes
In iPadOS, there is always one tool selected in the toolpicker by default. It is only possible to select one tool at a time. If a drawing tool is selected (pen, marker, pencil), then the corresponding color should be selected.

If your prototype includes a marked-up canvas, the Undo button override should be set to the enabled symbol. The More button should typically always be enabled.

![Light mode horizontal Toolpicker](https://github.com/WireFrameRate/PencilKitForSketch/raw/master/img/toolpicker_light_horizontal.png "Light mode horizontal Toolpicker")

![Dark mode horizontal Toolpicker](https://github.com/WireFrameRate/PencilKitForSketch/raw/master/img/toolpicker_dark_horizontal.png "Dark mode horizontal Toolpicker")

For the in-motion and minimized states, the tool should match the selected tool in the maximized Toolpicker. The mimimized and in-motion symmbols should alway use the "Selected" tool symbols.

![Light mode dragging Toolpicker](https://github.com/WireFrameRate/PencilKitForSketch/raw/master/img/toolpicker_light_inmotion.png "Light mode dragging Toolpicker") ![Dark mode dragging Toolpicker](https://github.com/WireFrameRate/PencilKitForSketch/raw/master/img/toolpicker_dark_inmotion.png "Dark mode dragging Toolpicker")

![Light mode minimized Toolpicker](https://github.com/WireFrameRate/PencilKitForSketch/raw/master/img/toolpicker_light_minimized.png "Light mode minimized Toolpicker") ![Dark mode minimized Toolpicker](https://github.com/WireFrameRate/PencilKitForSketch/raw/master/img/toolpicker_dark_minimized.png "Dark mode minimized Toolpicker")


## Installation Options




