# Ex.No:1(C) LOOPING STATEMENT

## QUESTION:
```
The Fibonacci series is a sequence of numbers in which each number is the sum of the two preceding ones. The series starts with 0 and 1. Write a Java program that asks the user to enter how many terms they want and display the Fibonacci series using a for loop.
```

## AIM:
```
To write a Java program to generate and display the Fibonacci series up to N terms using a for loop.
```

## ALGORITHM :
```
1.Start the program
2.Import java.util.Scanner package
3.Create Scanner object
4.Read number of terms (n) from user
5.Initialize first two terms: a = 0, b = 1
6.Print first n terms using a for loop
7.In each iteration, calculate next term = a + b
8.Update values of a and b
9.Stop program	
```




## PROGRAM:
 ```

Program to implement a Looping Statement using Java
Developed by: PREETHI A K
RegisterNumber:  212223230156

```

## SOURCE CODE:
```
import java.util.Scanner;

public class FibonacciSeries {
    public static void main(String[] args) {
        Scanner sc = new Scanner(System.in);

        int n = sc.nextInt();

        int a = 0, b = 1;

        System.out.print("Fibonacci Series: " + a + " " + b);

        for (int i = 3; i <= n; i++) {
            int next = a + b;
            System.out.print(" " + next);
            a = b;
            b = next;
        }

        sc.close();
    }
}
```






## OUTPUT:

<img width="785" height="247" alt="image" src="https://github.com/user-attachments/assets/b37dbeeb-bac2-48cc-afa8-26bcfd0ec83b" />





## RESULT:
```
Thus, a Java program was successfully implemented to generate and display the Fibonacci series up to N terms using a for loop.
```
