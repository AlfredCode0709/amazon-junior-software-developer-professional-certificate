# Course Quiz: Introduction to Software Development

This document contains answers and explanations for the course quiz on Introduction to Software Development.

---

## 1. To create an object `myCar` of class `Car`, which syntax is correct?

- Car = new myCar();
- myCar = new Car();
- **Car myCar = new Car();** ✅ (Correct)
- Car myCar();

**Explanation:**  
This syntax initializes a new object of the class Car. The `new` keyword creates a new object and assigns it to the variable `myCar`, which is of type `Car`.

---

## 2. Given an object `person` of class `Person` with a field `age`, how do you access the age field?

- person->age;
- **person.age;** ✅ (Correct)
- age.person;
- Person.age;

**Explanation:**  
You can access the variable `age` from the `person` object using `person.age`. This follows the standard pattern of accessing an object’s fields or methods in Java: `objectName.fieldName`.

---

## 3. Complete the sentence: In Java, a constructor…:

- Can return multiple values.
- Is a method that can be overridden.
- Is only called once during the class definition.
- **Is used to initialize objects.** ✅ (Correct)

**Explanation:**  
A constructor is a special method used to initialize objects.

---

## 4. You want to create `Customer` objects with either specific data or default values. What should you do?

- **Define multiple constructors, including a no-arg constructor and parameterized constructor.** ✅ (Correct)
- Use static factory methods.
- Use only a default constructor.
- Avoid constructors and initialize data manually.

**Explanation:**  
Multiple constructors allow creating objects with different initializations based on provided or default data.

---

## 5. In a Java class `Book`, what is the correct method signature for `getTitle` that returns a `String`?

- getTitle(String)
- title getTitle()
- **String getTitle()** ✅ (Correct)
- void getTitle()

**Explanation:**  
The method `getTitle` is correctly defined to return a `String`, which is the title of the book. The parentheses indicate that the method takes no parameters.

---

## 6. True or False: In Java, the `this` keyword refers to the current instance of the class.

- False
- **True** ✅ (Correct)

**Explanation:**  
The `this` keyword is used within a method or constructor to refer to the current object.

---

## 7. Which for loop will correctly calculate the sum of the first 100 positive integers?

- for (int i = 1; i < 100; i++) { sum += i; }
- **for (int i = 1; i <= 100; i++) { sum += i; }** ✅ (Correct)
- for (int i = 0; i < 100; i++) { sum += i; }
- **for (int i = 0; i <= 100; i++) { sum += i; }** ✅ (Correct)

**Explanation:**  
This loop starts at 1 and continues through 100, correctly adding each integer to the sum.

---

## 8. Which while loop correctly prints numbers from 1 to 10?

- int currentNumber = 0; while (currentNumber < 10) { currentNumber++; System.out.println(currentNumber); }
- int currentNumber = 1; while (currentNumber < 10) { System.out.println(currentNumber); currentNumber++; }
- **int currentNumber = 1; while (currentNumber <= 10) { System.out.println(currentNumber); currentNumber++; }** ✅ (Correct)
- int currentNumber = 10; while (currentNumber > 0) { System.out.println(currentNumber); currentNumber--; }

**Explanation:**  
This loop starts at 1 and continues through 10, printing each number.

---

## 9. How would you use a do-while loop to calculate the factorial of a given positive integer n?

--**✅ (Correct)**
int factorial = 1;
int i = 1;
do {
    factorial *= i;
    i++;
} while (i <= n);
--**✅ (Correct)**


int factorial = 1;
int i = 0;
do {
    factorial *= i;
    i++;
} while (i < n);


int factorial = 1;
int i = 1;
do {
    factorial *= i;
} while (i < n);


int factorial = 1;
int i = 1;
do {
    factorial *= i;
    i--;
} while (i > 0);

**Explanation:**  
This loop multiplies each number from 1 to n, ensuring the loop runs at least once.

---

