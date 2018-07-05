# Introduction and Conditional Logic

[Part 1: Introduction](#part-1-introduction)

[Part 2: Activities Code and Instruction](#part-2-activities-and-instruction)
* Activity #1: [Sandwich making and algorithms](https://github.com/treinartz/APCS.ProcessingResources/blob/gh-pages/chapters/IntroAndConditionalLogic.md#activity-1-make-a-peanut-butter-and-jelly-sandwich-activity)
* Activity #2: [Introduction to Processing](https://github.com/treinartz/APCS.ProcessingResources/blob/gh-pages/chapters/IntroAndConditionalLogic.md#activity-2-basic-introduction-to-processing)
* Activity #3: DVD Screensaver Code-along and Project
* Activity #4: FizzBuzz App

[Part 3: Formative Assessment](#part-3-formative-assessment)
* Around the World Activity
* 10 Question Quiz

---

## Part 1 Introduction

This unit is designed to be a student's first introduction to programming.  


## Part 2 Activities and Instruction

### Activity #1: Make a peanut butter and jelly sandwich activity

Activity modality: Unplugged

Goals: 
* Write an algorithm
* Compare human language to languages computers understand
* Pull out vocabulary
  * Parameter
  * Function
  


### Activity #2: Basic introduction to Processing. 

**Activity modality:** Modeling programming and Student-driven project

**Goals:** 
* Learn how writing code works - sequencing and basic syntax
* Read and interpret documentation
* Gain familiarity with the “setup” and the “draw” functions
* Pull out vocabulary
  * Syntax
  * Return
  * RGB Colors

**Activity Description**
Ask students to create a picture of some type on graph paper. There are many ways to do this - some suggestions are:
* Use pattern blocks or tanagrams to create a picture
* Use colored pencils to draw a picture of what they did this summer.
* Show some images of some modern art and have students create their own.

Once students have an image on their graph paper, have them transfer it to a processing sketch.

It is recommended that the teacher do this task too initially to model how students will start.  The teacher should have three things in front of them. 1) Their drawing, 2) The Processing IDE, and 3) The Processing Reference.

Give students a tour of what a typical sketch contains including how the setup() and draw() functions work.  At this point, it is ok to describe to students that any code written in the setup function runs once (when the program is run) and that the draw function runs repeatedly. 

********************* note for team: should this code be in the draw or setup function?

Initially, have students change the size of the sketch.  Students can do this by using the size() function.  They will need to put in two *parameters* into the size function to descsribe the length and width.  

At this point, students will see various sized gray display windows on their screens.  A natural tendancy of students will be to want to change the color of the background.  To do this, the teacher can model how to use the Processing reference.  It is to be expected that some students might be overwhlemed by all of the commands in the reference.  It may be a good idea to focus students' attention on the **2D Primitives** and **Setting** categories.

Have students click on background() under **Setting**.  Provide students with 1-2 minutes to explore the page themselves.  Ask students *"What do you notice?  What do you wonder?"*.  After students explore, gather their responses as a class.  Point out key portions of the reference.  Make sure to point out the following:
* Examples are very useful.  We might not understand them right away, but they help us see what is possible.
* It is not necessary to understand every word in the "description" in the reference.  Many times you can pullout what you need and ignore the rest.  Sometimes you need to do some further research.
* Under "Syntax" they show you different ways to use the function.  There are many ways it can be used, but the computer is expecting to see this syntax when it sees the word "background".  The recommendation today is to use background(v1, v2, v3)
* The parameters have data types associated with them.  Again, the computer is expecting a specific type of data when you use this mehtod.  If you don't use the right type of data, the computer may have trouble understanding your code.

This is the time to point out how RGB colors work.  Since the default mode in Processing is to use RGB colorMode, students maybe confused as to what v1, v2, and v3 are supposed to represent.  Describe how mixing paint is different than mixing light.  When we mix paint, we use red, yellow, and blue but when we mix light we use red, green, and blue (or RGB).  A quick google search of additive vs. subtractive color mixing can get more into the science behind this, but that is beyond the scope of the lesson as designed. 

