# Disney Afternoon Collection Overlays

The overlays you see here are the result of about a year of searching for tools to extract the game files. Finally found the tool on an obscure gaming forum. 

Now after ripping the borders and making the cfg files, of course they had to be further modified to work with Retroarch. The full screen ones didn't need much other that a stretch of the side art. The integer ones however...

*OH BOY*

The integer overlays are fine as they are, just had to remove the inner black square. But for some reason, the viewport fits no  true integer scale known to man. Too small for 3x vertical, too big for 2x vertical. Same with horizontal; 4x too big, 3x too small. In the end, I ended up with a 2.614x vertical and a 3.31x horizontal. This is obviously not an integer scale, so using a smoothing shader is *highly* recommended. I prefer the [sharp-bilinear shader](https://github.com/rsn8887/Sharp-Bilinear-Shaders) found here. This shader will smooth out the image enough to eliminate pixel wobble due to the combination of improper integer scale and uneven pixel rows.

## Video Settings

Full screen just requires using the default 4:3 setting in Retroarch, no integer scale needed.

Integer Scale uses the following settings:

* Custom X Pos: 237

* Custom Y Pos: 69

* Custom Width: 847

* Custom Height: 630

Preview

![preview](https://i.snag.gy/HbGyxu.jpg)