## 10. You are implementing a Java program that calculates discounts based on customer membership status. The program should apply a 10% discount for “Gold” members, 5% for “Silver” members, and no discount for “Regular” members. Which if-else statement correctly applies the discount based on membership status?

if (membership.equals("Gold") || membership.equals("Silver")) {
    discount = 0.10;
} else {
    discount = 0.00;
}


if (membership.equals("Gold")) {
    discount = 0.10;
} else {
    discount = 0.05;
}


if (membership == "Gold") {
    discount = 0.10;
} else if (membership == "Silver") {
    discount = 0.05;
} else {
    discount = 0.00;
}

--**✅ (Correct)**
if (membership.equals("Gold")) {
    discount = 0.10;
} else if (membership.equals("Silver")) {
    discount = 0.05;
} else {
    discount = 0.00;
}
--**✅ (Correct)**

**Explanation:**  
This statement uses `equals` to correctly compare Strings and applies the appropriate discount for each membership type.

---

## 11. In a Java program, you are creating a feature that assigns a grade based on a student's score. The grades are “A” for 90-100, “B” for 80-89, “C” for 70-79, “D” for 60-69, and “F” for below 60. Which switch statement correctly assigns the grade based on the student's score?  

switch (score) {
    case 90:
    case 80:
    case 70:
    case 60:
        grade = 'A';
        break;
    case 50:
        grade = 'B';
        break;
    default:
        grade = 'F';
}


--**✅ (Correct)**
switch (score / 10) {
    case 10:
    case 9:
        grade = 'A';
        break;
    case 8:
        grade = 'B';
        break;
    case 7:
        grade = 'C';
        break;
    case 6:
        grade = 'D';
        break;
    default:
        grade = 'F';
}
--**✅ (Correct)**


switch (score) {
    case 10:
    case 9:
        grade = 'A';
        break;
    case 8:
        grade = 'B';
        break;
    case 7:
        grade = 'C';
        break;
    case 6:
        grade = 'D';
        break;
    default:
        grade = 'F';
}


switch (score) {
    case 100:
        grade = 'A';
        break;
    case 90:
        grade = 'A';
        break;
    case 80:
        grade = 'B';
        break;
    case 70:
        grade = 'C';
        break;
    case 60:
        grade = 'D';
        break;
    default:
        grade = 'F';
}

**Explanation:**  
This switch statement uses integer division to categorize the score into the correct grade range.

---

## 12. Which method should you use to determine the number of characters in a username String?

- size()
- getLength()
- count()
- **length()** ✅ (Correct)

**Explanation:**  
The `length()` method in Java is used to find the number of characters in a String.

---

## 13. In a Java program, you need to keep track of the number of items in a cart. You decide to use an integer variable to store this number and set it to zero initially, as the cart starts empty. Complete the code to correctly declare and initialize an integer variable for the number of items in the cart: _____ itemsInCart = ___;.

- 0, int
- **int, 0** ✅ (Correct)
- int, "zero"
- itemsInCart, 0

**Explanation:**  
The `int` keyword specifies the type of the variable, and `0` initializes it.

---

## 14. You are building a Java application with a base class Employee that has a method calculateSalary(). You have a subclass Manager that needs to use the salary calculation from Employee but with an additional bonus. Fill in the blank to call the calculateSalary() method from the Employee class within the Manager class.

class Manager extends Employee {
    private double bonus;

    public double calculateSalary() {
        double baseSalary = super._____();
        return baseSalary + bonus;
    }
}

- salary
- calculate
- **calculateSalary** ✅ (Correct)
- getSalary

**Explanation:**  
The `super.calculateSalary()` call is used to invoke the method from the superclass Employee.

---

## 15. True or False: In Java, the `public` access modifier allows a class member to be accessible from any other class in any package.

- False
- **True** ✅ (Correct)

**Explanation:**  
The `public` access modifier provides the widest access level, allowing class members to be accessed from any class in any package.

---
