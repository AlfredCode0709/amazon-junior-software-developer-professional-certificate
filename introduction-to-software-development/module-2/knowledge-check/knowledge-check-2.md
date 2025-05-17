# Knowledge Check: Iterative Structures – For and While Loops

This document contains the answers and explanations for the knowledge check on "Iterative Structures – For and While Loops".

---

## 1. Consider the following code and choose the correct output.

int loopVar;

for (loopVar = 7; loopVar >= 1; loopVar--) {
    System.out.println("Hello");
}

- "Hello" is displayed six times, and loopVar = 1.
- "Hello" is displayed seven times and loopVar = 1.
- **"Hello" is displayed seven times, and loopVar = 0.** ✅ (Correct)
- None of the options.

**Explanation:**  
The initial value of loopVar is 7 and it is decremented by 1 with each run of the for loop. The for loop continues until loopVar >= 1. When loopVar = 0, the program will stop, returning the String "Hello" seven times.

---

## 2. True or False: The output of the following code block returns `Value : 2 Value : 5`.

for (int loopVar = 1; loopVar < 10; loopVar += 3) {
    System.out.print("\tValue : " + loopVar);
}


- False
- **True** ✅ (Correct)

**Explanation:**  
The value of loopVar starts at 1 and increments by 3 after each loop. The last value must be less than 10. The values printed are 1, 4, and 7. Therefore, the output is not `Value : 2 Value : 5`.

---

## 3. Explore the following code block. Select all that apply.

int numberToEvaluate = 11111;

while (numberToEvaluate > 0) {
    numberToEvaluate = numberToEvaluate / 10;
    System.out.println("The number: " + numberToEvaluate);
}


- **The println() method creates line breaks.** ✅ (Correct)
- **The while loop executes until a condition is met.** ✅ (Correct)
- The output displays an error.
- **The loop will execute five times.** ✅ (Correct)

**Explanation:**  
- The `println()` method prints each message on a new line.
- The `while` loop runs as long as `numberToEvaluate > 0`.
- The loop will execute five times, as each time the value is divided by 10, reducing the number of digits until it reaches 0.

---

## 4. Consider the following code and choose the correct output.

int loopVar = 12;

do {
    System.out.println("The number: " + loopVar + " gives the condition (loopVar <10) as: " + (loopVar < 10));
} while (loopVar < 10);


- **The output indicates The number: 12 gives the condition (loopVar <10) as: false.** ✅ (Correct)
- The output displays an error.
- The loop displays: The number: 12 gives the condition (loopVar <10) is true.
- The condition loopVar < 10 is false, and the loop stops.

**Explanation:**  
A do-while loop first executes the loop body and then checks the condition. In this code, the condition is false, so the loop executes only once and prints the statement.

---

## 5. Toni is selling ice cream, but he is running low on stock. Therefore, Toni instructs SideKick to buy ice cream containers while he is manning the store. SideKick can only carry three containers at a time. Explore the following code block and choose the correct answer.

int iceCreamForToni = 4;

while (iceCreamForToni <= 2) {
    System.out.println(iceCreamForToni + " ");
    iceCreamForToni = iceCreamForToni + 3;
}


- **No output** ✅ (Correct)
- 3 6
- Syntax Error.
- 4 8 12

**Explanation:**  
The variable `iceCreamForToni` starts at 4, but the condition `iceCreamForToni <= 2` is false from the start, so the loop body never executes and there is no output.

---
