## Visualizers for mpv

v 2026-04-07-1

It displays visualizers when there is no video played, without text in the middle.

### Installing:

copy lua files to mpv/scripts folder, or %appdata%/mpv/scripts, or .cache/mpv/scripts

- visualizer.lua - various audio visualization.

- firequalizer.lua - linear phase 15-bands equalizer (this is not graphic, it is automatically used)

### Key bindings

use c key to flip through

use standard f key to go to fullscreen in mpv.

### visualizer.lua, without text in the middle:

- removed two lines:  
"axisfile       = data\\\\:'" .. axis_0 .. "':" ..  
"axisfile       = data\\\\:'" .. axis_1 .. "':" ..

- changed font color, in both places:  
"fontcolor      = 'st(0, (midi(f)-53.5)/12); st(1, 0.5 - 0.5 * cos(PI*ld(0))); r(1-ld(1)) + b(ld(1))':" ..  
to  
"fontcolor      = 'a(0)':" ..
