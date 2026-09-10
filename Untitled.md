CS PROCESS/MODEL ANSWER QUESTIONS:

Photo to binary 6 mark:
img divided into grid of pix
each pix sampled to match nearest available colour
each colour assigned unique colour code
colour depth is no. bits per pixel, number of colour available to pix is 2^bd
The binary codes for the pixs are stored as a single bit stream in raster order, meaning row by row, left to right, top to bottom.
A file header stores the resolution (width and height) and colour depth, which lets the software split the stream back into pixels and rows to rebuild the image correctly.

Why bitmap gets pixelated 3 marks:
no add pix when expanding
pix duplicate/stretch to fill space
individual pixels grow larger + more noticeable

How vector encoded + stored 3 marks:
stored as mathematical expressions
each drawing object recorded with type
properties of each object stored along with it
held in drawing list, image redrawn from exact instructions

why vector no lose quality 3:
stored as mathematical formulas, not individual pixs
dimensions recalced when scaled
shapes redrawn at new size, no duplicate/stretch

why vector bad for images:
continuous variation in colour + tone
no clear defined geometric shape
every small area need own object, large drawing list

Microphone work:
sound waves are vibrations in air particles
vibrations hit diaphragm in mic, cause same freq vibration
diaphragm attached to coil position in permanent magnet field
vibrate cause coil move back and forth in mf, generate varying current in coil, creating electrical signal
electrical signal same freq, same amplitude
