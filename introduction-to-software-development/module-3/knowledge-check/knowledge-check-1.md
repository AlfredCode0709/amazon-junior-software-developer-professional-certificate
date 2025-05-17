# Knowledge Check: Classes and Objects – Making Code Reusable

This document contains the answers and explanations for the knowledge check on "Classes and Objects – Making Code Reusable".

---

## 1. Imagine you're building a game with different characters. You want to create a blueprint for each character that defines their properties (like name, health) and actions (like attack). Which of the following concepts enables you to do this?

- Variables  
- Loops  
- Objects  
- **Classes** ✅ (Correct)

**Explanation:**  
That’s correct. Classes act as blueprints that define the properties (name, health) and functionalities (attack) that all characters will have. Each character in the game would be an object created from this class.

---

## 2. Let's say you created a Character class with a method to display the character's health. How can you create multiple characters (such as a knight or an archer) with different health values but reuse the same method to display their health?

- Copy and paste the display health method into separate classes for each character.  
- There's no way to reuse the method with different health values.  
- **Create objects from the Character class and assign different health values to each object.** ✅ (Correct)  
- Create a single health variable outside the Character class and track which character it belongs to when displaying health.

**Explanation:**  
That’s correct. This approach reuses the display health method from the Character class while allowing each character object (knight or archer) to have its individual health value.

---

## 3. You designed a Calculator class with a method to add two numbers. How can you easily reuse this class to also perform subtractions?

- Use the addition method in a different way to achieve subtraction. For example, to calculate 10 minus 5, you might use the addition method: 10 + (a negative number representing 5).  
- Duplicate the entire Calculator class and rename it to Subtractor.  
- The Calculator class is specifically designed for addition and cannot be reused for subtraction.  
- **Write a separate method for subtraction within the Calculator class.** ✅ (Correct)

**Explanation:**  
That’s correct. This enables you to extend the functionality of the Calculator class without modifying the existing addition method.

---

## 4. You're designing a Point class in Java to represent a location in 2D space with x and y coordinates. The class currently has a no-argument constructor (meaning it takes no arguments). You haven't explicitly assigned values within the constructor for the x and y coordinates (type int).

What will happen to the x and y coordinates of a new Point object created using this no-argument constructor?

- The new Point object will be created with random values for x and y.  
- The new Point object will not be created due to an incomplete constructor.  
- **The object will be created with its x and y coordinates set to their default values (0 for integers in Java).** ✅ (Correct)  
- The new Point object will only be created if values are provided during creation.

**Explanation:**  
That’s correct. In Java, when you leave numbers uninitialized within a constructor, they are automatically set to their default values. For integers, the default value is 0. So, new Point objects created using this no-argument constructor will have both x and y coordinates set to 0.

---

## 5. True or False: In Java, all methods must return a value.

- True  
- **False** ✅ (Correct)

**Explanation:**  
That’s correct. Not all methods in Java must return a value. Methods can be declared with a void return type, indicating they don't return any specific value. These methods are often used to perform actions or modify objects without needing to return something explicitly.

---
