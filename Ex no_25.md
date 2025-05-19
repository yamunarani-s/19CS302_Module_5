# EX 25 C program to check whether a given character is a vowel or consonant using pointer
## DATE:19/05/25
## AIM:
To write a C program to check whether a given character is a vowel or consonant using pointer

## Algorithm
1. Analyze the question
2. Follow the algorithm
3. Try the code
4.  Check for error
5. Run & Display the output
## Program:
```
/*
C program to check whether a given character is a vowel or consonant using pointer
Developed by: 
RegisterNumber:  
*/
```
#include <stdio.h>

int main() {
    char ch;
    char *ptr = &ch;
    scanf(" %c", ptr);  // space before %c to consume any leftover newline

    // Convert to lowercase for easy comparison
    if ((*ptr >= 'A') && (*ptr <= 'Z')) {
        *ptr = *ptr + 32;
    }

    if (*ptr == 'a' || *ptr == 'e' || *ptr == 'i' || *ptr == 'o' || *ptr == 'u') {
        printf("The character '%c' is a vowel.\n", *ptr);
    } else if ((*ptr >= 'a' && *ptr <= 'z')) {
        printf("The character '%c' is a consonant.\n", *ptr);
    } else {
        printf("'%c' is not an alphabet.\n", *ptr);
    }

    return 0;
}
## Output:
The character 'e' is a vowel.

## Result:
Thus the program was executed and the output was verified successfully.
