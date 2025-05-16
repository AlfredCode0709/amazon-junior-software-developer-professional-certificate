# Module Quiz: Getting Started with Java

This document contains the answers and explanations for the module quiz on getting started with Java.

---

## 1. If `count = 30`, what is the new value of `count` after `count -= 5`?

- A. 30  
- B. 35  
- C. 5  
- **D. 25** ✅ (Correct)

**Explanation:**  
That’s correct. When we use the compound assignment operator `-=`, it subtracts the value on the right from the existing value of the assignee and assigns the value back to the assignee. So, `count -= 5` is the same as `count = count - 5` or `count = 30 - 5`, which is 25.

---

## 2. Select the correct output for the following code:

public class Main {
public static void main(String[] args) {
int num = 20;
boolean result = num != 15;
System.out.println(result);
}
}


- A. 25  
- B. 20  
- **C. true** ✅ (Correct)  
- D. false

**Explanation:**  
That’s correct. The expression `num != 15` checks whether the value of `num` is not equal to 15. Since `num` is 20, the result is `true`.

---

## 3. Alex is writing a program to store user information. How would he declare an integer variable named `age` and initialize it to 20?

- A. `age = 20;`  
- **B. `int age = 20;`** ✅ (Correct)  
- C. `var age = 20;`  
- D. `integer age = 20;`

**Explanation:**  
That’s correct. When you want to declare and initialize the int variable in a single line, then `int age = 20` is correct.

---

## 4. Andrea is working on a text processing application and needs to extract a specific part of a String. What method would she use to extract the substring "Dark" from the String `sentence = "The Dark Web"`?

- A. `sentence.sub(4, 8)`  
- **B. `sentence.substring(4, 8)`** ✅ (Correct)  
- C. `sentence.subString(4, 8)`  
- D. `sentence.slice(4, 8)`

**Explanation:**  
That’s correct. The String class has a method called `substring(int start, int end)`. The `substring()` method extracts characters from a String between two specified indices (positions) and returns the resulting substring.

---

## 5. Imagine you are writing a welcome message for a user in an application. Which code snippet would you use to combine the Strings `greeting = "Hello"` and `name = "Alice"` with a comma and a space in between?

- A. `greeting + name + ", "`  
- **B. `greeting + ", " + name`** ✅ (Correct)  
- C. `greeting.concat(", " + name)`  
- D. `greeting.concat(", ", name)`

**Explanation:**  
That’s correct. The `+` operator concatenates `greeting` and `name` with `", "` in between, resulting in the output "Hello, Alice". The other options either misuse the concat operator or incorrectly place the comma and space.

---

## 6. Tom is debugging his Java program and comes across a line of code that is causing an error. What is wrong with the following code snippet that Tom identifies?

int number = 10.5;


- A. There's nothing wrong; the code is correct.  
- B. The variable name is incorrect.  
- **C. The variable type int cannot hold decimal values.** ✅ (Correct)  
- D. The value should be enclosed in double quotes.

**Explanation:**  
That’s correct. The `int` data type is used for whole numbers (integers) and cannot store decimal values.

---

## 7. Which data type is used to store whole numbers in Java?

- A. double  
- B. float  
- **C. int** ✅ (Correct)  
- D. char

**Explanation:**  
That’s correct. `int` can store only whole numbers. If you want to store decimal numbers, use the `double` data type.

---

## 8. The symbol for the logical AND operator in Java is ________

- **A. `&&`** ✅ (Correct)  
- B. `||`  
- C. `&`  
- D. `and`

**Explanation:**  
That’s correct. `&&` is the logical AND operator. This operator evaluates to “true” only if the expressions on both sides are true.

---

## 9. Select the correct output for the following code:

public class Main {
public static void main(String[] args) {
int remainder = 22 % 6;
System.out.println(remainder);
}
}


- A. 2  
- **B. 4** ✅ (Correct)  
- C. 0  
- D. 1

**Explanation:**  
That’s correct. `22 % 6` results in 4. The modulo (or remainder) operator `%` returns the remainder after dividing the first number by the second number. In this case, 22 divided by 6 is 3, with a remainder of 4.

---

## 10. True or False: A String object in Java can be modified directly after it is created.

- A. True  
- **B. False** ✅ (Correct)

**Explanation:**  
That’s correct. Strings are immutable in Java, meaning their content cannot be changed once created.

---
