# Strings
(Note, this section contains selections of the Processing String Tutorial available here: https://processing.org/tutorials/text/)

## Introduction to Creating and Drawing Strings
Any time we want to use text in our programs, or display text in our output, we are likely going to need Strings. We've seen Strings in our code before, and in this chapter we will start to understand how they work and how we can display and manipulate them in Processing.

Here are some examples of ways you may have used strings in your code:
println("printing some text to the message window!");  // Printing a String
PImage img = loadImage("filename.jpg");                // Using a String for a file name
Nevertheless, although you may have used a String here and there, it's time to unleash their full potential.

Where do we find documentation for the String class?
Although technically a Java class, because Strings are so commonly used, Processing includes documentation in its reference: http://www.processing.org/reference/String.html.

This page only covers some of the available methods of the String class. The full documentation can be found on java's String page.

### What is a String?
A String, at its core, is really just a fancy way of storing an array of characters. If we didn't have the String class, we'd probably have to write some code like this:

char[] sometext = {'H', 'e', 'l', 'l', 'o', ' ', 'W', 'o', 'r', 'l', 'd'};
Clearly, this would be a royal pain in the Processing behind. It's much simpler to do the following and make a String object:

String sometext = "How do I make String? Type some characters between quotation marks!";

### Displaying Text
The easiest way to display a String is to print it in the message window. This is likely something you've done while debugging. For example, if you needed to know the horizontal mouse location, you would write:

println(mouseX);
Or if you needed to determine that a certain part of the code was executed, you might print out a descriptive message.

println("We got here and we're printing out the mouse location!!!");
While this is valuable for debugging, it's not going to help our goal of displaying text for a user. To place text on screen, we have to follow a series of simple steps.

1. Declare an object of type PFont.

PFont f;
2. Create the font by referencing the font name and the function createFont().
This should be done only once, usually in setup(). Just as with loading an image, the process of loading a font into memory is slow and would seriously affect the sketch's performance if placed inside draw(). You can see a list of your available system fonts by via PFont.list(). Because of limitations in Java, not all fonts can be used and some might work with one operating system and not others. When sharing a sketch with other people or posting it on the web, you may need to include a .ttf or .otf version of your font in the data directory of the sketch because other people might not have the font installed on their computer. Only fonts that can legally be distributed should be included with a sketch. In addition to the name of the font, you can specify the size as well as whether the font should be antialiased or not.

f = createFont("Arial",16,true); // Arial, 16 point, anti-aliasing on

3. Specify the font using textFont().
textFont() takes one or two arguments, the font variable and the font size, which is optional. If you do not include the font size, the font will be displayed at the size originally loaded. When possible, the text() function will use a native font rather than the bitmapped version created behind the scenes with createFont() so you have the opportunity to scale the font dynamically. When using P2D, the actual native version of the font will be employed by the sketch, improving drawing quality and performance. With the P3D renderer, the bitmapped version will be used and therefore specifying a font size that is different from the font size loaded can result in pixelated text.

textFont(f,36);

4. Specify a color using fill().

fill(255);

5. Call the text() function to display text.
This function is just like shape or image drawing, it takes three arguments—the text to be displayed, and the x and y coordinate to display that text.

text("Hello Strings!",10,100);
Here are all the steps together:

PFont f;                           // STEP 1 Declare PFont variable
  
void setup() {
  size(200,200);
  f = createFont("Arial",16,true); // STEP 2 Create Font
}

void draw() {
  background(255);
  textFont(f,16);                  // STEP 3 Specify font to be used
  fill(0);                         // STEP 4 Specify font color 
  text("Hello Strings!",10,100);   // STEP 5 Display Text
}
Fonts can also be created using "Tools" → "Create Font." This will create and place a VLW font file in your data directory which you can load into a PFont object using loadFont().

f = loadFont("ArialMT-16.vlw");

## LAB EXERCISE 1
Copy the code above and paste into Processing. Run the code and you should see output that looks like the following:
![ALT-TEXT](APCS.ProcessingResources/chapters/HelloString.png)
