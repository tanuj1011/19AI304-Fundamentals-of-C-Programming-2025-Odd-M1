# 19AI304-Fundamentals-of-C-Programming-2025-Odd-M1
# IAPR-1- Module 1 - FoC
## 1. Implementation of basic C programs using Literals,Consonants, Variables, Data types.
## 2. Implementation of different categories of operators.
# Ex.No:1
  Build a C program to demonstrate the usage of different types of literals: integer, float, character, and string.  
# Date : 21/11/2025
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
    printf("Integer literal: %d, Size = %zu bytes\n", 10, sizeof(10));
    printf("Float literal: %f, Size = %zu bytes\n", 3.14f, sizeof(3.14f));
    printf("Character literal: %c, Size = %zu bytes\n", 'A', sizeof('A'));
    printf("String literal: %s, Size = %zu bytes\n", "Hello C", sizeof("Hello C"));

    return 0;
}
```
# Output:
<img width="527" height="302" alt="image" src="https://github.com/user-attachments/assets/b604fbc4-78f4-4a72-bc0c-a413e7c7e134" />

# Result: 
Thus, the program was implemented and executed successfully, and the required output was obtained.


# 19AI304-Fundamentals-of-C-Programming-2025-Odd
# IAPR-1- Module 1 - FoC
# Ex.No:2
  Build a C program to display the value of a macro constant and a constant variable.
# Date : 21/11/2025
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

#define PI 3.14159  

int main() {
    const int DAYS = 7;  

    printf("Value of macro constant PI: %f\n", PI);
    printf("Value of constant variable DAYS: %d\n", DAYS);

    return 0;
}
```
# Output:
<img width="517" height="277" alt="image" src="https://github.com/user-attachments/assets/7f754609-f149-4835-b013-2a85dc250891" />

# Result: 
Thus, the program was implemented and executed successfully, and the required output was obtained.


# 19AI304-Fundamentals-of-C-Programming-2025-Odd
# IAPR-1- Module 1 - FoC
# Ex.No:3
  Build a C program to demonstrate the use of different data types such as int, float, double, and char, and display their values using printf().
# Date : 21/11/2025
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
    int age = 20;
    float height = 5.8f;
    double distance = 12345.6789;
    char grade = 'A';

    printf("Integer value (age): %d\n", age);
    printf("Float value (height): %f\n", height);
    printf("Double value (distance): %lf\n", distance);
    printf("Character value (grade): %c\n", grade);

    return 0;
}
```
# Output:
<img width="542" height="321" alt="image" src="https://github.com/user-attachments/assets/bfcb88a7-ad73-451b-a3ec-f2912bc8b7bc" />

# Result: 
Thus, the program was implemented and executed successfully, and the required output was obtained.


# 19AI304-Fundamentals-of-C-Programming-2025-Odd
# IAPR-1- Module 1 - FoC
# Ex.No:4
  Build a C program to perform arithmetic and bitwise operations on two integers entered by the user. The program should display: Arithmetic operations: addition, subtraction, multiplication, division, and remainder. Bitwise operations: AND, OR, XOR, left shift, right shift, and NOT.
# Date : 21/11/2025
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
    printf("Sum (a + b): %d\n", a + b);
    printf("Difference (a - b): %d\n", a - b);
    printf("Product (a * b): %d\n", a * b);
    printf("Quotient (a / b): %d\n", a / b);
    printf("Remainder (a %% b): %d\n", a % b);

    printf("\n--- Bitwise Operations ---\n");
    printf("AND (a & b): %d\n", a & b);
    printf("OR (a | b): %d\n", a | b);
    printf("XOR (a ^ b): %d\n", a ^ b);
    printf("Left shift (a << b): %d\n", a << b);
    printf("Right shift (a >> b): %d\n", a >> b);
    printf("Bitwise NOT of a (~a): %d\n", ~a);
    printf("Bitwise NOT of b (~b): %d\n", ~b);

    return 0;
}
```
# Output:
<img width="635" height="542" alt="image" src="https://github.com/user-attachments/assets/3e39f116-0013-4722-b47d-072dadb5d754" />

# Result: 
Thus, the program was implemented and executed successfully, and the required output was obtained.


# 19AI304-Fundamentals-of-C-Programming-2025-Odd
# IAPR-1- Module 1 - FoC
# Ex.No:5
  Develop a C program to check whether a given character is a vowel, consonant, digit, or special symbol using the ternary operator.
# Date : 21/11/2025
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

    (ch >= '0' && ch <= '9') ? printf("Digit\n") :
    ((ch >= 'A' && ch <= 'Z') || (ch >= 'a' && ch <= 'z')) ?
        ((ch=='a'||ch=='e'||ch=='i'||ch=='o'||ch=='u'||
          ch=='A'||ch=='E'||ch=='I'||ch=='O'||ch=='U')
            ? printf("Vowel\n")
            : printf("Consonant\n"))
        : printf("Special Symbol\n");

    return 0;
}
```
# Output:
<img width="563" height="305" alt="image" src="https://github.com/user-attachments/assets/0fe07465-8174-4520-b284-72a20e7c8a73" />

# Result: 
Thus, the program was implemented and executed successfully, and the required output was obtained.


