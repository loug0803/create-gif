# GIF creator
This project is a simple Python program that creates an animated GIF from multiple PNG images using the imageio library.

## How it works

The program:

1. Stores the names of the PNG images in a list.
2. Reads each image using imageio.
3. Adds the images to a list.
4. Creates a GIF from all the images.
5. Sets the duration of each frame to 500 ms and makes the GIF loop continuously.

The main code uses:

import imageio.v3 as iio
file_names = ["chiclet1.png", "chiclet2.png", "chiclet3.png", "chiclet4.png"]
images = []
for file_name in file_names:
    images.append(iio.imread(file_name))
iio.imwrite("chiclet.gif", images, duration=500, loop=0)

## Project files

The repository contains:

* create_GIF.py — the Python script used to create the GIFs.
* 9 PNG images — used as frames for the different GIF tests.
* 3 GIF files — created using 2, 3, and 4 images respectively.

I tested the program several times to see how the animation changes depending on the number of frames.

Technologies

* Python
* imageio
* Git & GitHub