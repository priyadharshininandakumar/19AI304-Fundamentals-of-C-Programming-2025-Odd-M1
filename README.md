# 19AI304-Fundamentals-of-C-Programming-2025-Odd-M1
# IAPR-1- Module 1 - FoC
## 1. Implementation of basic C programs using Literals,Consonants, Variables, Data types.
## 2. Implementation of different categories of operators.
# Ex.No:1
  Build a C program to demonstrate the usage of different types of literals: integer, float, character, and string.  
# Date : 29/01/2026
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
    int age = 17; 
    printf("Integer literal: %d\n", age);    
    float height = 5.6; 
    printf("Float literal: %.1f\n", height); 
    char grade = 'A'; 
    printf("Character literal: %c\n", grade);  
    char name[] = "Priya"; 
    printf("String literal: %s\n", name);
    return 0;
}
```
# Output:
<img width="839" height="543" alt="Screenshot 2026-03-24 214807" src="https://github.com/user-attachments/assets/281f4bca-f38a-408a-abe7-c7af52bd368d" />
# Result: 
Thus, the program was implemented and executed successfully, and the required output was obtained.


# 19AI304-Fundamentals-of-C-Programming-2025-Odd
# IAPR-1- Module 1 - FoC
# Ex.No:2  29/01/2026
  Build a C program to display the value of a macro constant and a constant variable.
# Date : 
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
    const int DAYS_IN_WEEK = 7; 
    printf("Value of macro constant PI: %.5f\n", PI);
    printf("Value of constant variable DAYS_IN_WEEK: %d\n", DAYS_IN_WEEK);
    return 0;
}
```
# Output:
<img width="572" height="472" alt="Screenshot 2026-03-24 221955" src="https://github.com/user-attachments/assets/bffdccbe-4fc6-44d1-8a56-dab89e5b0576" />


# Result: 
Thus, the program was implemented and executed successfully, and the required output was obtained.


# 19AI304-Fundamentals-of-C-Programming-2025-Odd
# IAPR-1- Module 1 - FoC
# Ex.No:3  29/01/2026
  Build a C program to demonstrate the use of different data types such as int, float, double, and char, and display their values using printf().
# Date : 
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
    int age = 17;
    float height = 5.6f;      
    double weight = 55.75; 
    char grade = 'A';
    printf("Integer value (int): %d\n", age);
    printf("Floating point value (float): %.2f\n", height);
    printf("Double precision value (double): %.2lf\n", weight);
    printf("Character value (char): %c\n", grade);
    return 0;
}
```
# Output:
<img width="744" height="666" alt="Screenshot 2026-03-24 215752" src="https://github.com/user-attachments/assets/c2d5ec84-5859-459d-8a6b-34e409216833" />

# Result: 

# 19AI304-Fundamentals-of-C-Programming-2025-Odd
# IAPR-1- Module 1 - FoC
# Ex.No:4
  Build a C program to perform arithmetic and bitwise operations on two integers entered by the user. The program should display: Arithmetic operations: addition, subtraction, multiplication, division, and remainder. Bitwise operations: AND, OR, XOR, left shift, right shift, and NOT.
# Date :  29/01/2026
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
    int num1, num2;
    printf("Enter the first integer: ");
    scanf("%d", &num1);
    printf("Enter the second integer: ");
    scanf("%d", &num2);
    printf("\n--- Arithmetic Operations ---\n");
    printf("Addition: %d + %d = %d\n", num1, num2, num1 + num2);
    printf("Subtraction: %d - %d = %d\n", num1, num2, num1 - num2);
    printf("Multiplication: %d * %d = %d\n", num1, num2, num1 * num2);
    if(num2 != 0) {
        printf("Division: %d / %d = %d\n", num1, num2, num1 / num2);
        printf("Remainder: %d %% %d = %d\n", num1, num2, num1 % num2);
    } else {
        printf("Division and remainder: Cannot divide by zero!\n");
    }
    printf("\n--- Bitwise Operations ---\n");
    printf("Bitwise AND: %d & %d = %d\n", num1, num2, num1 & num2);
    printf("Bitwise OR: %d | %d = %d\n", num1, num2, num1 | num2);
    printf("Bitwise XOR: %d ^ %d = %d\n", num1, num2, num1 ^ num2);
    printf("Left shift num1 by 1: %d << 1 = %d\n", num1, num1 << 1);
    printf("Right shift num1 by 1: %d >> 1 = %d\n", num1, num1 >> 1);
    printf("Bitwise NOT of num1: ~%d = %d\n", num1, ~num1);
    return 0;
}
```
# Output:
<img width="577" height="714" alt="Screenshot 2026-03-24 220421" src="https://github.com/user-attachments/assets/5da57604-0273-49b6-90e3-49ecd9c5275e" />

# Result: 
Thus, the program was implemented and executed successfully, and the required output was obtained.


# 19AI304-Fundamentals-of-C-Programming-2025-Odd
# IAPR-1- Module 1 - FoC
# Ex.No:5  29/01/2026
  Develop a C program to check whether a given character is a vowel, consonant, digit, or special symbol using the ternary operator.
# Date : 
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
    ( (ch >= '0' && ch <= '9') ? printf("'%c' is a Digit\n", ch) :
      (ch == 'A' || ch == 'E' || ch == 'I' || ch == 'O' || ch == 'U' ||
       ch == 'a' || ch == 'e' || ch == 'i' || ch == 'o' || ch == 'u') ?
       printf("'%c' is a Vowel\n", ch) :
      ( (ch >= 'A' && ch <= 'Z') || (ch >= 'a' && ch <= 'z') ) ?
       printf("'%c' is a Consonant\n", ch) :
       printf("'%c' is a Special Symbol\n", ch)
    );
    return 0;
}
```
# Output:
<img width="662" height="517" alt="Screenshot 2026-03-24 221656" src="https://github.com/user-attachments/assets/fe8ffb6d-00d7-4bf7-adc1-73301bfc19f3" />

# Result: 
Thus, the program was implemented and executed successfully, and the required output was obtained.


