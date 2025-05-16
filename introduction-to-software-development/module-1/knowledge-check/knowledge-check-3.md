# Knowledge Check: Strings - Working with text in Java

This document contains the answers and explanations for the knowledge check on "Strings - Working with text in Java".

---

## 1. In the following code block, which snippet would you insert to correctly determine the String length in Java?

public class Main {
public static void main(String[] args) {
String text = "Java is fun!";
int length = text.__________;
System.out.println("The length of the string is: " + length);
}
}


- A. **`length()`** ✅ (Correct)
- B. `count()`
- C. `getLength()`
- D. `size()`

**Explanation:**  
That's correct. The `length()` method returns the number of characters in a String.

---

## 2. While formatting a document, you’re asked to replace all instances of the word "old" with the word "new". You’ve been provided with the following code. What method would you insert to make the required changes?

public class Main {
public static void main(String[] args) {
String document = "This is an old document. The old content needs to be updated.";
String updatedDocument = document.__________("old", "new");
System.out.println(updatedDocument);
}
}


- A. `substitute()`
- B. `swap()`
- C. `change()`
- D. **`replace()`** ✅ (Correct)

**Explanation:**  
That’s correct. The `replace()` method can replace all the occurrences of a specified substring with a new substring. For example, replace "old" with "new".

---

## 3. You are developing a user registration system and need to ensure that the first letter of a username is not a digit. You are using the following code block. Which method would you insert to check the first character?

public class Main {
public static void main(String[] args) {
String username = "1JohnDoe";
if (Character.isDigit(username.__________(0))) {
System.out.println("The username cannot start with a digit.");
} else {
System.out.println("The username is valid.");
}
}
}


- A. **`charAt(int index)`** ✅ (Correct)
- B. `firstChar()`
- C. `initialChar()`
- D. `getChar(int index)`

**Explanation:**  
That’s correct. The `charAt(int index)` method returns the character at the specified index. For example, if you want to check the index in the String “Jonas”, `charAt(0)` will return “J”.

---

## 4. Toni is writing a Java program to set a password for the alarm system. Toni needs to compare a user's input with a stored password in a case-sensitive manner. Toni is working with the following code. Which method would Toni insert to achieve this?

public class Main {
public static void main(String[] args) {
String storedPassword = "SecurePass123";
String userInput = "securepass123";
    if (storedPassword.__________(userInput)) {
        System.out.println("Access granted.");
    } else {
        System.out.println("Access denied. Incorrect password.");
    }
}


- A. `compare()`
- B. `==`
- C. `match()`
- D. **`equals()`** ✅ (Correct)

**Explanation:**  
That's correct. The `equals()` method checks if two Strings have the same content and can be used to compare two passwords case-sensitively.

---

## 5. True or False: To capitalize the first letter of each word in a String, you can use the `toTitleCase()` method.

- A. True
- **B. False** ✅ (Correct)

**Explanation:**  
That’s correct. Java does not have a built-in method to capitalize the first letter of each word in a String. You'll have to implement a custom method.

---
