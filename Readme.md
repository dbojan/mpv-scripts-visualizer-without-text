## Various mpv lua scripts

- visualizer.lua - various audio visualization.

- firequalizer.lua - linear phase 15-bands equalizer.

## Key bindings

use c key to flip through

## Screenshoots

### visualizer.lua

removed two lines:  
"axisfile       = data\\\\:'" .. axis_0 .. "':" ..  
"axisfile       = data\\\\:'" .. axis_1 .. "':" ..

changed font color:  
"fontcolor      = 'st(0, (midi(f)-53.5)/12); st(1, 0.5 - 0.5 * cos(PI*ld(0))); r(1-ld(1)) + b(ld(1))':" ..  
to  
"fontcolor      = 'a(0)':" ..

### firequalizer15.lua

![firequalizer15](screenshoots/firequalizer15.jpg)

## Related projects

- [HTML5 ShowCQTBar](https://github.com/mfcc64/html5-showcqtbar) - showcqt/showcqtbar visualizer on an HTML5 page.
- [YouTube Musical Spectrum](https://github.com/mfcc64/youtube-musical-spectrum) - showcqt visualizer as a Chrome extension.
