# 2dArrays

[https://processing.org/tutorials/pixels/] (Processing tutorial on images and pixels)
This tutorial contains a lot of information, but walks through how to create an image and the two ways to loop through pixles. Here we are using images as a way to teach 2D arrays, so a suggested progression through the material would be:
(1) Learn basics of opening an image
(2) Modify all pixels (as a list) - review color in Processing and discuss other modifications
(3) Modify all pixels using nested loops (introduce 2D arrays)- it can be tricky to explain how the x and y values turn into a single value to access the pixel - you might need to spend some time going over this concept
(4) Modify selections of pixels using nested loops 

[https://www.youtube.com/watch?v=15aqFQQVBWU] Code.org video about pixels

## LAB #1: Modify all the pixels in an image

The code below modifies all of the pixels in an image. Load an image from your computer and see if you can figure out what changes when this code is run.

```
PImage img; // Declare the image object

void setup() {
  size(200,200);
  img = loadImage("dino.jpg");  // load the image in setup() - change the name to reflect your image
  // NOTE: Make sure your image is in the same folder as your code
}

void draw() {
  loadPixels();  // load all the pixels from your image into the pixels[] array
  for(int i=0; i<pixels.length; i++){  // loop through every pixel
    float r = red(img.pixels[i]);      // get the red, green, and blue values for each pixel
    float g = green(img.pixels[i]);
    float b = blue(img.pixels[i]);
    r = r * 0.5;
    pixels[i] =  color(r,g,b);     
  }
  updatePixels();  // redraw the picture with modified pixels
}
```

Now that you've seen how to modify all the pixels in a picture, try each of the following modifications on the same picture. 
1. Remove all the blue from each pixel
2. Modify each pixel to have the maximum amount of green
3. Make an image appear "through rose colored glasses" by modifying the r, g, b values to give the image a rosey color
4. Convert an image to grayscale by averaging the r, g, and b values for each pixel and using the new value for all three color components

## LAB #2: 

## LAB #3:

## SUMMATIVE ASSESSMENT: Instagram Filter


