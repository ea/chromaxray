# Pseudocolor image augmentation utility. 

As I was doing X-Ray imaging of some electronics, I wanted to test the idea of adding false color to monochrome images to see if it would enhance visibility and readability. Turns out it's actually useful in some cases!

Opened images are _not uploaded_. All processing done _client-side_.

This simple tool takes an image, runs a heuristic on it's pixel values and applies a color map. Color map can be further manipulated by changing the sliders. _Shift_ moves the center of the color map which can help zero in on the features of interest._Quantize_ equalizes nearby color values which can be handy in some color maps. 
Using _Min_ and _Max_ sliders you can control the range of the color map that's applied. Play around with these and see if they lead to a better image. 

You can also change the color map itself. All of the ones in the drop down list come from [js-colormaps](https://github.com/timothygebhard/js-colormaps) library which in turn comes from Python's matplotlib. Default color map is [turbo](https://research.google/blog/turbo-an-improved-rainbow-colormap-for-visualization/) which was specifically designed with regards to human vision.

_Guess parameters_ is run by default when you open a new image, but can be used to reset all the sliders back if you go too far.
Finally, you can _Save_ the augmented image which should render it in the same resolution as the original and make it into a download.    

This whole thing started when a [neighbor](https://twitter.com/travisgoodspeed) lent me his X-Ray machine to have some fun. You can read more about that work [here](https://github.com/ea/film_xrays).

