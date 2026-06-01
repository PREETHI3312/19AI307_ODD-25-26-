# Ex.No:2(D) VARIABLE SCOPE AND CONSTRUCTOR

## QUESTION:
```
Write a program to access a static variable using both class name and object.
```

## AIM:
```
To write a Java program demonstrating variable scope using a static variable and accessing it using both class name and object.
```

## ALGORITHM :
```
1.Start the program
Create a class with a static variable
Read input value from user
Assign value to static variable
Access static variable using class name
Access static variable using object reference
Display both outputs
Stop program
```




## PROGRAM:
 ```
/*
Program to implement a Variable scope and Constructor using Java
Developed by: PREETHI A K
RegisterNumber:  212223230156
*/
```

## SOURCE CODE:
```
import java.util.Scanner;

class prog {
    static int num;  // static variable

    public static void main(String[] args) {
        Scanner sc = new Scanner(System.in);

        num = sc.nextInt();  // input

        // Access using class name
        System.out.println("Accessing using class name: " + prog.num);

        // Access using object
        prog obj = new prog();
        System.out.println("Accessing using object: " + obj.num);

        sc.close();
    }
}
```






## OUTPUT:
<img width="758" height="314" alt="image" src="https://github.com/user-attachments/assets/1f7d006c-1385-43cc-b418-1dd093a94586" />



## RESULT:
```
Thus, a Java program was successfully implemented to demonstrate static variable access using both class name and object reference.
```
