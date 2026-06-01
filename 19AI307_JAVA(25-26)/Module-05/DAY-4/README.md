# Ex.No:5(D) THREAD PRIORITY

## QUESTION:
```
Write a Java program to set the priority and name of two threads (t1 and t2). Read thread names from the user.
```

## AIM:
```
To write a Java program to create two threads, set their names and priorities, and display their details.
```
## ALGORITHM :
```
1.Start the program
2.Import java.util.Scanner package
3.Read thread names from user
4.Create two Thread objects (t1 and t2)
5.Set name and priority for both threads
6.Set priority: t1 = 4, t2 = 2
7.Display thread details using toString()
8.Stop program
```




## PROGRAM:
 ```
/*
Program to implement a Thread Priority Concept using Java
Developed by: PREETHI A K
RegisterNumber:  212223230156
*/
```

## SOURCE CODE:
```
import java.util.Scanner;

public class Main {
    public static void main(String[] args) {
        Scanner sc = new Scanner(System.in);

        String name1 = sc.nextLine();
        String name2 = sc.nextLine();

        Thread t1 = new Thread();
        Thread t2 = new Thread();

        t1.setName(name1);
        t2.setName(name2);

        t1.setPriority(4);
        t2.setPriority(2);

        System.out.println(t1);
        System.out.println(t2);

        sc.close();
    }
}

```




## OUTPUT:
<img width="811" height="247" alt="image" src="https://github.com/user-attachments/assets/fce00057-930d-4737-b2e3-679c673b1f3f" />



## RESULT:
```
Thus, a Java program was successfully implemented to set thread names and priorities and display their details.
```
