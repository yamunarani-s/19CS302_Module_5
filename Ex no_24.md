# EX 24 Create a structure program to read(empno,dept and basic pay) and store the data of 3 employees and calculate their Gross Salary(da =10% and HRA=30% from BP).
## DATE:19/05/25
## AIM:
To Create a structure program to read(empno,dept and basic pay) and store the data of 3 employees and calculate their Gross Salary(da =10% and HRA=30% from BP).

## Algorithm
1. Analyze the question
2. Follow the algorithm
3. Try the code
4.  Check for error
5. Run & Display the output
## Program:
```
/*
A structure program to read(empno,dept and basic pay) and store the data of 3 employees and calculate their Gross Salary(da =10% and HRA=30% from BP).
Developed by: 
RegisterNumber:  
*/
```
#include <stdio.h>

struct Employee {
    int empno;
    char dept[20];
    float basic_pay;
    float da;
    float hra;
    float gross_salary;
};

int main() {
    struct Employee emp[3];
    int i;

    // Input details
    for (i = 0; i < 3; i++) {
  
        scanf("%d", &emp[i].empno);
        scanf("%s", emp[i].dept);
        scanf("%f", &emp[i].basic_pay);

        // Calculate DA (10%) and HRA (30%)
        emp[i].da = 0.10 * emp[i].basic_pay;
        emp[i].hra = 0.30 * emp[i].basic_pay;
        emp[i].gross_salary = emp[i].basic_pay + emp[i].da + emp[i].hra;
    }

    // Display details
    printf("\nEmployee Details with Gross Salary:\n");
    for (i = 0; i < 3; i++) {
        printf("\nEmployee %d\n", i + 1);
        printf("Emp No        : %d\n", emp[i].empno);
        printf("Department    : %s\n", emp[i].dept);
        printf("Basic Pay     : %.2f\n", emp[i].basic_pay);
        printf("DA (10%%)      : %.2f\n", emp[i].da);
        printf("HRA (30%%)     : %.2f\n", emp[i].hra);
        printf("Gross Salary  : %.2f\n", emp[i].gross_salary);
    }

    return 0;
}

## Output:

Employee Details with Gross Salary:

Employee 1
Emp No        : 101
Department    : HR
Basic Pay     : 30000.00
DA (10%)      : 3000.00
HRA (30%)     : 9000.00
Gross Salary  : 42000.00

Employee 2
Emp No        : 102
Department    : IT
Basic Pay     : 40000.00
DA (10%)      : 4000.00
HRA (30%)     : 12000.00
Gross Salary  : 56000.00

Employee 3
Emp No        : 103
Department    : Sales
Basic Pay     : 35000.00
DA (10%)      : 3500.00
HRA (30%)     : 10500.00
Gross Salary  : 49000.00


## Result:
Thus the program was executed and the output was verified successfully.
