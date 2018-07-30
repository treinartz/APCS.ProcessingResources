# Advanced Object Oriented Programming (Advanced OOP)

[Part 1: Introduction](#part-1-introduction)

[Part 2: Activities Code and Instruction](#part-2-activities-code-and-instruction)

[Part 3: Formative Assessment](#part-3-formative-assessment)

[Part 4: Projects](#part-4-projects)

---

## Part 1 Introduction

To explore Advanced OOP requires understanding classes, objects, interfaces, inheritance, and concepts such as abstraction, encapsulation, and polymorphism.  Our experience has been that these topics are some of the more abstract and difficult.  To ground the concepts into something more concrete, we'll be using dogs as our theme.  We begin here with interfaces and polymorphism.  To prepare, complete the following before the activity implementation.

* First, click here [Advanced OOP](https://runestone.academy/runestone/static/JavaReview/index.html) to read about Interfaces and Inheritance that specifically addresses the AP Computer Science subset.
* Second, take a look at some Processing code for Interfaces here [Processing Interfaces](
https://processing.org/reference/implements.html) 
* Third, watch this video on polymorphism, a concept used for both Interfaces and Inheritance. 

<a href="http://www.youtube.com/watch?feature=player_embedded&v=e6eXD8DHc_A
" target="_blank"><img src="https://img.youtube.com/vi/qqYOYIVrso0/hqdefault.jpg" 
alt="IMAGE ALT TEXT HERE" width="240" height="180" border="10" /></a>

* Later, click here  [Processing Inheritance](
http://learningprocessing.com/examples/chp22/example-22-01-inheritance) to see some sample code in Processing
* Then, watch this video on Inheritance

<a href="http://www.youtube.com/watch?feature=player_embedded&v=e6eXD8DHc_A
" target="_blank"><img src="http://img.youtube.com/vi/e6eXD8DHc_A/0.jpg" 
alt="IMAGE ALT TEXT HERE" width="240" height="180" border="10" /></a>




## Part 2: Activities, Code and Instruction

### Interfaces
Activity #1:  Fundamental to these concepts is a thorough understanding of terms used when referring to object oriented programming.  Click here  [OOP Concepts](
https://docs.google.com/document/d/1u3BpoNlyrw3QzdOsm-rxMtCWDjyJW4Q1BfKRHbelO-c/edit?usp=sharing) for a sheet to get you started. 

Activity #2:  Getting started with interfaces.  In an IDE of choice or with paper, students write their own dog class that implements the Dog interface below.

```java
public interface Dog {
	public String getOwnerName();
	public String getDogName();
	public String getBark();
}
```
Here are more specific steps in the process:

		// name your class "yourNameDog"
		
		// need to implement interface Dog with 3 methods
		
		// instance data is all Strings ownersName, dogsName, and dogsBark
		
		// class has a constructor that takes an ownersname, dogname, and dogbark
		
		// toString() needs to return the instance data like this:
		
		// return ownerName + "'s dog "+dogName +" says "+ dogBark;
		
		//exchange your class with at least three others
		
		// write runner like this:
```java
		List<Dog> csKennel = new ArrayList<Dog>();
		csKennel.add(new JoansDog("Joanie", "2String()", "arf"));
		csKennel.add(new RogersDog("Roger", "Hershey", "GRRRRR!"));

	for (Dog d : csKennel) {
			System.out.println(d);
		}
```
                // make your dogs bark!

### Inheritance
In the following lab, students will create a class hierarchy composed of Dogs.  The term “dog” could also be a metaphor.  For example, in your school who is a “top dog?”  Who is a “lucky dog?”  Who is “sick as a” or “lucky as a” or “working like a” dog?  But we keep it simple below.

Design a Dog class with the following:  
• An instance variable for the name of the dog (a string)  
• An instance variable for the age of the dog (a string)  
• A constructor and appropriate accessors (getMethods()) and mutators (setMethods()) .   
• A toString method that displays the Dog's name and the Dog’s age.  

Then, design a BigDog class that extends the Dog class. The BigDog class should have the following 
members:
• A field (instance variable) for the dog’s weight (an int)
• A constructor and appropriate accessors and mutators.
• A toString method that overrides the toString method in the base class. The BigDog class's toString 
method should display only the Dog's name and the Dog’s weight.

Design a SmallDog class that extends the Dog class. The SmallDog class should have the following 
members:
• A field for the dog’s bark (a String)
• A constructor and appropriate accessors and mutators
• A toString method that overrides the toString method in the base class. The SmallDog class's toString 
method should display only the dog's name and the dog's bark sound.

Demonstrate the classes in a program (Runner) that has a Dog array. Assign various Dog, BigDog, and 
SmallDog objects to the array elements. The program should then step through the array, calling each 
object's toString method.

## Part 3: Formative Assessment
Assessment #1:  For the dog interface activity, you might collect all student dogs in one runner and demonstrate to class what all the dogs "say."  

Or, in an audio program like Audacity, have students create an audio file of how their dog sounds. Then in Processing, using those sound files, your abundant spare time, and this Processing code  [Sound files](
https://processing.org/reference/libraries/sound/SoundFile.html) to read through each file to hear the sounds.

Assessment #2:  Have students quiz each other and give examples before a brief quiz.












## Part 4: Projects
For Interfaces,  have students create a snowflake class in Processing that implements the Snow interface below. 
```java
public interface Snow{
 
  public void display();
  
  public void fall();
  	
  	public void fall(float speed);
  
  
}
```
The following are more specific guidelines for students:
To do this, you will have 3 tabs in your processing Sketch:
1. A tab with the interface (as shown below).  This interface should NEVER be edited by you.  The whole point of having an interface is that is common between everyone working on that project.
2. A tab with your snowflake code.  This should have at a minimum 1 constructor and 3 methods (specifically, the three methods outlined in the interface.  The first line of this code should be 

public class SnowflakeYourName implements Snow{

3. A tab with your runner class.  This should have a setup and draw method it should be what you use to make sure your Snowflake class is working as you expect.

Details for the Snowflake class you create:
Your class name can be named whatever you like, but please include your initials in the class name.  
Since your snowflake will extend the Snow class, you MUST have a display() method,  fall() method, and a fall(float speed) method.  
Things to keep in mind:
This will be combined with everyone else’s snowflakes so you might want to decide how yours will act once it reaches the bottom
Additionally, please have the following constructors:
a no-argument constructor which sets the starting x-position to a random number between 0 and the width of the screen
A parameterized constructor which allows the client to set the starting x-position of the snowflake




