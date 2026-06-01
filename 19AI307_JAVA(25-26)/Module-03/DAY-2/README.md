# Ex.No:3(b) POLYMORPHISM

## QUESTION:
```
Write a Java program that calculates the area of different shapes using method overloading.
```

## AIM:
```
To write a Java program demonstrating polymorphism using method overloading to calculate the area of different shapes.
```

## ALGORITHM :
```
1.Start the program
2.Create a class AreaCalculator
3.Define method area(int side) for square
4.Define method area(int length, int breadth) for rectangle
5.Define method area(double radius) for circle
6.Create object of class in main method
7.Call methods based on input
8.Display results
9.Stop program
```





## PROGRAM:
 ```
/*
Program to implement a Polymorphism using Java
Developed by: PREETHI A K
RegisterNumber: 212223230156 
*/
```

## SOURCE CODE:
```
import java.util.*;
class AreaCalculator
{
    int area(int side)
    {
        return side*side;
    }
    
    int area(int length,int breadth)
    {
        return length*breadth;
    }
    double area(double radius)
    {
        return  Math.PI*radius*radius;
    }
}
public class Main
{
    public static void main(String[] args)
    {
        Scanner sc=new Scanner(System.in);
        int side=sc.nextInt();
        int length=sc.nextInt();
        int breadth=sc.nextInt();
        double radius=sc.nextDouble();
        
        AreaCalculator obj=new AreaCalculator();
        System.out.println("Area of square: "+obj.area(side));
        System.out.println("Area of rectangle: "+obj.area(length,breadth));
        System.out.println("Area of circle: "+obj.area(radius));
    }
}
```






## OUTPUT:
<img width="829" height="378" alt="image" src="https://github.com/user-attachments/assets/973b39c4-ae46-4449-80fa-9b4ec85fcc18" />




## RESULT:
```
Thus, a Java program was successfully implemented to demonstrate polymorphism using method overloading for calculating the area of different shapes.
```
