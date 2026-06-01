# Ex.No:5(A) INPUTSTREAMREADER 

## QUESTION:
```
Write a program to demonstrate chaining of streams using BufferedReader on top of InputStreamReader on top of System.in.
```
## AIM:
```
To write a Java program using InputStreamReader and BufferedReader to read input from the user using stream chaining.
```
## ALGORITHM :
```
1.Start the program
2.Import required I/O classes
3.Create InputStreamReader using System.in
4.Wrap it with BufferedReader
5.Read input using readLine()
6.Display the input
7.Stop program
```



## PROGRAM:
 ```
/*
Program to implement a InputStreamReader using Java
Developed by: PREETHI A K
RegisterNumber: 212223230156 
*/
```

## SOURCE CODE:
```
import java.io.BufferedReader;
import java.io.IOException;
import java.io.InputStreamReader;

public class ChainingStreamsExample {
    public static void main(String[] args) {
        // Chaining: System.in -> InputStreamReader -> BufferedReader
        BufferedReader br = new BufferedReader(new InputStreamReader(System.in));

        try {
            String name = br.readLine();
            int age = Integer.parseInt(br.readLine());

            System.out.println("--- User Details ---");
            System.out.println("Name: " + name);
            System.out.println("Age: " + age);
        } catch (IOException e) {
            System.out.println("Error reading input");
        }
    }
}

```




## OUTPUT:
<img width="681" height="451" alt="image" src="https://github.com/user-attachments/assets/80db9a84-6ab5-4190-ae16-e5914f49d14f" />



## RESULT:
```
Thus, a Java program was successfully implemented to demonstrate stream chaining using BufferedReader and InputStreamReader for input handling.
```
