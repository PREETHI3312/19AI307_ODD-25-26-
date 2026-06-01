# Ex.No:2(A) CLASS AND OBJECT

## QUESTION:
```
Create a class Student with attributes name, rollNumber, marks. Create 3 student objects and print their details.
```

## AIM:
```
To write a Java program using class and objects to store and display details of students.
```

## ALGORITHM :
```
1.Start the program
2.Create a class Student with attributes name, rollNumber, and marks
3.Create objects of the Student class
4.Assign values to each object
5.Display the details of each student
6.Stop the program
```





## PROGRAM:
 ```
/*
Program to implement a Class and Objects using Java
Developed by: PREETHI A K
RegisterNumber:  212223230156
*/
```

## SOURCE CODE:
```
import java.util.Scanner;

class Student {
    String name;
    int rollNumber;
    int marks;
}

public class Main {
    public static void main(String[] args) {
        Scanner sc = new Scanner(System.in);

        Student s1 = new Student();
        s1.name = sc.next();
        s1.rollNumber = sc.nextInt();
        s1.marks = sc.nextInt();

        Student s2 = new Student();
        s2.name = sc.next();
        s2.rollNumber = sc.nextInt();
        s2.marks = sc.nextInt();

        Student s3 = new Student();
        s3.name = sc.next();
        s3.rollNumber = sc.nextInt();
        s3.marks = sc.nextInt();

        System.out.println(s1.name + " | " + s1.rollNumber + " | " + s1.marks);
        System.out.println(s2.name + " | " + s2.rollNumber + " | " + s2.marks);
        System.out.println(s3.name + " | " + s3.rollNumber + " | " + s3.marks);

        sc.close();
    }
}
```






## OUTPUT:
<img width="664" height="291" alt="image" src="https://github.com/user-attachments/assets/c77ac3de-6fd4-4867-a547-16c345f3890b" />




## RESULT:
```
Thus, a Java program was successfully implemented using class and objects to create and display details of three students.
```
