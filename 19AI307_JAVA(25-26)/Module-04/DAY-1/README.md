# Ex.No:4(A) EXCEPTION HANDLING

## QUESTION:
```
Write a program that reads two integers and divides the first by the second. Handle the case when division by zero occurs.
```
## AIM:
```
To write a Java program using exception handling to perform division of two integers and handle ArithmeticException when division by zero occurs.
```
## ALGORITHM :
```
1.Start the program
2.Import java.util.Scanner package
3.Read two integer inputs from the user
4.Use try block to perform division
5.Catch ArithmeticException if denominator is zero
6.Display appropriate message
7.Stop the program


```


## PROGRAM:
 ```
/*
Program to implement a Exception Handling using Java
Developed by: PREETHI A K
RegisterNumber:  212223230156
*/
```

## SOURCE CODE:
```
import java.util.Scanner;

public class DivisionProgram {
    public static void main(String[] args) {
        Scanner scanner = new Scanner(System.in);

        int num1 = scanner.nextInt();

        int num2 = scanner.nextInt();

        try {
            int result = num1 / num2;
            System.out.println("Result: " + result);
        } catch (ArithmeticException e) {
            System.out.println("Error: Division by zero");
        }

        scanner.close();
    }
}

```



## OUTPUT:
<img width="769" height="308" alt="image" src="https://github.com/user-attachments/assets/a4ba20c2-5abf-4a91-82c8-fe9802f07c59" />



## RESULT:
```
Thus, a Java program was successfully implemented using exception handling to manage division by zero errors using try-catch block.
```
