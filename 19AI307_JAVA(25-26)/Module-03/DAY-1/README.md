# Ex.No:3(A) INHERITANCE AND AGGREGATION

## QUESTION:
```
Create a Super class Vehicle with fields brand (String) and speed (int). Create a subclass Car that inherits from Vehicle and adds a field fuelType (String).

Implement a method in Car called displayInfo() that prints the vehicle's brand, speed, and fuel typ
```
## AIM:
```
To write a Java program demonstrating inheritance by creating a superclass Vehicle and a subclass Car, and displaying vehicle details using a method.
```

## ALGORITHM :
```
1.Start the program
2.Create superclass Vehicle with variables brand and speed
3.Create subclass Car that extends Vehicle
4.Add fuelType variable in Car class
5.Create method displayInfo() in Car class
6.Read input values using Scanner
7.Create object of Car class
8.Assign values and display details
9.Stop program
```




## PROGRAM:
 ```
/*
Program to implement a Inheritance and Aggregation using Java
Developed by: PREETHI A K
RegisterNumber: 212223230156 
*/
```

## SOURCE CODE:
```
import java.util.*;
class Vehicle
{
    String brand;
    int speed;
}
class Car extends Vehicle
{
    String fuelType;
    
    void displayInfo()
    {
        System.out.println("Brand: "+brand);
        System.out.println("Speed: "+speed+" km/h");
        System.out.println("Fuel Type: "+fuelType);
    }
}
public class Main
{
    public static void main(String[] args)
    {
        Scanner sc=new Scanner(System.in);
        Car c=new Car();
        c.brand=sc.next();
        c.speed=sc.nextInt();
        c.fuelType=sc.next();
        c.displayInfo();
        
    }
}
```






## OUTPUT:
<img width="747" height="393" alt="image" src="https://github.com/user-attachments/assets/de008c7a-56f3-4674-af8a-0f2c99d14c1e" />




## RESULT:
```
Thus, a Java program was successfully implemented using inheritance by creating a superclass and subclass, and displaying vehicle details using a method.
```
