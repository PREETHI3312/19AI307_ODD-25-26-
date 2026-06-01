# Ex.No:2(C) ACCESS SPECIFIERS

## QUESTION:
```
Write a Java program to create a class called “Book” with private instance variables title, author, and price. Provide public getter and setter methods to access and modify these variables. Add a method called applyDiscount() that takes a percentage as a parameter and reduces the price by that percentage.
```

## AIM:
```
To write a Java program using access specifiers (private and public) to encapsulate data in a class and apply discount on book price.
```

## ALGORITHM :
```
1.Start the program
2.Create a class Book with private variables title, author, price
3.Create public getter and setter methods for each variable
4.Create a method applyDiscount() to reduce price by given percentage
5.In main method, create a Book object
6.Set values using setter methods
7.Apply discount
8.Display updated details
9.Stop program
```



## PROGRAM:
 ```
/*
Program to implement a Access Specifiers using Java
Developed by: PREETHI A K
RegisterNumber:  212223230156
*/
```

## SOURCE CODE:
```
import java.util.Scanner;

class Book {
    private String title;
    private String author;
    private double price;

    public String getTitle() {
        return title;
    }

    public String getAuthor() {
        return author;
    }

    public double getPrice() {
        return price;
    }

    public void setTitle(String title) {
        this.title = title;
    }

    public void setAuthor(String author) {
        this.author = author;
    }

    public void setPrice(double price) {
        this.price = price;
    }

    public void applyDiscount(double percentage) {
        if (percentage > 0 && percentage <= 100) {
            price = price - (price * (percentage / 100));
        }
    }

    public void display() {
        System.out.println("Title: " + title);
        System.out.println("Author: " + author);
        System.out.printf("Discounted Price: %.2f\n", price);
        System.out.println("-------------------------");
    }
}

class prog {
    public static void main(String[] args) {
        Scanner sc = new Scanner(System.in);

        Book b = new Book();

        b.setTitle(sc.nextLine());
        b.setAuthor(sc.nextLine());
        b.setPrice(sc.nextDouble());
        double discount = sc.nextDouble();

        b.applyDiscount(discount);
        b.display();

        sc.close();
    }
}
```







## OUTPUT:
<img width="1027" height="578" alt="image" src="https://github.com/user-attachments/assets/cf98a78b-c2b5-4f33-a690-bc4733270828" />




## RESULT:
```
Thus, a Java program was successfully implemented using access specifiers with private variables, public getter and setter methods, and a discount calculation method.
```
