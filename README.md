# CAD Remap

## A tool to create CAD-helpful key and mouse behaviors.

I have an architectural background and have some ideas for key and mouse bindings that would be helpful for daily CAD work. 

The fork will be modified to provide the following behaviors (all currently in the planning/design phase, no implementation yet)

## Activation

The F Keys will be used as "toggles". Pressing a toggle activates the layer to listen to the applicable inputs. Pressing the toggle again disables the layer and stops listening to applicable inputs.

## Ortho Mode (F1)

Press F1 and activate *_Ortho Mode_*. This affects click-drag behavior. Drags with the mouse will sample the first delta and create an orthographic direction based on the first delta (up, down, left, or right). consequent mouse moves will be blocked and the delta extracted into a delta from the original point, effectively meaning the cursor will only move in straight line directions.

This will be implemented for all drag behaviors, Left, right and middle mouse buttons.

## Spin Scroll Mode (F2)

I use a trackball daily. I click-drag pan around drawings daily. Click-drag click-drag click-drag click-drag etc... grrrrr. 

Press F2 and enable _spin-scroll-mode_. now MMB becomes a toggle too.  MMB down activates spin-mode. spin the trackball and mouse moves will be delta compared to the original point and converted into a scrollwheel message, meaning that spinning the trackball scrolls instead of moving the cursor. 

Note that this mode will work in tandem with _Ortho Mode_.

## Infinite desktop pointer mode (F3)

Press F3 and activate _infinite pointer mode_. (Note: F3 disables F2). MMB becomes a toggle on this layer too. This time on holding down MMB, if the cursor leaves the boundary of the screen it will be reset to the bottom of the screen to create an infinite mouse gesture that never ends. 

This is especially helpful for a trackball, as the ball spin can move the mouse pointer much further than a mouse. 

Now when panning in a CAD program the mouse will not stop the pan when reaching the edge of the screen. 

Note that this mode disables _Spin-Scroll Mode_ but works in tandem with _Ortho Mode_


## Future

_More to come, stay tuned._
_2022-09-03_


Legal
======

The MIT License (MIT)

Copyright (c) 2022, NWoodsman

Permission is hereby granted, free of charge, to any person obtaining a copy
of this software and associated documentation files (the "Software"), to deal
in the Software without restriction, including without limitation the rights
to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
copies of the Software, and to permit persons to whom the Software is
furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in
all copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN
THE SOFTWARE.

_This project is a fork of Lakey._

**Lakey**

The MIT License (MIT)

Copyright (c) 2014, Adrian L Lange

Permission is hereby granted, free of charge, to any person obtaining a copy
of this software and associated documentation files (the "Software"), to deal
in the Software without restriction, including without limitation the rights
to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
copies of the Software, and to permit persons to whom the Software is
furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in
all copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN
THE SOFTWARE.
