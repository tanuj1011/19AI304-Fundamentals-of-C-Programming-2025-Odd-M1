# 19AI304-Fundamentals-of-C-Programming-2025-Odd-M1
# IAPR-1- Module 1 - FoC
## 1. Implementation of basic C programs using Literals,Consonants, Variables, Data types.
## 2. Implementation of different categories of operators.
# Ex.No:1
  Build a C program to demonstrate the usage of different types of literals: integer, float, character, and string.  
# Date : 21.11.2025 
# Aim:
To build a C program that prints integer, float,character, and string literals on the console using the printf() function.
# Algorithm:
### Step 1:
  Start
### Step 2: 
  Include the standard input-output library: #include<stdio.h>.
### Step 3: 
  Inside the main() function, use printf() to display each literal along with its size in bytes using sizeof() :
  
   3.1 Integer literal (e.g., 10) using `%d`
   
   3.2 Float literal (e.g., 3.14) using `%f`
   
   3.3 Character literal (e.g., 'A') using `%c`
   
   3.4 String literal (e.g., "Hello C") using `%s`
   
### Step 4: 
   Stop
# Program:
```
#include <stdio.h>
int main() {
    printf("Integer literal: %d\n", 25);
    printf("Float literal: %.2f\n", 12.75);
    printf("Character literal: %c\n", 'A');
    printf("String literal: %s\n", "Hello, World!");
    return 0;
}
```
# Output:

<img width="460" height="207" alt="image" src="https://github.com/user-attachments/assets/ccaae68d-55d6-427c-9004-7f40d321cfd2" />

# Result: 
Thus, the program was implemented and executed successfully, and the required output was obtained.


# 19AI304-Fundamentals-of-C-Programming-2025-Odd
# IAPR-1- Module 1 - FoC
# Ex.No:2
  Build a C program to display the value of a macro constant and a constant variable.
# Date : 21.11.2025 
# Aim:
  To build a C program that demonstrates the use of macro constants and constant variables.
# Algorithm:
### Step 1:
  Start  
### Step 2: 
  Include the standard input-output library: #include<stdio.h>.
### Step 3: 
  Define a macro constant `PI` with value `3.14159` using `#define`.
### Step 4: 
   Inside `main()`:
   
   4.1 Declare a constant integer variable `DAYS`
   
   4.2 Initialize it with the value `7`
   
### Step 5:  
  Use `printf()` to display the values of `PI` and `DAYS`.     
### Step 6:  
  Stop
# Program:
```
#include <stdio.h>

// Macro constant
#define PI 3.14

int main() {
    // Constant variable
    const int DAYS_IN_WEEK = 7;

    printf("Macro constant PI: %.2f\n", PI);
    printf("Constant variable DAYS_IN_WEEK: %d\n", DAYS_IN_WEEK);

    return 0;
}
```
# Output:

<img width="519" height="157" alt="image" src="https://github.com/user-attachments/assets/0fbdfc73-4535-4a1a-b0e3-24e4d64db9cf" />

# Result: 
Thus, the program was implemented and executed successfully, and the required output was obtained.


# 19AI304-Fundamentals-of-C-Programming-2025-Odd
# IAPR-1- Module 1 - FoC
# Ex.No:3
  Build a C program to demonstrate the use of different data types such as int, float, double, and char, and display their values using printf().
# Date : 21.11.2025 
# Aim:
  To build a C program that declares variables of various data types—integer, float, double, and character—initializes them, and prints their values on the screen.
# Algorithm:
### Step 1:
  Start
### Step 2: 
  Include the standard input-output library: #include<stdio.h>.
### Step 3: 
  Inside main(), declare and initialize variables of types int, float, double, and char.
### Step 4: 
   Display their values using printf().
### Step 5:    
   Stop
# Program:
```
#include <stdio.h>
int main() {
    int age = 25;                
    float height = 5.8f;         // float
    double distance = 12345.678; // double
    char grade = 'A';            // char

    printf("Integer value (age): %d\n", age);
    printf("Float value (height): %.2f\n", height);
    printf("Double value (distance): %.3lf\n", distance);
    printf("Character value (grade): %c\n", grade);

    return 0;
}
```
# Output:

<img width="551" height="205" alt="image" src="https://github.com/user-attachments/assets/b036ff6d-0424-42a0-a823-042f0bdba3c5" />

# Result: 
Thus, the program was implemented and executed successfully, and the required output was obtained.

# 19AI304-Fundamentals-of-C-Programming-2025-Odd
# IAPR-1- Module 1 - FoC
# Ex.No:4
  Build a C program to perform arithmetic and bitwise operations on two integers entered by the user. The program should display: Arithmetic operations: addition, subtraction, multiplication, division, and remainder. Bitwise operations: AND, OR, XOR, left shift, right shift, and NOT.
