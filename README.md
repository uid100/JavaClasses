# JavaClasses
 _(derived from CISC191M3BeginningClasses)_


Java Test Driven Development (TDD) project to review simple Java classes with unit testing ( with **JUnit** )

________

## Learning Outcome
- _preliminary_
________

![220px-MesaLogo](https://github.com/schougaard/SanDiegoMesaCISC191ProgrammingChallenges/assets/716243/334f6724-6afa-4198-9eff-7c49c472cd35)

# San Diego Mesa College CISC 191 Programming Challenges
Programming challenges for San Diego Community College CISC 191 Intermediate Java classes.

Created by
- Professor Dr. Tasha Frankie
- and Professor [Allan Schougaard](https://github.com/schougaard), San Diego Mesa College.

With contributions from: 
- Dom David,
- [Dan Sullivan](https://github.com/uid100)

________

## Learning Outcome
- _preliminary_
-------

## Assignment Overview
_Java_ classes are the building blocks of Java programs. They are used to define the data and behavior of objects. Classes are needed in Java because they provide a way to encapsulate data and behavior, which makes programs more modular, reusable, and maintainable.

Here are some of the specific reasons why Java classes are needed:

- To define the data and behavior of objects: A class defines the data that an object can hold, as well as the methods that an object can perform. This allows us to create objects that have specific properties and can perform specific actions.
- To improve modularity: Classes can be grouped into packages, which makes it easier to organize and manage code. This also makes it easier to reuse code, as we can simply import the classes that we need from a package.
- To improve reusability: Classes can be reused in multiple programs. This saves time and effort, as we don't have to rewrite the same code over and over again.
- To improve maintainability: Classes make it easier to maintain programs, as changes to a class can be made without affecting other parts of the program.

In short, Java classes are essential for writing well-organized, reusable, and maintainable Java programs.

________

## Instructions

## _(Open the Project)_
1. From the **<> Code** dropdown link in the repository (above), download the Zip file to your computer.
2. Extract the files to your working folder
3. Open Eclipse and import the project. 
   - You can use File>Import menu item or right-click in the Package Manager and choose Import.
   - select General>Projects from Folder or Archive
   - navigate into the project until you see the `bin` and `src` folders, and choose *open*
4. Expand the project in the package explorer and find the .java files below the **src** folder.

## _(Complete the Assignment)_
In this challenge you are going to write code to support a boat shop.

The shop needs to be able to store data about their boats, such a make, color, speed and price. Furthermore, the shop also needs to keep track of where their boats are stored.

### Boat
#### Part 1
##### First Tester Method
Let's try to get the first tester method to compile. The first thing you will notice is the missing getPrice method from the Boat class. When you use a method that does not exist you will get the message: The method <<method name>> is undefined for the type <<Class>>. Add this method to the Boat class.

```
public int getPrice() {
  // TODO Auto-generated method stub
  return -1;
}
```
Now the default return is currently -1, but if you look at the existing methods in the Boat class they are actually getters. Getters for a class help with retrieval of instance variables of that class so they usually pair with an instance variable. Let's add all the missing instance variables at the very top of the class and make sure to keep them private to follow a common java programming paradigm called encapsulation where you limit the access to instance variables of a class.

```
private String make; // a Boat has-a make
private Color color; // you should add the remaining comments for the instance variables
private int speed;
private int price;
```
Go back to the methods in Boat and correct them so that they are correct getter methods. You will notice that all of them will have a typical default value for their type with exception of the price which should return -1. You can fix this in a variety of ways, but add a default constructor that will set all the initial values of these variables rather than setting them directly at the top.

At this point, go ahead and also add the default constructor. The default constructor of a class is a no-parameter constructor. Remember that constructors help assign values to instance variables so you should have assignment statements as shown below.

```
public class Boat()//<-- no parameter constructor a.k.a. default constructor
{ 
  //the job of the constructor is to initialize the instance variable
  make = null;
  color = null;
  speed = ?; //what should be the initial speed?
  price = ?; //see the tester method for the default value for the price. Hint: It's not 0. 
}
```

___________
## Complete and zip the project
1. Run  and add the code to the source file
(`M2ArrayChallenge.java`) until the tests are successful.
2. Uncomment each test case in the **Test** file (`TestBeginningClasses.java`), one at a time. 
Do not modify the content in this file except to uncomment the tests. Add and modify class files
as needed for the tests to pass.
3. Review and refactor any of the code as needed:
    - be sure your code follows good coding practices and coding style and standards.
    - update the javadoc comments at the top of the file to add your name as author
    - update the comments for each method in the file.
4. Export the project as a zip file and submit your work.

___________

## Rubric

[Rubric](Rubric.md)


___________

_this repository is a subset of the CISC191 exercises. It is derived from the CISC191ProgrammingChallenges 
activity hosted by Professor Allan Schougaard, San Diego Mesa College, and not a direct fork._

_This project is to decompose that repository into git submodules_
