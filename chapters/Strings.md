# Strings
(Note, this section contains text and code from the Processing String Tutorial available here: https://processing.org/tutorials/text/)

[Part 1: Introduction](#part-1-introduction)

[Part 2: Activities, Code, & Intstruction](#part-2-activities-code-instruction)

Part 3 Formative Assessment

## Part 1 Introduction


### What is a String?


## Part 2 Activities Code Instruction

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
Learning Objectives
After completion of this lab, students should be able to
* Create and display a string object using formatted text

Previous knowlege required:
* Basic drawing in Processing, including color representation

Copy the code above and paste into Processing. Run the code and you should see output that looks like the following:
![The String "Hello Strings" in black arial font on a white background](https://github.com/treinartz/APCS.ProcessingResources/blob/gh-pages/chapters/HelloString.png)

Modify the code to change
(1) The font used 
(2) The font size
(3) The background color
(4) The font color
Here is an example of a completed lab (note yours will look different depending on the font and colors you chose)
![The String "Hello Strings" in purple parchment font on a light blue background](https://github.com/treinartz/APCS.ProcessingResources/blob/gh-pages/chapters/HelloString2.png)


## Section B: Manipulating Strings
It appears from the above that a String is nothing more than a list of characters in between quotes. Nevertheless, this is only the data of a String. We must remember that a String is an object with methods (which you can find on the reference page.) This is just like how we learned in the Pixels tutorial that a PImage stores both the data associated with an image as well as the functionality: copy(), loadPixels(), etc.

For example, the method charAt() returns the individual character in the String at a given index. Note that Strings are just like arrays in that the first character is index #0!

String message = "some text here.";
char c = message.charAt(3);
println(c);                // Results in 'e'
Another useful method is length(). This is easy to confuse with the length property of an array. However, when we ask for the length of a String object, we must use the parentheses since we are calling a function called length() rather than accessing a property called length.
String message = "This String is 34 characters long.";
println(message.length());

We can also change a String to all uppercase using the toUpperCase() method (toLowerCase() is also available).

String uppercase = message.toUpperCase();
println(uppercase); 
You might notice something a bit odd here. Why didn't we simply say "message.toUpperCase()" and then print "message" variable? Instead, we assigned the result of "message.toUpperCase()" to a new variable with a different name—"uppercase".

This is because a String is a special kind of object. It is immutable. An immutable object is one whose data can never be changed. Once we create a String, it stays the same for life. Anytime we want to change the String, we have to create a new one. So in the case of converting to uppercase, the method toUpperCase() returns a copy of the String object with all caps.

Finally, let's look at equals(). Now, Strings can be compared with the "==" operator as follows:

String one = "hello";
String two = "hello";
println(one == two);

However, technically speaking, when "==" is used with objects, it compares the memory addresses for each object. Even though they contain the same data—"hello"-- if they are different object instances "==" could result in a false comparison. The equals() function ensures that we are checking to see if two String objects contain the exact same sequence of characters, regardless of where that data is stored in the computer's memory.

String one = "hello";
String two = "hello";
println(one.equals(two));
Although both of the above methods return the correct result, it's safer to use equals(). Depending on how String objects are created in a sketch, "==" will not always work.

One other feature of String objects is concatenation, joining two Strings together. Strings are joined with the "+" operator. Plus, of course, usually means add in the case of numbers. When used with Strings, it means join.

String helloworld = "Hello" + "World";
Variables can also be brought into a String using concatenation.

int x = 10;
String message = "The value of x is: " + x;

## Section C: String Input
