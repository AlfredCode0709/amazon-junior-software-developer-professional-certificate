# Knowledge Check: Inheritance and Polymorphism – Super and Sub Classes

This document contains the answers and explanations for the knowledge check on "Inheritance and Polymorphism – Super and Sub Classes".

---

## 1. Which of the following statements about inheritance in Java is accurate?

- A superclass in Java can inherit methods from its subclass.
- **A subclass in Java can only inherit from a single superclass.** ✅ (Correct)
- Java allows a subclass to inherit from multiple superclasses.
- A subclass in Java is not allowed to override methods from its superclass.

**Explanation:**  
That’s correct. In Java, a subclass can only inherit from one superclass (single inheritance), not multiple superclasses[1][5][6].

---

## 2. Which of the following statements correctly describes polymorphism in Java?

- Polymorphism allows objects to be treated as instances of their subclass instead of their superclass.
- Polymorphism in Java prevents a class from defining multiple methods with the same name.
- Polymorphism in Java applies solely to methods, not to variables.
- **Polymorphism allows a superclass reference to refer to an object of a subclass.** ✅ (Correct)

**Explanation:**  
That’s correct. Polymorphism allows a superclass reference to refer to an object of any subclass, enabling flexible and dynamic method invocation[2][6].

---

## 3. Considering the Java code snippet below, what will be the output?

class Animal {
    public void makeSound() {
        System.out.println("Some generic animal sound");
    }
}
class Dog extends Animal {
    @Override
    public void makeSound() {
        System.out.println("Bark");
    }
}


- The code will produce runtime errors.
- The code will fail to compile.
- "Some generic animal sound" will be printed.
- **"Bark" will be printed.** ✅ (Correct)

**Explanation:**  
That’s correct. The `makeSound()` method in the Dog class overrides the one in Animal, so "Bark" is printed when called on a Dog object[6].

---

## 4. Suppose you are developing a vehicle rental system. You have a Vehicle superclass with a `calculateRentalCost()` method. Subclasses like Car, Truck, and Motorcycle each implement this method based on different rental rate calculations.

Which of the following best describes how polymorphism is applied in this scenario?

- Polymorphism mandates that each subclass include unique methods unrelated to the Vehicle class.
- Polymorphism requires that all subclasses implement `calculateRentalCost()` identically.
- **Polymorphism allows a Vehicle reference to invoke `calculateRentalCost()` on any subclass, executing the subclass-specific implementation.** ✅ (Correct)
- Polymorphism restricts subclasses from adding new methods.

**Explanation:**  
That’s correct. Polymorphism lets you invoke `calculateRentalCost()` on a Vehicle reference, executing the method specific to the subclass, enabling dynamic method dispatch[2][4][6].

---

## 5. What is the main purpose of the `super` keyword in Java?

- **To access superclass methods and variables from within a subclass.** ✅ (Correct)
- To mark a method for overriding in a subclass.
- To create multiple instances of a class.
- To create a new subclass from an existing class.

**Explanation:**  
That’s correct. The `super` keyword is used to refer to the immediate superclass of a subclass, allowing access to its methods and variables[4][5].

---
