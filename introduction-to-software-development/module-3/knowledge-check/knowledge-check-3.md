# Knowledge Check: Encapsulation and Abstraction – Enhancing Code Modularity

This document contains the answers and explanations for the knowledge check on "Encapsulation and Abstraction – Enhancing Code Modularity".

---

## 1. What key characteristics are exhibited by the abstract class Robot in the provided code?

abstract public class Robot {
    private int modeOfOperation;

    public int getModeOfOperation() {
        return modeOfOperation;
    }

    public void setModeOfOperation(int modeOfOperation) {
        if (modeOfOperation >= 1 && modeOfOperation <= 4) {
            this.modeOfOperation = modeOfOperation;
        } else {
            this.modeOfOperation = 1;
        }
    }
}


- Inheritance
- Method overloading
- **Encapsulation** ✅ (Correct)
- Interfaces

**Explanation:**  
That’s correct. The property `modeOfOperation` is made private, demonstrating encapsulation by restricting direct access and exposing it through a public method. Encapsulation is a key OOP principle that bundles data and methods and controls access to class members[1][6][7][8].

---

## 2. Consider the following code, where the Robot class extends the Machine class and implements the Jumping interface:

class Machine {
    int numberOfGears;
}
        
interface Jumping {
    public void jumpAround();
}

class Robot extends Machine implements Jumping {
    private void drive() {
        System.out.println("Robot is driving a car");
    }
}


Given this code, what must the Robot class do to ensure it correctly implements the Jumping interface and fully adheres to Java’s object-oriented principles?

- The Robot class must implement the Machine class.
- **The Robot class must implement the jumpAround() method.** ✅ (Correct)
- The Robot class can choose not to implement the jumpAround() method if it does not use it.
- The Robot class must make the method drive() public.

**Explanation:**  
That’s correct. By implementing the Jumping interface, the Robot class must provide an implementation for all interface methods. If it does not, the class must be declared abstract[2].

---

## 3. Consider the following code, which attempts to create an AmphibianAnimal class that inherits properties from both LandAnimal and WaterAnimal:

class LandAnimal {
    // code for LandAnimal class
}
        
class WaterAnimal {
    // code for WaterAnimal class     
}
        
class AmphibianAnimal extends LandAnimal, WaterAnimal {
    // code for AmphibianAnimal class   
    private int transferSpeedFromLandToWater;
}


Identify the issue with this code.

- The class AmphibianAnimal cannot have the property transferSpeedFromLandToWater as private.
- The class AmphibianAnimal must implement both classes.
- **The AmphibianAnimal class cannot extend from more than one parent class.** ✅ (Correct)
- WaterAnimal must extend the class LandAnimal before implementing AmphibianAnimal.

**Explanation:**  
That’s correct. Java does not support multiple inheritance for classes to avoid complexity and ambiguity (such as the diamond problem). A class can only extend one parent class[3].

---

## 4. Which properties of the Parent class can be directly accessed within the Child class? Consider the provided code and select all correct statements.

class Parent {
    private String privateField;
    protected String protectedField;
    public String publicString;
}

class Child extends Parent {
    // code of Child class
}


- The property publicField can be accessed directly only in Parent class.
- **The property privateField can be accessed directly in Parent class.** ✅ (Correct)
- **The property protectedField can be accessed directly in Child class.** ✅ (Correct)
- The property privateField can be accessed directly in Child class.

**Explanation:**  
Private fields are accessible only within their own class. Protected fields are accessible in subclasses (child classes), and public fields are accessible everywhere[4][5].

---

## 5. True or False: The following code will display “Hi humans” and “Bow wow!” because the dogObject is both an Animal and a Dog.

class Animal {
    public void sound() {
        System.out.println("Hi humans.");
    }
}

class Dog extends Animal {
    public void sound() {
        System.out.println("Bow wow!");
    }
}

public class QuizQuestions {
    public static void main(String[] args) {
        Dog dogObject = new Dog();
        dogObject.sound();
    }
}


- True
- **False** ✅ (Correct)

**Explanation:**  
That's correct. When a method is overridden in a child class, calling that method on an object of the child class executes only the child's version. It would display only "Bow wow!". To also execute the parent's method, you'd need to explicitly call it using `super.sound()` within the child's method[5].

---
