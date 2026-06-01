# Ex.No:1(E) STRINGS AND MATH FUNCTION

## QUESTION:
Write a Java program to calculate the power of a given number.

## AIM:
To write a Java program to calculate the power of a number using the Math function.

## ALGORITHM :
Start the program
Import java.util.Scanner package
Read base number from user
Read exponent from user
Use Math.pow() function to calculate power
Display the result
Stop the program	





## PROGRAM:
 ```

Program to implement a Strings and Math Function using Java
Developed by: PREETHI A K
RegisterNumber: 212223230156 

```

## SOURCE CODE:
```
import java.util.Scanner;

public class PowerCalculator {
    public static void main(String[] args) {
        Scanner sc = new Scanner(System.in);

        double base = sc.nextDouble();
        double exponent = sc.nextDouble();

        double result = Math.pow(base, exponent);

        System.out.println(base + " raised to the power of " + exponent + " is: " + result);

        sc.close();
    }
}
```







## OUTPUT:
<img width="968" height="239" alt="image" src="https://github.com/user-attachments/assets/a9800b62-0c2f-4286-8aa4-8e2323c9359a" />




## RESULT:
```
Thus, a Java program was successfully implemented to calculate the power of a given number using the Math function Math.pow().
```
