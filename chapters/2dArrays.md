# 2dArrays

[https://processing.org/tutorials/pixels/] (Processing tutorial on images and pixels)
This tutorial contains a lot of information, but walks through how to create an image and the two ways to loop through pixles. Here we are using images as a way to teach 2D arrays, so a suggested progression through the material would be:
(1) Learn basics of opening an image
(2) Modify all pixels (as a list) - review color in Processing and discuss other modifications
(3) Modify all pixels using nested loops (introduce 2D arrays)- it can be tricky to explain how the x and y values turn into a single value to access the pixel - you might need to spend some time going over this concept
(4) Modify selections of pixels using nested loops 

[https://www.youtube.com/watch?v=15aqFQQVBWU] Code.org video about pixels

## LAB #1: Modify all the pixels in an image
PImage img;

void setup() {
  size(200,200);
  img = loadImage("dino.jpg");
}

void draw() {
  //image(img,0,0);
  loadPixels();
  for(int i=0; i<pixels.length; i++){
    float r = red(img.pixels[i]);
    float g = green(img.pixels[i]);
    float b = blue(img.pixels[i]);
    r = r * 0.5;
    pixels[i] =  color(r,g,b);     
  }
  updatePixels();  
}

## LAB #2: 

## LAB #3:

## SUMMATIVE ASSESSMENT: Instagram Filter


