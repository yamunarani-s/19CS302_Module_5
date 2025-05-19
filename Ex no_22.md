# EX 22 C program to count total number of even elements in an array using calloc().
## DATE:19/05/25
## AIM:
To write a C program to count total number of even elements in an array using calloc().

## Algorithm
1. Analyze the question
2. Follow the algorithm
3. Try the code
4.  Check for error
5. Run & Display the output
## Program:
```
/*
C program to count total number of even elements in an array using calloc().
Developed by: 
RegisterNumber:  
*/
```
/* C program to count total number of even elements in an array using calloc()
   Developed by: Your Name
   Register Number: Your Register Number
*/

#include <stdio.h>
#include <stdlib.h>

int main() {
    int *arr, n, i, evenCount = 0;
    scanf("%d", &n);
    arr = (int *)calloc(n, sizeof(int));

    if (arr == NULL) {
        printf("Memory allocation failed.\n");
        return 1;
    }
    for (i = 0; i < n; i++) {
        scanf("%d", &arr[i]);
    }

    // Count even numbers
    for (i = 0; i < n; i++) {
        if (arr[i] % 2 == 0) {
            evenCount++;
        }
    }

    printf("Total number of even elements: %d\n", evenCount);

    // Free allocated memory
    free(arr);

    return 0;
}


## Output:

10 15 20 33 42 55
Total number of even elements: 3

## Result:
Thus the program was executed and the output was verified successfully.
