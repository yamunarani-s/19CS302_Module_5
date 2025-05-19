# EX 23 C program to store and display the name, id, age and salary of an employee using structure(using array of structure).
## DATE:19/05/25
## AIM:
To write a C program to store and display the name, id, age and salary of an employee using structure(using array of structure).

## Algorithm
1. Analyze the question
2. Follow the algorithm
3. Try the code
4.  Check for error
5. Run & Display the output  

## Program:
```
/*
C program to store and display the name, id, age and salary of an employee using structure(using array of structure).
Developed by: 
RegisterNumber:  
*/
```
#include <stdio.h>

struct Employee {
    char name[50];
    int id;
    int age;
    float salary;
};

int main() {
    int n, i;
    scanf("%d", &n);

    struct Employee emp[n];  // Array of structures

    // Input employee details
    for (i = 0; i < n; i++) {
        printf("\nEnter details for Employee %d\n", i + 1);

        printf("Name: ");
        scanf(" %[^\n]", emp[i].name);  // Read string with spaces

        printf("ID: ");
        scanf("%d", &emp[i].id);

        printf("Age: ");
        scanf("%d", &emp[i].age);

        printf("Salary: ");
        scanf("%f", &emp[i].salary);
    }

    // Display employee details
    printf("\nEmployee Details:\n");
    for (i = 0; i < n; i++) {
        printf("\nEmployee %d\n", i + 1);
        printf("Name   : %s\n", emp[i].name);
        printf("ID     : %d\n", emp[i].id);
        printf("Age    : %d\n", emp[i].age);
        printf("Salary : %.2f\n", emp[i].salary);
    }

    return 0;
}


## Output:
Enter the number of employees: 2

Enter details for Employee 1
Name: John Doe
ID: 101
Age: 30
Salary: 55000

Enter details for Employee 2
Name: Jane Smith
ID: 102
Age: 28
Salary: 62000

Employee Details:

Employee 1
Name   : John Doe
ID     : 101
Age    : 30
Salary : 55000.00

Employee 2
Name   : Jane Smith
ID     : 102
Age    : 28
Salary : 62000.00


## Result:
Thus the program was executed and the output was verified successfully.
