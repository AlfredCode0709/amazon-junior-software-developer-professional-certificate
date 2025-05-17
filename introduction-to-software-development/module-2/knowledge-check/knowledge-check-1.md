# Knowledge Check: Conditional Statements – Controlling Program Flow

This document contains the answers and explanations for the knowledge check on "Conditional Statements – Controlling Program Flow".

---

## 1. What is the output of the following code?

int x = 2;
if (x == 5) {
    System.out.println("I am good");
}
System.out.println("I am average");


- A. I am good  
- B. I am average  
- **C. I am good  
   I am average** ✅ (Correct)  
- D. (No output)

**Explanation:**  
That’s correct. The `if` statement has a semicolon immediately after the closing parenthesis of the condition, so control ends there. The rest of the code is executed without any checks.

---

## 2. True or False: The following code will execute correctly:

int x = 5;

else {
  System.out.println("I am good");
}

System.out.println("I am average");


- A. True  
- **B. False** ✅ (Correct)

**Explanation:**  
That’s correct. An `else` statement cannot exist without being associated with a corresponding condition in an `if` statement. An `else` statement is meant to be executed when the `if` statement associated with it is false.

---

## 3. What are the advantages of logical operators over nested if and else statements? Select all that apply.

- **Reduction of complexity by having concise and readable code** ✅ (Correct)  
  It is easier to work with logical operators than nested if-else statements.
- Helps repetition of code  
- **More in tune with the human thought process** ✅ (Correct)  
  Logical operators align with how people naturally consider multiple conditions together, enhancing code readability and understanding.
- **Minimizing unnecessary evaluations** ✅ (Correct)  
  Logical operators like `&&` (AND) and `||` (OR) stop evaluating as soon as the outcome is determined, optimizing performance.

**Example:**  
Concise with logical operators:

if (x == 2 && y == 5 && z != 4) {
    // do something here
}

Nested if-else:

if (x == 2) {
    if (y == 5) {
        if (z != 4) {
            // do something here
        }
    }
}


---

## 4. Choose the correct statements. Select all that apply.

- A default statement is compulsory in a switch case.  
- A switch statement can be used to compare values using the comparison operators like >, < , >= and so on.  
- **A switch statement is equivalent to using multiple if statements. We can use multiple if statements in place of a switch, but a switch statement helps us reduce code.** ✅ (Correct)  
  A switch statement is a short form for multiple if statements with equality checks only.
- **A switch statement makes the code easier and more concise when multiple if equality checking is required.** ✅ (Correct)  
  A default is purely optional. Yes, a switch statement makes it easier to make multiple equality checks.

---

## 5. Review the code block below and choose the correct display that you would get:

int x = 2;
switch (x) {
    case 2:
        System.out.print("A ");
    case 4:
        System.out.print("B ");
    case 12:
        System.out.print("C ");
    default:
        System.out.print("D ");
}

- A. A  
- B. B  
- **C. A B C D** ✅ (Correct)  
- D. A C

**Explanation:**  
That’s correct. A "fall through" occurs since when the 1st case (`case 2`) matches with the value of `x`, which is 2, the code after it is executed till it does not encounter a `break` statement or the closing curly brace of the switch. So, it displays `A B C D`.

---
