# Ex.No:4(C)  COMPOSITION IN JAVA

## QUESTION:
```
Implement a system where a Library contains multiple Book objects. Each Book is created inside the Library (Composition).
```
## AIM:
```
To implement composition in Java by creating a Library class that owns and manages multiple Book objects.
```
## ALGORITHM :
```
1.Start the program
2.Create a Book class with attributes
3.Create a Library class
4.Inside Library, create Book objects (composition)
5.Store books in a collection
6.Display all book details
7.Stop program
```




## PROGRAM:
 ```
/*
Program to implement a Composition Concepts in Java
Developed by: PREETHI A K
RegisterNumber:  212223230156
*/
```

## SOURCE CODE:
```
import java.util.*;

public class CompositionExample {
    public static void main(String[] args) {
        Scanner sc = new Scanner(System.in);
        Library library = new Library();

        int n = sc.nextInt();
        sc.nextLine();

        for (int i = 0; i < n; i++) {
            String title = sc.nextLine();
            String author = sc.nextLine();
            library.addBook(title, author);
        }

        library.showBooks();
        sc.close();
    }
}

class Book {
    private String title;
    private String author;

    public Book(String title, String author) {
        this.title = title;
        this.author = author;
    }

    public String getDetails() {
        return title + " by " + author;
    }
}

class Library {
    private List<Book> books;

    public Library() {
        books = new ArrayList<>();
    }

    public void addBook(String title, String author) {
        books.add(new Book(title, author));
    }

    public void showBooks() {
        System.out.println("Books in Library:");
        for (Book book : books) {
            System.out.println("- " + book.getDetails());
        }
    }
}
```





## OUTPUT:
<img width="847" height="511" alt="image" src="https://github.com/user-attachments/assets/ff687836-a47f-4e83-aa28-d504d9d4a72d" />



## RESULT:
```
Thus, a Java program was successfully implemented using composition where a Library contains and manages Book objects.
```
