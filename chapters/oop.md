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




```ruby
require 'redcarpet'
markdown = Redcarpet.new("Hello World!")
puts markdown.to_html
```






## Part 2: Activities, Code and Instruction

Activity #1:  Fundamental to these concepts is a thorough understanding of terms used when referring to object oriented programming.  Click here  [OOP Concepts](
https://docs.google.com/document/d/1u3BpoNlyrw3QzdOsm-rxMtCWDjyJW4Q1BfKRHbelO-c/edit?usp=sharing) for a sheet to get you started. 

Activity #2:  Getting started with interfaces.  In an IDE of choice or with paper, students write their own dog class that implements the Dog interface below.

```public interface Dog {
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
```
		List<Dog> csKennel = new ArrayList<Dog>();
		csKennel.add(new JoansDog("Joanie", "2String()", "arf"));
		csKennel.add(new RogersDog("Roger", "Hershey", "GRRRRR!"));

	for (Dog d : csKennel) {
			System.out.println(d);
		}
```
                // make your dogs bark!

## Part 3: Formative Assessment
Assessment #1:  For the dog interface activity, you might collect all student dogs in one runner and demonstrate to class what all the dogs "say."  

Or, in an audio program like Audacity, have students create an audio file of how their dog sounds. Then in Processing, using those sound files, your abundant spare time, and this Processing code  [Sound files](
https://processing.org/reference/libraries/sound/SoundFile.html) to read through each file to hear the sounds.

Assessment #2:  Have students quiz each other and give examples before a brief quiz.












## Part 4: Projects





