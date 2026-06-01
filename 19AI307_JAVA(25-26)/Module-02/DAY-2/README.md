# Ex.No:2(B) METHODS

## QUESTION:
```
Create a method printName(String name) that gets input from the user for the string and prints "Hello, " followed by the name passed.
```

## AIM:
```
To write a Java program using a method that takes a string parameter and prints a greeting message.

```
## ALGORITHM :
```
1.Start the program
2.Import java.util.Scanner package
3.Create a method printName(String name)
4.Inside the method, print "Hello, " + name
5.In main method, read user input
6.Call printName() method with input value
7.Stop the program
```





## PROGRAM:
 ```
/*
Program to implement a Methods using Java
Developed by: PREETHI A K
RegisterNumber:  212223230156
*/
```

## SOURCE CODE:
```
import java.util.Scanner;

public class Main {

    public static void printName(String name) {
        System.out.println("Hello, " + name);
    }

    public static void main(String[] args) {
        Scanner sc = new Scanner(System.in);
        String name = sc.nextLine();
        printName(name);
    }
}
```






## OUTPUT:

<img width="586" height="161" alt="image" src="https://github.com/user-attachments/assets/0a6d4a5a-1585-40e7-8f20-3d2cc4968678" />


## RESULT:
```
Thus, a Java program was successfully implemented using a method to accept a string input and display a greeting message.
```