![alt text][lightMixing]

[lightMixing]: https://upload.wikimedia.org/wikipedia/commons/c/c2/AdditiveColor.svg

With this infromation, allow students to experiment with changing thier background color.  At some point, it may be useful to show students [Google's tool for choosing colors](https://www.google.com/search?rlz=1C1GGRV_enUS758US758&ei=sGs9W-KoDdWQ0PEPiPyr8A0&q=color+picker&oq=color+picker&gs_l=psy-ab.3..35i39k1l2j0i20i263k1j0i67k1j0l6.3493.3864.0.4104.2.2.0.0.0.0.93.181.2.2.0....0...1c.1.64.psy-ab..0.2.181...0i20i264k1.0.nbbg8nNpD1U). 

![alt text][colorPicker]

[colorPicker]: https://github.com/treinartz/APCS.ProcessingResources/blob/gh-pages/chapters/ColorPicker.PNG

The task for the rest of the time is for students to re-create their image in processing using the commands found in the reference language.  It is recommended that the teacher model an element of their own drawing to show students how to navigate the reference and how coordinates work on the display screens.

Using the provided handout, students can use the grid system to identify key points on their image.  

### Activity #3: DVD Screensaver Code-along and Project

**Activity modality:** Code-along

**Goals:** 
* Use conditional statements in a program
+ Animate shapes in 2 dimensions on a screen
+ Put images (and if time, sounds) into a sketch
+ Initiate variables and update variables

**Activity Description**
Students re-create the bouncing DVD logo in a sketch.  Students are guided through this with an instructor the process suggested is as follows:
+ Get image on the screen
+ Get the image to move in the x direction
+ Indentify why the movement isn't perfect... yet
+ Allow students to solve the movement problems AND add movement in the y direction
+ Encourage extensions, listed below

**Hook**
Show video from "The Office" (attached here or found at [this link](https://www.google.com/url?sa=t&rct=j&q=&esrc=s&source=web&cd=1&cad=rja&uact=8&ved=0ahUKEwiX2ZTjwffUAhUGdT4KHbtvANQQuAIIKTAA&url=http%3A%2F%2Fwww.godtube.com%2Fwatch%2F%3Fv%3DJJBJFCNU&usg=AFQjCNFn-kQjAoiL0w_j0CRY40owbPUagA))

Transition: 
*"Animation is exciting.  Today, we are going to use p5 to re-create the animation from The Office"*

**Get image on the screen**

**Get image to move in x direction**
+ Introduce variables by declaring a global variable dvdx
+ Encourage students to predict how you will use the variable to make the image move
+ Do a code along to show how you can make the image move in the x direction (make it clear that you are updating the dvdx variable to change the position)
+ Show that the loop re-draws the image leaving a "path" behind it, thus you need to clear the screen.

**Indentify why the movement isn't perfect... yet**
* Ask students *"What could we do to make this better?"*
  * Make the image bounce off the screen
  * Make the image so it bounced off both ends
  * Make the image so it bounces off the screen perfectly (not just off the screen)
  * Make the image move in the y direction too

+ Ask students to predict with a partner how they might get the image to bounce off the screen.
+ Gather student generated ideas and do a code-along to make the bounce happen.

* Ask students *"What could we do to make this better?"*
 * Make the image bounce off both ends
 * Make the image bounce off the screen perfectly (not just off the screen)
 * Make the image move in the y direction too

**Allow students to solve the movement problems AND add movement in the y direction**
+ Monitor students and bring the class back together to share solutions and troubleshoot problems

**Encourage extensions!** 
* Make it your own! 
  * Make it move at a different speeds
  * Make your own image/shape 
  * Make it start in a random direction/location each time it starts
  * Change the code so when it hits the corner something happens (colors change, sound happens?)
  * Add in interactivity (make it when it bounces, it changes color, or when you click the screen the background changes color…)
  * … other

## Part 3: Formative Assessment












## Part 4: Projects


* Activity #3 was co-developed with Brian Shott for p5 and and adjusted here