# Date : 21.11.2025 
# Aim:
  To build a C program that takes two integers as input and demonstrates the arithmetic and bitwise operations, displaying the results of each operation.
# Algorithm:
### Step 1:
  Start
### Step 2: 
  Include the standard input-output library: #include<stdio.h>.
### Step 3: 
  Declare two integer variables a and b.
### Step 4: 
   Prompt the user to enter two integers and read the input using scanf().
### Step 5:    
   Perform arithmetic operations on a and b:
   #### Sum (a + b)
   #### Difference (a - b)
   #### Product (a * b)
   #### Quotient (a / b)
   #### Remainder (a % b)
### Step 6: 
  Perform bitwise operations on a and b:
  #### AND (a &amp; b)
  #### OR (a | b)
  #### XOR (a ^ b)
  #### Left shift (a << b)
  #### Right shift (a >> b)
  #### Bitwise NOT of a (~a) and b (~b)
### Step 7:   
  Display the results of all operations using printf().
### Step 8:   
  Stop
# Program:
```
#include <stdio.h>
int main() {
    int a, b;
    printf("Enter two integers: ");
    scanf("%d %d", &a, &b);
    printf("\n--- Arithmetic Operations ---\n");
    printf("Addition: %d + %d = %d\n", a, b, a + b);
    printf("Subtraction: %d - %d = %d\n", a, b, a - b);
    printf("Multiplication: %d * %d = %d\n", a, b, a * b);

    if (b != 0) {
        printf("Division: %d / %d = %d\n", a, b, a / b);
        printf("Remainder: %d %% %d = %d\n", a, b, a % b);
    } else {
        printf("Division and Remainder: Cannot divide by zero\n");
    }
    printf("\n--- Bitwise Operations ---\n");
    printf("a & b = %d\n", a & b);   // AND
    printf("a | b = %d\n", a | b);   // OR
    printf("a ^ b = %d\n", a ^ b);   // XOR
    printf("a << 1 = %d\n", a << 1); // Left shift
    printf("a >> 1 = %d\n", a >> 1); // Right shift
    printf("~a = %d\n", ~a);         // NOT of a
    printf("~b = %d\n", ~b);         // NOT of b

    return 0;
}
```
# Output:

<img width="535" height="558" alt="image" src="https://github.com/user-attachments/assets/5e2fb24f-9a99-4d70-971d-3a5f8f37707e" />

# Result: 
Thus, the program was implemented and executed successfully, and the required output was obtained.


# 19AI304-Fundamentals-of-C-Programming-2025-Odd
# IAPR-1- Module 1 - FoC
# Ex.No:5
  Develop a C program to check whether a given character is a vowel, consonant, digit, or special symbol using the ternary operator.
# Date : 21.11.2025 
# Aim:
  To develop and implement a C program that classifies a character as a vowel, consonant, digit, or special symbol using the ternary operator.
# Algorithm:
### Step 1:
  Start
### Step 2: 
  Include the standard input-output library: #include<stdio.h>.
### Step 3: 
  Input a character ch from the user.
### Step 4: 
   Check if ch is a digit ('0' to '9').
   
   If true → Print "Digit" → Go to Step 8.
   
   If false → Go to Step 5.
   
### Step 5:    
   Check if ch is an alphabet letter ('A' - 'Z' or 'a' – 'z').
   
   If true → Go to Step 6.
   
   If false → Go to Step 7.
   
### Step 6: 
   Check if ch is a vowel (a, e, i, o, u or A, E, I, O, U).
   
   If true → Print "Vowel" → Go to Step 8.
   
   If false → Print "Consonant" → Go to Step 8.
   
### Step 7:   
   Print "Special Symbol".
### Step 8:   
  Stop
# Program:
```
#include <stdio.h>
int main() {
    char ch;
    printf("Enter a character: ");
    scanf("%c", &ch);
    ( (ch >= 'A' && ch <= 'Z') || (ch >= 'a' && ch <= 'z') ) ?
        ( (ch=='A'||ch=='E'||ch=='I'||ch=='O'||ch=='U'||
           ch=='a'||ch=='e'||ch=='i'||ch=='o'||ch=='u') ?
            printf("Vowel\n") :
            printf("Consonant\n")
        )
    :
    ( (ch >= '0' && ch <= '9') ?
        printf("Digit\n") :
        printf("Special Symbol\n")
      );

    return 0;
}
```
# Output:

<img width="455" height="156" alt="image" src="https://github.com/user-attachments/assets/8722bf9b-93f8-44a9-b032-4ed835b71c9c" />

# Result: 
Thus, the program was implemented and executed successfully, and the required output was obtained.


