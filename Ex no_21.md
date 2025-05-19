# EX 21 C program to calculate the area of a triangle using pointer.
## DATE: 19/05/25
## AIM:
To write a C program to calculate the area of a triangle using pointer.

## Algorithm
1. Analyze the question
2. Follow the algorithm
3. Try the code
4.  Check for error
5. Run & Display the output

## Program:
```
/*
C program to calculate the area of a triangle using pointer.
Developed by: 
RegisterNumber:  
*/
```
/* C program to calculate the area of a triangle using pointers
   Developed by: Your Name
   RegisterNumber: Your Register Number
*/

#include <stdio.h>

int main() {
    float base, height, area;
    float *pBase = &base;
    float *pHeight = &height;
    float *pArea = &area;
    scanf("%f", pBase);
    scanf("%f", pHeight);

    *pArea = 0.5 * (*pBase) * (*pHeight);

    printf("Area of the triangle = %.2f\n", *pArea);

    return 0;
}

## Output:

Area of the triangle = 25.00

## Result:
Thus the program was executed and the output was verified successfully.
