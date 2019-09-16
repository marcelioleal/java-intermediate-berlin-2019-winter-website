# 07 - OOP Exercises & Overloading

<Teacher name="Marcelio"></Teacher>

## Goals

- Preject Questions
- Questions? Let's address doubts on previous exercise(s)!
- Introduction to Inheritance
- Overloading and Overriding 
- Access modifiers
- Exercises

## OOP Slides

<GoogleSlides src="https://docs.google.com/presentation/d/1t7k0-o_S9Z-Rqg33MBOeYQe_lf5QDAunnfyrPPhWJe0/embed?start=false&loop=false&delayms=3000"></GoogleSlides>

https://docs.google.com/presentation/d/1t7k0-o_S9Z-Rqg33MBOeYQe_lf5QDAunnfyrPPhWJe0/edit#slide=id.g600867f478_0_91


## Review Exercises 
 
### Exercise 1
- Create a new constructor in Robot Class with String name, String eyesColor, int weight as parameters
- Create a new Class called YellowRobot that:
- is a subclass of Robot (extends Robot)
- Have the color equals to Yellow
- Have a new behaviour/method that sums 2 Integers returning an Integer
- Use this class in main, calls introduce, calls sum method and print the result

### Exercise 2
- Let's create another subclass of Robot called BlueRobot
- The BlueRobots must be always Blue
- Have a new behaviour/method that multiply 2 Integers returning an Integer
- We need to change the accessibility of the color property, it must be only changed inside the super class.
- Create a method in Robot called changeColor, to enable to change color in the sub classes. (change the constructor in subclasses)
- Now the method introduce for BlueRobots should return the following output:
"Hey, I am a BlueRobot! I know how to multiply integers." +
"Hello! My name is (name), I am (color), I have (eyes color) and I weight (weight) kilograms"
- Use this class in main, calls introduce, calls multiply method and print the result

### Exercise 3 - Overriding, multilevel inheritance
- Let's create another class called PurpleRobot, but now, the superclass is BlueRobot
- The PurpleRobots must be always Purple
- Have a new behaviour/method that calculate a number raise to the power of 2. (Give the name Pow) - Integer as parameter and return.
- Try to reuse the method multiply from BlueRobot.
- Now the method introduce for PurpleRobots should return the following output:
"Hey, I am a PurpleRobot! My parent class is BlueRobot."
"Hello! My name is (name), I am (color), I have (eyes color) and I weight (weight) kilograms"
- Use this class in main, calls introduce, calls pow method and print the result


### Exercise 3 - Polymorphism
- Now it's time to create a method calculate in all Robots
- This method must run the specific ability that the robots do. Like Yellow Robot sum, Blue multiply, etc.
- In the case of Purple Robot, we must create a new method pow, with two Integer parameters, and call Math.pow
- the return of the calculate method must be an Integer. Cast the result from Math.pow. Add (int) before the method call.
- Now it's time to create a new class - RobotHelper - this class has two properties Integer a and b
- You cannot change the properties out of this class
- This class helps the Robots to calculate,
it has a method that get any Robot as parameter (Robot, BlueRobot, YellowRobot, PurpleRobot)
and return the result of calculate from them using the properties.
- Use this class in main, print the result passing each Robot you have created
// Integer result = helper.calculateOperation(newYellow);
// System.out.println("The Result is: " + result); 


## Homework

### Homework 1

- Create more two Robots, one that know how to subtract and another one the divides two integers.
- Try them using the RobotHelper 

### Homework 2

- There are three different types of robots: robots that can fly, robot that can run and robot that can swim. Each one of them can only do one activity: running, swimming or flying. Extend your Robot class to support them and make sure that they have a method to fly, run or swim a given distance. How can you approach the problem? Should all robots have a fly(int distance) method?


## Additional Resources

http://www.ntu.edu.sg/home/ehchua/programming/java/J3f_OOPExercises.html#zz-1.1
https://docs.oracle.com/javase/tutorial/java/IandI/subclasses.html
https://javaconceptoftheday.com/java-inheritance-practice-coding-questions/
