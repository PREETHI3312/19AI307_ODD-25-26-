# Ex.No:2(E) ACCESS MODIFIERS

## QUESTION:
```
Create a class Calculator with:

One non-static method add(int a, int b) that returns the sum
One static method info() that says "Calculator is ready"
```


## AIM:
```
To write a Java program demonstrating static and non-static methods using a Calculator class.
```


## ALGORITHM :
```
1.Start the program
2.Create a class Calculator
3.Define a static method info() to display a message
4.Define a non-static method add(int a, int b) to return sum
5.In main, call static method using class name
6.Create object to call non-static method
7.Display result
8.Stop program
```





## PROGRAM:
 ```
/*
Program to implement a Access Modifiers using Java
Developed by: PREETHI A K
RegisterNumber:  212223230156
*/
```

## SOURCE CODE:
```
import java.util.Scanner;

class Calculator {

    // Non-static method
    int add(int a, int b) {
        return a + b;
    }

    // Static method
    static void info() {
        System.out.println("Calculator is ready");
    }
}

class prog {
    public static void main(String[] args) {
        Scanner sc = new Scanner(System.in);

        int a = sc.nextInt();
        int b = sc.nextInt();

        Calculator.info();  // call static method

        Calculator obj = new Calculator();
        int sum = obj.add(a, b);  // call non-static method

        System.out.println("Sum: " + sum);

        sc.close();
    }
}
```






## OUTPUT:
<img width="615" height="309" alt="image" src="https://github.com/user-attachments/assets/327962a5-63c7-4fa6-91ee-1e6cd817bce4" />




## RESULT:
```
Thus, a Java program was successfully implemented to demonstrate static and non-static methods using a Calculator class.
```
