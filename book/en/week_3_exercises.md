# Week 3 Exercises: Programming III

CONTENTS: Wrapper Classes and first OOP exercises

## Mandatory Exercises:

1. You must create a `Person.java` class with attributes `name`, `height`, and `weight`, and their corresponding getters and setters. In the main method, you must instantiate 3 objects of this class and complete their information by asking the user via console for each object. Finally, you must show who is the tallest and who weighs the most. You must always use the getters and setters to get and set the information in each object instance.

2. Improve exercise 1 so that there is a parameterless constructor that initializes the values of name, height, and weight to default values that you consider appropriate.

3. Improve exercise 1 so that the `Person` class offers a method that calculates the person's BMI using the current values of the object's attributes. You must consider the possibility that the values have not been initialized to valid values.

4. Analyze the execution flow of the program by placing breakpoints in the constructor and in the different parts of the code of exercise 1. Set values to the attributes directly in their declaration and set a breakpoint to check what is executed first: the constructor or the attribute declaration.

## Extension Exercises:

5. Using the `parseXXX` methods of the wrapper classes, build a class with appropriate methods to read all numeric data types (`int`, `float`, `double`) as strings. If the user does not enter a valid value, ask for the value again.

6. Modify exercise 1 so that the `Person.java` class is inside a package called `model` instead of the same package as the `App.java` class. What did you need to change to be able to use it in `App.java`?

7. What is the difference between the default constructor of a class in Java and a parameterless constructor?

8. Why use getters and setters and not access the attributes directly through the dot? Encapsulation. Is it a security or design issue?

9. What is the difference between defining an attribute as `public`, `private`, or no visibility modifier? In which case is it possible to access them through the dot (.) with an object reference?

10. What is the `this` keyword used for? And the `new` keyword?

11. It is possible to define classes that in turn have attributes of other classes (called Composition). You must now modify exercise 1 so that the `Person` class has an attribute of type `DNI` (another class that you will have to create) that will have as attributes number and letter. The constructor of the `Person` class must be passed a DNI number as a parameter and an object of type `DNI` will be created, generating the corresponding letter from the algorithm to obtain the DNI letter from the number.

12. Create a class called `Rectangle.java` with length and width attributes, each with a default value of 1. It must have methods to calculate the perimeter and area of the rectangle. It must have getter and setter methods for length and width. The setter methods must verify that length and width are floating-point numbers greater than 0.0, and less than 20.0. Write a program to test the `Rectangle` class.

13. Create a new project with the `Person.java` class that you initially created. Perform the following instructions and answer the questions.

```java
public static void main(String[] args) {
    // Creation of an object of the Person class
    Person paco = new Person("Paco", 22, 177.3f, 82.3f);
    
    // We copy the reference of the previous object to another reference
    Person refPaco2 = paco;
    
    // We use the second reference to set a value in the object it references
    refPaco2.setAgeYears(77);
    
    // Result?
    System.out.printf("The age of %s is:%d%n", paco.getName(), paco.getAgeYears());
    
    // What is the age shown?
    // How many objects are in memory? How many references? Check the Debugger
}
```
