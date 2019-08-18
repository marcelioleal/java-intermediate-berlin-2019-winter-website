# 01 - Introduction to Intermediate Java Course

<Teacher name="Michele"></Teacher>

## Goals

- Getting to know each other
- Get familiar with schedule, attendance, tools
- Course introduction
- Install required software
- Do some basic Java exercises (hopefully 🤩)


## Slides

<GoogleSlides src="https://docs.google.com/presentation/d/1pYFYnzWbZIh74X8k15qF4ij01lKnsZJfGyYI5V0ZpDs/edit#slide=id.gcb9a0b074_1_140/embed?start=false&loop=false&delayms=3000"></GoogleSlides>

## Java Basics Recap

```java
package com.redi.j2;

public class Main {

    public static void main(String[] args) {
        System.out.println("Hello World");

        String name = "Memet";
        String profession = "skydiver";
        int age = 40;
        boolean smoking = false;

        someMethod(profession);

        for (int i = 0; i < 10; i++) {
            System.out.println("hey " + i);
        }
    }

    private static void someMethod(String profession) {
        if (profession.equals("skydiver")) {
            System.out.println("Cool");
        } else {
            System.out.println("Not cool");
        }
    }
}
```

## Exercises

Same exercises as on the slides, copied here for convenience.

### Exercise 1

Write the method _squares_ that for X and Y given by arguments prints the square of each number between X and Y.

```square(1,3)
> 1 - 1
> 2 - 4
> 3 - 9

square(5,6)
> 5 - 25
> 6 - 36
```

### Exercise 2

In german, nouns ending with e are almost always feminine. Write a method _isFeminineNoun_ that checks if the provided word ends with e or not.


```isFeminineNoun("Katze")
> true

isFeminineNoun("Hund")
> false
```

Bonus: can you also make sure the method also catches words ending in _-ung_? Those are also feminine.

### Exercise 3

Let’s assume a freelancer has to pay insurance and income tax. Let’s assume insurance is fixed at 300€, while income tax is 9% for incomes of less than 1000€ (after insurance payment), and 21% otherwise.

``` inPocket(5000)
> 3713

inPocket
> 637
```


## Homework

Write a program that for given value of variable ‘height’ will print out the right-half of a pine tree to the console.

- The tree starts with “I” on the top and ends with “M” on the bottom. 
- The tree is built from “X” and “Y” characters one after another

For example, for an `height` of 6 it will print:

```
I
XY
XYX
XYXY
XYXYX
M
```

## Additional Resources

- The Java Tutorials (from Oracle) - https://docs.oracle.com/javase/tutorial/
- [W3Schools Java Tutorial](https://www.w3schools.com/java/)
- O'Reilly Programming Podcasts - https://www.oreilly.com/topics/oreilly-programming-podcast
