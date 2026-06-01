# Ex.No:5(C)  FILE HANDLING USING JAVA
## QUESTION:
```
Write a Java program to create a new file named example.txt.
```
## AIM:
```
To write a Java program to create a file using File Handling concepts in Java.
```
## ALGORITHM :
```
1.Start the program
2.Import required java.io package
3.Create a File object with file name example.txt
4.Use createNewFile() method
5.Check whether file is created successfully
6.Display result message
7.Stop program

```



## PROGRAM:
 ```
/*
Program to implement a File Handling using Java
Developed by: PREETHI A K
RegisterNumber:  212223230156
*/
```

## SOURCE CODE:
```
import java.io.File;
import java.io.IOException;

public class Main {
    public static void main(String[] args) {
        try {
            File file = new File("example.txt");

            if (file.createNewFile()) {
                System.out.println("File created: example.txt");
            } else {
                System.out.println("File already exists.");
            }
        } catch (IOException e) {
            System.out.println("An error occurred.");
        }
    }
}

```




## OUTPUT:
<img width="703" height="165" alt="image" src="https://github.com/user-attachments/assets/16085e4a-d38d-4d64-be99-677079d602d5" />




## RESULT:
```
Thus, a Java program was successfully implemented to create a new file using File Handling concepts.
```
