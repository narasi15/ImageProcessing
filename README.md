# Image Processing
An application that places different filters and functions on any image. There are 2 functions(copy, scale) and 3 filters(greyscale, edge detection, gaussian blur). The sample image, dog.bmp, is what we will use to apply the filters and functions, and the new transformed image will be created in the images folder.

## Features
 * Copy: Creates an exact copy of the sample image.
 * Scale: Scales the image dimensions by a specified scale factor.

## Filters
 * greyscale: Creates a black and white image.
  > ![splashpage](dog.bmp) 
  > ![splashpage](/images/dog_grey.bmp)
 * edge detection: Finds the boundaries of objects within the image.
  > ![splashpage](dog.bmp)
  > ![splashpage](/images/dog_edge.bmp)
 * gaussian blur: Blurs the image by a Gaussian function. 
  >![splashpage](dog.bmp)
  >![splashpage](/images/dog_blur.bmp)

## How to use:
Download the repo in your local directory, and run the Makefile with following commands:
```make all
```
Make all will create the executables of each filter/function.
```make test
```
Make test will do the following 
mkdir -p images
	./copy < dog.bmp > images/dog_copy.bmp
	./greyscale < dog.bmp > images/dog_grey.bmp
	./scale 2 < dog.bmp > images/dog_scale.bmp
	./gaussian_blur < dog.bmp > images/dog_blur.bmp
	./edge_detection < dog.bmp > images/dog_edge.bmp
	./image_filter dog.bmp images/dog_piped.bmp

