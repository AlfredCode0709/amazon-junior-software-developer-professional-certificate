# Knowledge Check: Java Basics - Variables and Operators

This document contains the answers and explanations for the knowledge check on "Java Basics - Variables and Operators".

---

## 1. What is the correct way to declare and initialize an integer variable named `yearsOld` in Java?

- A. `int yearsOld = "ten";`
- B. `String yearsOld = 10;`
- **C. `int yearsOld = 10;`** ✅ (Correct)
- D. `double yearsOld = 10.0;`

**Explanation:**  
That's correct. This declares an integer variable `yearsOld` and initializes it with the value 10.

---

## 2. What will be the output of the following code?

public class SampleCode {
public static void main(String[] args) {
int age = 12;
String name = "Tom";
System.out.println("Age: " + age + ", Name: " + name);
}
}

- A. Age: 12 Name Tom  
- B. Age: 12 Name: Tom  
- **C. Age: 12, Name: Tom** ✅ (Correct)  
- D. 12, Tom

**Explanation:**  
That's correct. The `System.out.println` statement prints the text with the correct formatting. Everything that is surrounded with `" "` will be displayed exactly as it was typed.

---

## 3. What is wrong with the following code?

int number;
number = "5";

- A. The variable `number` is not declared.
- B. The variable `number` should be declared as a character.
- C. The value `5` should be a character.
- **D. The value `5` should be a number and should be assigned as `number = 5;`** ✅ (Correct)

**Explanation:**  
That's correct. The value assigned to the variable `number` should be a numeric value without quotation marks, like `5`.

---

## 4. Which of the following variable declarations is the most appropriate to store a single letter `'K'` in Java?

- A. `String letter = 'K';`
- B. `char letter = "K";`
- **C. `char letter = 'K';`** ✅ (Correct)
- D. `String letter = "K";`

**Explanation:**  
That's correct. This correctly declares a `char` variable with the single letter `'K'`.

---

## 5. What is the output of the following code?

public class SampleCode {
public static void main(String[] args) {
int a = 5;
int b = 10;
int sum = a + b;
System.out.println("Sum: " + sum);
}
}

- A. Sum: a + b  
- B. Sum: 5 + 10  
- C. Sum: 510  
- **D. Sum: 15** ✅ (Correct)

**Explanation:**  
That's correct. The code correctly adds the values of `a` and `b`, resulting in `15`. In the print line, the addition operator concatenates the `"Sum:"` and the value of the variable `sum`.

---
