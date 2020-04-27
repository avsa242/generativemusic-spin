generativemusic-spin
--------------------

This is a P2X8C4M64P/Propeller 2 application that generates music algorithmically from short routines (generally "one-liners"), plays them using the P2's smart pin DAC mode, and _attempts_ to visualize the output on a 320x200x8bpp VGA-connected display. The output is inspired by viznut's Bytebeat video at https://www.youtube.com/watch?v=tCRPUv8V22o

## Salient Features

* Display sample as blue scope/waveform
* Display sample as red vertical pixel per sample (scrolled right to left)
* Display sample as green vertical pixel per sample (scrolled right to left)

## Requirements

* P2 rev B or newer silicon. 250MHz or greater clock is strongly recommended (default is 250MHz)

## Compiler Compatibility

* FastSpin (tested with 4.1.4)

## Limitations

* Doesn't do the original justice - the only visualization that's close to complete is the DrawWave() scope output, but this has a "rolling" effect due to no triggering
* DrawSampleRed() doesn't look right - you can tell there is a correlation with the original YouTube video, at times, but this needs work
* DrawSampleGreen() is farthest from completion - it draws _something_, but again isn't quite right
* Visualizations aren't drawn together

## TODO

- [ ] Add triggering to DrawWave()
- [ ] Fix DrawSampleRed()
- [ ] Fix DrawSampleGreen()
- [ ] Composite the three visualizations together and display as complete frame
- [ ] Add the ability to change some of the sample generation at runtime and display the updated routine?
