# EX-16-LEFT-SHIFT-OPERATION
## AIM
To write a C Program to perform the basic left shift operation for 44 integer number with 3 shifts.

## ALGORITHM
1.	Start the program.
2.	Assign values of a and b as 44 and 3.
3.	Use left shift operator (<<) and shift the value of a three times.
4.	Display the result.
5.	Stop the program.

## PROGRAM
```c
#include <stdio.h>

int main() {
    int a = 44, b = 3;
    int result = a << b;
    printf("Result after left shifting %d by %d positions = %d\n", a, b, result);
    return 0;
}

```
## OUTPUT

![image](https://github.com/user-attachments/assets/1b940866-5b50-4b1a-9719-50d28d129861)









## RESULT
Thus the program to perform the basic left shift operation for 44 integer number with 3 shifts has been executed successfully.




 
 


# EX-17-TWO-NUMBERS-ARE-EQUAL-OR-NOT


## AIM

Write a C Program to check whether the two numbers are equal or not using simple if statement.

## ALGORITHM

1.	Start the program.
2.	Read two numbers.
3.	If first number is equal to second number, display both are equal.
4.	Otherwise display both are not equal.
5.	Stop the program.

## PROGRAM
```c
#include <stdio.h>

int main() {
    int num1, num2;

    printf("Enter first number: ");
    scanf("%d", &num1);

    printf("Enter second number: ");
    scanf("%d", &num2);

    if(num1 == num2) {
        printf("Both numbers are equal.\n");
    }
    else {
        printf("Both numbers are not equal.\n");
    }

    return 0;
}

```

## OUTPUT

![image](https://github.com/user-attachments/assets/e7e6fcc0-ef33-4589-a5ac-f9b1802ca64b)
           
## RESULT

Thus the program to check whether the two numbers are equal or not using simple if statement has been executed successfully
 
 


# EX-18-STRING-LOWERCASE-CONVERSION
## AIM
Write a C Program to convert the given string into lowercase.

## ALGORITHM
1.	Start the program.
2.	Read a string variable.
3.	Using tolower( ) function convert the given string into its lowercase.
4.	Display the result.
5.	Stop the program.

## PROGRAM
```c
#include <stdio.h>
#include <ctype.h>

int main() {
    char str[100];
    int i = 0;

    printf("Enter a string: ");
    scanf("%s", str);

    while(str[i] != '\0') {
        str[i] = tolower(str[i]);
        i++;
    }

    printf("String in lowercase: %s\n", str);

    return 0;
}

```
## OUTPUT

![image](https://github.com/user-attachments/assets/3aa844b9-163e-43d6-b99e-518fd391971b)



## RESULT
Thus the program to convert the given string into lowercase has been executed successfully
 
 


# EX-19-COUNT-OF-WORDS-IN-A-STRING
## AIM
Write a C Program to count the total number of words in a given string using do While loop.

## ALGORITHM
1.	Start the program.
2.	Read a string variable.
3.	Using for loop, inspect the string character by character.
4.	Whenever a space is encountered increment count by 1.
5.	Display the result.
6.	Stop the program.

## PROGRAM
```c
#include <stdio.h>

int main() {
    char str[100];
    int count = 1, i = 0;

    printf("Enter a string: ");
    fgets(str, sizeof(str), stdin);

    do {
        if (str[i] == ' ') {
            count++;
        }
        i++;
    } while (str[i] != '\0');

    printf("Total number of words: %d\n", count);

    return 0;
}

```
## OUTPUT

![image](https://github.com/user-attachments/assets/60ab79b1-51fc-4166-9446-5060cf0598e4)




## RESULT
Thus the program to count the total number of words in a given string using do While loop has been executed successfully
 
 


# EX  -20 -COMPARING TWO STRINGS
## AIM
write a Program to compare two strings without using strcmp().
## ALGORITHM
1. Start the program.
2. Declare two character arrays c1 and c2 of size 100 to store the strings. Also, declare an integer variableflag and initialize it to 0, and i for indexing.
3. Read the first string c1 using scanf("%[^\n]", c1); — this reads input until a newline is encountered (i.e., can include spaces).
4. Read the second string c2 using scanf("%s", c2); — this reads input until a space or newline (i.e., no spaces in the second string).
5. Start comparing characters of both strings from index i = 0.
6. Repeat the following while neither c1[i] nor c2[i] is '\0' (i.e., end of string):
•	If c1[i] is not equal to c2[i], set flag = 1.
•	Increment i by 1.
7. After the loop, check the value of flag:
•	If flag == 0, print "strings are same".
•	Otherwise, print "strings are not same".
8. End the program.

## PROGRAM
```c
#include <stdio.h>

int main() {
    char c1[100], c2[100];
    int i = 0, flag = 0;

    printf("Enter the first string: ");
    scanf("%[^\n]", c1);

    getchar(); // to consume the newline character left by scanf

    printf("Enter the second string: ");
    scanf("%s", c2);

    while (c1[i] != '\0' && c2[i] != '\0') {
        if (c1[i] != c2[i]) {
            flag = 1;
            break;
        }
        i++;
    }

    if (c1[i] != '\0' || c2[i] != '\0') {
        flag = 1; // If one string ends before the other
    }

    if (flag == 0) {
        printf("Strings are same.\n");
    } else {
        printf("Strings are not same.\n");
    }

    return 0;
}
```

## OUTPUT

![image](https://github.com/user-attachments/assets/66f3c2c5-f432-4b3d-a5f2-6ece213697e6)

## RESULT
Thus the C Program to compare two strings without using strcmp() has been executed successfully.

