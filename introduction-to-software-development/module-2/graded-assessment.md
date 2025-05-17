# Control Flow - Statements and Loops

This document contains the answers and explanations for the knowledge check on "Control Flow - Statements and Loops".

---

## 1. Select the correct output for the following code snippet:

int checkVal = 15;

if (checkVal > 12) {
    System.out.println("A");
}


- Compilation error  
- **A** ✅ (Correct)  
- None of the options  
- No output  

**Explanation:**  
Since `checkVal` is greater than 12, the if statement is true, so it executes the code inside the if statement to display "A".

---

## 2. Select the correct output for the following code:

public class Main {
    public static void main(String[] args) {
        int num = 10;
        boolean result = num == 10;
        System.out.println(result);
    }
}


- **true** ✅ (Correct)  
- false  
- !A  
- Compilation error  

**Explanation:**  
The expression `num == 10` checks whether the value of num is equal to 10. Since num is indeed 10, the result is true.

---

## 3. Select the correct output for the following code snippet:

int checkVal = 15;

if (checkVal <= 15) {
    System.out.println("**");
} else if (checkVal < 12) {
    System.out.println("##");
    if (checkVal == 15) {
        System.out.println("$$");
    }
} else {
    // ...
}


- **\*\*** ✅ (Correct)  
- ##  
- @@  

**Explanation:**  
Since `checkVal` is 15, it satisfies the condition `if(checkVal <= 15)`, which is true. Therefore, "**" is displayed as the code inside the if statement executes.

---

## 4. Select the correct output for the following code:

int checkVal = 25;

if (checkVal > 10) {
    if (checkVal < 20) {
        System.out.println("##");
    } else {
        System.out.println("@@");
    }
}


- No display.  
- **@@** ✅ (Correct)  
- None of the options  
- Compilation error  

**Explanation:**  
The if statement checks if `checkVal > 10`, which is true. It then checks if `checkVal < 20`, which is false. Consequently, it executes the else part of this second level if statement and displays "@@".

---

## 5. Select the correct output for the following code:

int variable1 = 5, variable2 = 10;

if (variable1 > 3 && variable2 < 25) {
    System.out.println("##");
}


- None of the options  
- No output   
- **##** ✅ (Correct)  
- Compilation error  

**Explanation:**  
`variable1` is greater than 3 and `variable2` is less than 25, so the condition is true. Therefore, "##" is displayed.

---

## 6. Select the correct output for the following code:

int month = 6;
switch (month) {
    case 1:
        System.out.println("January");
        break;
    case 2:        
        System.out.println("February");
        break;
    case 3:        
        System.out.println("March");
        break;
    case 10:        
        System.out.println("October");
        break;
    case 11:        
        System.out.println("November");
        break;
    case 12:        
        System.out.println("December");
        break;
    default:        
        System.out.println("Invalid month for a playing with snow in our zone.");
}

- November  
- November December  
- June  
- **Invalid month for playing with snow in our zone** ✅ (Correct)  

**Explanation:**  
The switch statement checks the variable `month` for equality against the case statements. Since the variable `month` has a value of 6, none of the case statements match, so the default code is executed.

---

## 7. Select all the correct outputs for the following code:

int i;
for (i = 10; i >= 0; i -= 2) {
    System.out.println(" " + i);
}


- No output  
- **10 8 6 4 2 0** ✅ (Correct)  
- 10 8 6 4 2 0 -2  
- 10 9 8 7 6 5 4 3 2 1 0  

**Explanation:**  
The loop runs as long as the condition `i >= 0` is true. Starting with i set to 10, it decreases by 2 each iteration. So, i takes values 10, 8, 6, 4, 2, 0, and finally -2. However, the loop stops executing when i is -2 because -2 >= 0 is false.

---

## 8. Select the correct output for the following code:

int loopVar = 1;
while (loopVar <= 3) {
    System.out.print("Value= " + loopVar);
}


- Value = 1 Value = 2 Value = 3  
- **Infinite loop** ✅ (Correct)  
- Compilation error  
- None of the options  

**Explanation:**  
The variable `loopVar` starts with an initial value of 1, and the loop continues as long as loopVar is less than or equal to 3. However, loopVar is never updated inside the loop, so it remains 1 indefinitely. This leads to the continuous display of "Value = 1" until the program is terminated.

---

## 9. Select all the values that will be displayed for the following code:

int loopVar = 12;

do {
    System.out.println(" " + loopVar);
    loopVar = loopVar - 4;
} while (loopVar <= 3);


- 12 8 4  
- A do-while does not end with a semicolon.  
- Compilation error  
- **12** ✅ (Correct)  

**Explanation:**  
A do-while loop executes at least once, regardless of the initial condition, and checks the condition after each iteration. Here, initially, loopVar is set to 12. The loop runs once and displays 12. Then, loopVar is updated to 8, and the condition 8 <= 3 fails immediately, causing the loop to stop.

---

## 10. Select all the values that would be displayed for the following code:

int x = 12;

if (x > 10) {
    System.out.print("A");

    switch (x) {
        case 12:
            System.out.print("B");
            break;
        case 14:
            System.out.print("D");
            break;
    }

} else {
    System.out.print("Z");
}


- Z  
- AD  
- **AB** ✅ (Correct)  
- None of the options  

**Explanation:**  
With x set to 12, the first condition `if(x > 10)` is true, displaying "A". Then in the switch statement, the case 12 is also true, displaying "B". Therefore, "AB" is displayed.

---
