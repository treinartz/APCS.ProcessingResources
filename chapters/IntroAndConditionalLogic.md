# Introduction and Conditional Logic

[Part 1: Introduction](#part-1-introduction)

[Part 2: Activities Code and Instruction](#part-2-activities-and-instruction)
* Activity #1: [Sandwich making and algorithms](https://github.com/treinartz/APCS.ProcessingResources/blob/gh-pages/chapters/IntroAndConditionalLogic.md#activity-1-make-a-peanut-butter-and-jelly-sandwich-activity)
* Activity #2: [Introduction to Processing](https://github.com/treinartz/APCS.ProcessingResources/blob/gh-pages/chapters/IntroAndConditionalLogic.md#activity-2-basic-introduction-to-processing)
* Acitivty #3: [DVD Screensaver Code-along and Project](https://github.com/treinartz/APCS.ProcessingResources/blob/gh-pages/chapters/IntroAndConditionalLogic.md#activity-3-dvd-screensaver-code-along-and-project)
* Activity #4: [ColorMixer](https://github.com/treinartz/APCS.ProcessingResources/blob/gh-pages/chapters/IntroAndConditionalLogic.md#activity-4-colormixer)


[Part 3: Formative Assessment](#part-3-formative-assessment)
* Using math operations
* Around the World Activity
* 10 Question Quiz

---

## Part 1 Introduction

This unit is designed to be a student's first introduction to programming.  This section includes 4 total activities, one unplugged activity, and 3 programming-based activities.  

In addition to these activities, there are three formative assessment activities.  For these formative assessments, students will need to know the following:
* Integer division
* Modular arithmetic
* Order of operations
* Conditionals and nested conditionals
* Variables assignment




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
  * Arguments
  * Functions
  * RGB Colors

**Resources:**
* Student Guide ( [PDF](https://github.com/treinartz/APCS.ProcessingResources/chapters/Student Guide_ Introduction-to-Processing-Handout-Activty2.pdf), [Google Doc](https://docs.google.com/document/d/17kb6P0IDRqhpzw-FXE69M4fWFeKF7DNggaVdpP6R1g0/edit?usp=sharing)
* Optional Videos about [Pixels](https://www.youtube.com/watch?v=a562vsSI2Po), [How to Use Setup and Draw](https://www.youtube.com/watch?v=o8dffrZ86gs), and [RGB Colors](https://www.youtube.com/watch?v=n2oHuKG_BQc&list=PLRqwX-V7Uu6Yo4VdQ4ZTtqRQ1AE4t_Ep9&index=2)

**Activity Description**

In this lesson, students will create an image on paper and then transfer it to processing.  This lesson calls for a mixture of instructor modeling as well as a student-driven project.  The general flow of the lesson includes the following:
* Students make an image on graph paper
* Students open up the Processing IDE and reference
* Instructor introduces the setup(), draw(), and size() functions
* Students change the size of their screen
* Instructor introduces the background() function and models reading the documentation with students.  Students learn the concept of RGB colors.
* Students change the background color
* Instructor may choose to model reading the documentation and using other functions to get forms on the screen.
* Students re-create their image in Processing.

<details><summary>Activity Details</summary>
<p>


**Students Create their Image**

Ask students to create a picture of some type on graph paper. There are many ways to do this - some suggestions are:
* Use pattern blocks or tanagrams to create a picture
* Use colored pencils to draw a picture of what they did this summer.
* Show some images of some modern art and have students create their own.

Once students have an image on their graph paper, have them transfer it to a processing sketch.

**Getting Into Processing**

It is recommended that the teacher do this task too initially to model how students will start.  The teacher should have three things in front of them. 1) Their drawing, 2) The Processing IDE, and 3) The Processing Reference.

Give students a tour of what a typical sketch contains including how the setup() and draw() functions work.  At this point, it is ok to describe to students that any code written in the setup function runs once (when the program is run) and that the draw function runs repeatedly. 

Initially, have students change the size of the sketch in the setup() function.  Students can do this by using the size() function.  They will need to put in two *arguments* into the size function to descsribe the length and width.  

**Modeling Reading the Documentation**

At this point, students will see various sized gray display windows on their screens.  A natural tendancy of students will be to want to change the color of the background.  To do this, the teacher can model how to use the Processing reference.  It is to be expected that some students might be overwhlemed by all of the commands in the reference.  It may be a good idea to focus students' attention on the **2D Primitives** and **Setting** categories.

Have students click on background() under **Setting**.  Provide students with 1-2 minutes to explore the page themselves.  Ask students *"What do you notice?  What do you wonder?"*.  After students explore, gather their responses as a class.  Point out key portions of the reference.  Make sure to point out the following:
* Examples are very useful.  We might not understand them right away, but they help us see what is possible.
* It is not necessary to understand every word in the "description" in the reference.  Many times you can pullout what you need and ignore the rest.  Sometimes you need to do some further research.
* Under "Syntax" they show you different ways to use the function.  There are many ways it can be used, but the computer is expecting to see this syntax when it sees the word "background".  The recommendation today is to use background(v1, v2, v3)
* The parameters have data types associated with them.  Again, the computer is expecting a specific type of data when you use this mehtod.  If you don't use the right type of data, the computer may have trouble understanding your code.

**Introducing RGB Colors**

This is the time to point out how RGB colors work.  Since the default mode in Processing is to use RGB colorMode, students maybe confused as to what v1, v2, and v3 are supposed to represent.  Describe how mixing paint is different than mixing light.  When we mix paint, we use red, yellow, and blue but when we mix light we use red, green, and blue (or RGB).  A quick google search of additive vs. subtractive color mixing can get more into the science behind this, but that is beyond the scope of the lesson as designed. 

![alt text][lightMixing]

[lightMixing]: https://upload.wikimedia.org/wikipedia/commons/c/c2/AdditiveColor.svg

With this infromation, allow students to experiment with changing thier background color.  At some point, it may be useful to show students [Google's tool for choosing colors](https://www.google.com/search?rlz=1C1GGRV_enUS758US758&ei=sGs9W-KoDdWQ0PEPiPyr8A0&q=color+picker&oq=color+picker&gs_l=psy-ab.3..35i39k1l2j0i20i263k1j0i67k1j0l6.3493.3864.0.4104.2.2.0.0.0.0.93.181.2.2.0....0...1c.1.64.psy-ab..0.2.181...0i20i264k1.0.nbbg8nNpD1U). 

![alt text][colorPicker]

[colorPicker]: https://github.com/treinartz/APCS.ProcessingResources/blob/gh-pages/chapters/ColorPicker.PNG

**Creating The Image**
The task for the rest of the time is for students to re-create their image in processing using the commands found in the reference language.  It is recommended that the teacher model an element of their own drawing to show students how to navigate the reference and how coordinates work on the display screens.

Using the provided handout, students can use the grid system to identify key points on their image.  



</p>
</details>


### Activity #3: DVD Screensaver Code-along and Project

**Activity modality:** Code-along
_Alternative modality:_ This may also work as a pair programming activity or a POGIL-type of activity.  A set of student facing directions can be found in [Google Doc](https://docs.google.com/document/d/1NAmKSAu1hne4R3ABDo6uf9MYptpzR7nx3umLUi1H6x0/edit?usp=sharing) form if you decide to have students work through this in partners rather than as a big class. 

**Goals:** 

* Use conditional statements in a program
+ Animate shapes in 2 dimensions on a screen
+ Put images (and if time, sounds) into a sketch
+ Initiate variables and update variables

**Resources**
* Student Guide 
* [Coding Train Videos](https://www.youtube.com/watch?v=wsI6N9hfW7E&list=PLRqwX-V7Uu6YqykuLs00261JCqnL_NNZ_) on Boolean Expressions (5.1 - 5.5) - optional


**Activity Description**

Students re-create the bouncing DVD logo in a sketch.  Students are guided through this with an instructor the process suggested is as follows:
+ Get image on the screen
+ Get the image to move in the x direction
+ Indentify why the movement isn't perfect... yet
+ Allow students to solve the movement problems AND add movement in the y direction
+ Encourage extensions

<details><summary>Activity Details</summary>
<p>

**Hook**
Show video from "The Office" (attached here or found at [this link](https://www.youtube.com/watch?v=QOtuX0jL85Y))

Transition: 
*"Animation is exciting.  Today, we are going to use Processing to re-create the animation from The Office"*

**Get image on the screen**

To do this, students need to add the DVD////////////////////////////////////////////////////////////////////////////////

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
 * During code-along, model frequent testing of code as well as mistake making.

**Allow students to solve the movement problems AND add movement in the y direction**
+ Monitor students and bring the class back together to share solutions and troubleshoot problems

**Encourage extensions!** 
* Possible extensions include: 
  * Make it move at a different speeds
  * Make your own image/shape 
  * Make it start in a random direction/location each time it starts
  * Change the code so when it hits the corner something happens (colors change, sound happens?)
  * Add in interactivity (make it when it bounces, it changes color, or when you click the screen the background changes color…)
  * … other



</p>
</details>

  
### Activity #4: ColorMixer 

**Activity modality:** Individual Lab

**Goals:** 
* Introduce MouseClicked() function
* Read and interpret documentation
* Read and comment code
* Use variables and nested conditionals

**Resources:**
* Student code


**Activity Description**
Students are provided some code and are asked to A) comment the exisiting code to make sense of it, and B) modify the exisiting code to function as desired.  

The code provided creates a user interfaces with 6 "buttons" for a user to add or take away red, green, and blue values from a color.  The resulting color swatch is shown on the screen.  Students need to add the functionality of the clicking on the appropriate buttons.  To do this, students will use conditional statements. 

![ColorMixer](https://media.giphy.com/media/1gSTyvtrXWZdltpdo8/giphy.gif)


## Part 3: Formative Assessment

### Math Operations Worksheet
10 Question worksheet ([google doc](https://docs.google.com/document/d/1ItyzrSFambR9eiSZUhoYZwsi1zq4GNAJ55N6r4wG3FI/edit?usp=sharing) || [pdf]())that covers the following:
* int and double data types
* Casting from doubles to ints
* Modular arithmetic
* Order of opreations

### Around the World Activity
The Around the World Activity is an opportunity for students to collaboratively read and trace code while also checking their answers as they go along.  In this document, each sheet of paper has a different problem on it as well as an answer that is NOT 

### 10 Question Quiz









* Activity #3 was co-developed with Brian Shott for p5 and and adjusted here
