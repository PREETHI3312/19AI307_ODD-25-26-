# Ex.No:4(D) DESIGN PATTERN -- ABSTRACT FACTORY

## QUESTION:
```
Implement Abstract Factory Pattern to create UI components (Button and Checkbox) for Dark and Light themes.
```

## AIM:
```
To implement the Abstract Factory design pattern in Java for creating theme-based UI components.
```

## ALGORITHM :
```
1.Start the program
2.Create interfaces Button and Checkbox
3.Create concrete classes for Dark and Light variants
4.Create abstract factory interface UIFactory
5.Implement DarkFactory and LightFactory
6.Read user input for theme
7.Create objects using factory
8.Display created components
9.Stop program
```




## PROGRAM:
 ```
/*
Program to implement a Abstract Factory Pattern using Java
Developed by: PREETHI A K
RegisterNumber:  212223230156
*/
```

## SOURCE CODE:
```
import java.util.Scanner;

// Abstract Products
interface Button {
    void create();
}

interface Checkbox {
    void create();
}

// Dark Theme Products
class DarkButton implements Button {
    public void create() {
        System.out.println("Dark Button created");
    }
}

class DarkCheckbox implements Checkbox {
    public void create() {
        System.out.println("Dark Checkbox created");
    }
}

// Light Theme Products
class LightButton implements Button {
    public void create() {
        System.out.println("Light Button created");
    }
}

class LightCheckbox implements Checkbox {
    public void create() {
        System.out.println("Light Checkbox created");
    }
}

// Abstract Factory
interface UIFactory {
    Button createButton();
    Checkbox createCheckbox();
}

// Dark Factory
class DarkThemeFactory implements UIFactory {
    public Button createButton() {
        return new DarkButton();
    }

    public Checkbox createCheckbox() {
        return new DarkCheckbox();
    }
}

// Light Factory
class LightThemeFactory implements UIFactory {
    public Button createButton() {
        return new LightButton();
    }

    public Checkbox createCheckbox() {
        return new LightCheckbox();
    }
}

// Main Class
public class Main {
    public static void main(String[] args) {
        Scanner sc = new Scanner(System.in);
        String theme = sc.nextLine().trim().toLowerCase();

        UIFactory factory = null;

        if (theme.equals("dark")) {
            factory = new DarkThemeFactory();
        } 
        else if (theme.equals("light")) {
            factory = new LightThemeFactory();
        } 
        else {
            System.out.println("Invalid theme");
            return; // stop execution
        }

        Button button = factory.createButton();
        Checkbox checkbox = factory.createCheckbox();

        button.create();
        checkbox.create();

        sc.close();
    }
}
```




## OUTPUT:
<img width="818" height="292" alt="image" src="https://github.com/user-attachments/assets/dad0e35a-81dc-459e-ae50-435867b05ad3" />



## RESULT:
```
Thus, a Java program was successfully implemented using the Abstract Factory design pattern to generate theme-based UI components dynamically.
```
