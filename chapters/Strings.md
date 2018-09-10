# Strings
(Note, this section contains text and code from the Processing String Tutorial available here: https://processing.org/tutorials/text/)

[Part 1: Introduction](#part-1-introduction)

[Part 2: Activities, Code, & Instruction](#part-2-activities-code-instruction)

Part 3 Formative Assessment

## Part 1 Introduction

[https://processing.org/reference/String.html](Processing string documentation)
[https://docs.oracle.com/javase/6/docs/api/java/lang/String.html] (Java string documentation)

[https://www.youtube.com/watch?v=NLzne4XaR3M ](Video: Introduction to Strings and Drawing Text)

[https://processing.org/tutorials/text/](Processing string tutorial)


## Part 2 Activities Code Instruction

Here are all of the steps needed to draw a string on the screen.

```
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

f = loadFont("ArialMT-16.vlw");
```

## LAB EXERCISE 1: Displaying Strings
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

## LAB EXERCISE 2: Parts of Strings

## LAB EXERCISE 3: Character input

## LAB EXERCISE 4: Processing Strings

## SUMMATIVE ASSESSMENT
After students have completed this series of labs, we suggest using the College Board MagPie lab. This chatbot-based lab will give the students more practice using Strings in the context of a larger problem. This lab and starter code is available through the College Board portal.

