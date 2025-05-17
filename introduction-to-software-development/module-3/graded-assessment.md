# Module Quiz: Object-Oriented Programming Basics

This document contains answers and explanations for the module quiz on "Object-Oriented Programming Basics".

---

## 1. True or False: A class is represented by a real-world object like Toni, and an object is used as a blueprint for creating classes.

- **False** ✅ (Correct)

**Explanation:**  
An object like Toni is not the blueprint but rather the implementation of the blueprint. The blueprint is the class from which objects like Toni are created.

---

## 2. What is the output of the following code?

class Calculator {
    int calc(int number1, int number2) {
        return number1 + number2;
    }

    double calc(double number1, double number2) {
        return number1 * number2;
    }
}

public class ModuleQuiz_M3L3 {
    public static void main(String[] args) {
        Calculator calcObject = new Calculator();

        System.out.println(calcObject.calc(2, 1));
    }
}

If called with `calc(2, 1)`:

- Compile time error
- 5
- 2
- **3** ✅ (Correct)

**Explanation:**  
In method overloading, the method that gets called is determined by the arguments' types. Here, both arguments are integers, so `calc(int, int)` is invoked, returning 3.

---

## 3. Select the output of the following code:

class Student {
    int rollNo;
    int age;
    String name;
    String subject;

    public void payFees() {
        System.out.println("Paying full fees.");
    }
}

class Trainee extends Student {
    int stipend;

    public void payFees() {
        System.out.println("Paying fees with 30% discount.");
    }
}

public class ModuleQuiz_M3L3 {
    public static void main(String[] args) {
        Student traineeObject = new Trainee();
        traineeObject.payFees();
    }
}


- Paying full fees.
- **Paying fees with 30% discount.** ✅ (Correct)
- Compile time error. Cannot assign a Trainee class object to a Student class object.
- Paying no fees.

**Explanation:**  
A child class object can be assigned to a parent class reference. When a method is called, the method from the actual object's class (here, Trainee) is executed.

---

## 4. Select the output of the following code:

class Vehicle {
    String typeOfVehicle = "vehicle";

    void printType() {
        System.out.println("This is a " + typeOfVehicle);
    }
}

class Car extends Vehicle {
    String typeOfVehicle;

    @Override
    void printType() {
        super.printType();
        System.out.println("A car is a vehicle.");
    }
}

public class ModuleQuiz_M3L3 {
    public static void main(String[] args) {
        Car carObject = new Car();
        carObject.printType();
    }
}


- The output is “A car is a vehicle” only.
- The output is “This is a vehicle” only.
- **The output is both “This is a vehicle” and “A car is a vehicle”.** ✅ (Correct)
- The output is both “super” and “A car is a vehicle”.

**Explanation:**  
The Car class's `printType()` method first calls `super.printType()`, which prints "This is a vehicle", then prints "A car is a vehicle".

---

## 5. Select all that apply. Which of the following statements are true about access modifiers in Java inheritance?

- A private member of a superclass can be accessed in the subclass using the keyword super only.
- **A protected member of a superclass can be accessed directly by the subclass.** ✅ (Correct)
- **A private member of a superclass cannot be accessed directly by the subclass.** ✅ (Correct)
- **Access modifiers affect inheritance by determining which members of the superclass can be inherited by the subclass.** ✅ (Correct)

**Explanation:**  
Protected members are accessible in child classes. Private members are only accessible within their own class. Access modifiers control inheritance and accessibility.

---

## 6. In the following code, what should replace ------- to display “I am a duck”?

class Animal {
    void whatAmI() {
        System.out.println("I am an animal.");
    }
}

class Duck extends Animal {
    @Override
    void whatAmI() {
        System.out.println("I am a Duck");
    }
}

public class ModuleQuiz_M3L3 {
    public static void main(String []args) {
       Animal animalObject = -------;
       animalObject.whatAmI();
    }
}


- **new Duck()** ✅ (Correct)
- new Animal()
- Duck()
- Animal()

**Explanation:**  
Assigning a Duck object to an Animal reference allows `whatAmI()` to call the overridden method in Duck, displaying "I am a Duck".

---

## 7. What is displayed when you run the following code?

abstract class Animal {
    void sleep() {
        System.out.println("Animal is sleeping.");
    }

    void whatAmI() {
        System.out.println("I am an animal.");
    }
}

class Duck extends Animal {
    @Override
    void whatAmI() {
        System.out.println("I am a Duck.");
    }
}

public class ModuleQuiz_M3L3 {
    public static void main(String[] args) {
        Animal animalObject = new Duck();
        animalObject.whatAmI();
        animalObject.sleep();
    }
}


- It gives a compile time error.
- It displays both “I am an Animal.” and “Animal is sleeping.”
- It displays only “Animal is sleeping.”
- **It displays both “I am a Duck.” and “Animal is sleeping.”** ✅ (Correct)

**Explanation:**  
The overridden `whatAmI()` in Duck is called, and since Duck does not override `sleep()`, the parent version is called.

---

## 8. What is displayed when you run the following code?

interface Moveable {
    void move();
}

class Bike implements Moveable {
    public void move() {
        System.out.println("Bike is moving.");
    }

    public void stop() {
        System.out.println("Bike has stopped.");
    }
}

public class ModuleQuiz_M3L3 {
    public static void main(String[] args) {
        Moveable moveableObject = new Bike();
        moveableObject.stop();
    }
}


- **Bike is moving** ✅ (Correct)
- Bike has stopped.
- No output.
- A compilation error.

**Explanation:**  
The interface reference can only access methods declared in the interface. Only `move()` is called and displayed.

---

## 9. In the code below, what should replace ----- to ensure that the Bike class correctly implements both the Moveable and Hoverable interfaces without becoming abstract?

interface Moveable {
    void move();
}

interface Hoverable {
    void hover();
}

class Bike implements ----- {
    public void ----- {
        System.out.println("one method implemented");
    }

    public void ----- {
        System.out.println("another method implemented");
    }
}


- Moveable and Hoverable.
- A compilation error.
- 123
- **Moveable, Hoverable** ✅ (Correct)
- move()
- hover()
- No output.

**Explanation:**  
To implement multiple interfaces, list them after the `implements` keyword, separated by commas.

---

## 10. Given the following code, what methods should replace ----- to correctly implement the required methods?

interface Steerable {
    void steer();
}

abstract class Vehicle {
    abstract void start();

    void stop() {
        System.out.println("The vehicle stopped.");
    }
}

class Boat extends Vehicle implements Steerable {
    public void ------ {
        System.out.println("Boat has started.");
    }
    
    public void ----- {
        System.out.println("Boat is steering.");
    }    
}


- stop(), steer()
- **start(), steer()** ✅ (Correct)
- stop(), start()
- stop(), stop()

**Explanation:**  
The Boat class must implement the abstract method `start()` from Vehicle and the `steer()` method from Steerable.

---
