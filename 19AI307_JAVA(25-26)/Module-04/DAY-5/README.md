# Ex.No:4(D) DESIGN PATTERN  ---- BEHAVIOUR PATTERN

## QUESTION:
```
Write a DAO class for a Contact model with fields like name and phone. Implement a method to return all contacts starting with a specific letter.
```
## AIM:
```
To implement a DAO (Data Access Object) behavior pattern in Java to manage contacts and filter them based on the starting letter of the name.
```
## ALGORITHM :
```
1.Start the program
2.Create Contact model class with name and phone
3.Create ContactDAO interface with required methods
4.Implement DAO in ContactDAOImpl class
5.Store contacts in a list
6.Read inputs using Scanner
7.Filter contacts by starting letter
8.Display matching contacts
9.Stop program
```




## PROGRAM:
 ```
/*
Program to implement a Behaviour Pattern using Java
Developed by: PREETHI  A  K
RegisterNumber:  212223230156
*/
```

## SOURCE CODE:
```
import java.util.*;

class Contact {
    private String name;
    private String phone;

    // Constructor
    public Contact(String name, String phone) {
        this.name = name;
        this.phone = phone;
    }

    // Getters
    public String getName() {
        return name;
    }

    public String getPhone() {
        return phone;
    }
}

interface ContactDAO {
    void addContact(Contact contact);
    List<Contact> getContactsStartingWith(char letter);
}

class ContactDAOImpl implements ContactDAO {
    private List<Contact> contacts = new ArrayList<>();

    public void addContact(Contact contact) {
        contacts.add(contact);
    }

    public List<Contact> getContactsStartingWith(char letter) {
        List<Contact> result = new ArrayList<>();

        for (Contact contact : contacts) {
            if (contact.getName().charAt(0) == letter) {
                result.add(contact);
            }
        }

        return result;
    }
}

public class ContactManager {
    public static void main(String[] args) {
        Scanner sc = new Scanner(System.in);

        ContactDAO dao = new ContactDAOImpl();

        int n = sc.nextInt();
        sc.nextLine();

        for (int i = 0; i < n; i++) {
            String name = sc.nextLine();
            String phone = sc.nextLine();

            dao.addContact(new Contact(name, phone));
        }

        char letter = sc.nextLine().charAt(0);

        List<Contact> filteredContacts = dao.getContactsStartingWith(letter);

        for (Contact contact : filteredContacts) {
            System.out.println(contact.getName());
            System.out.println(contact.getPhone());
        }

        sc.close();
    }
}


```



## OUTPUT:

<img width="649" height="748" alt="image" src="https://github.com/user-attachments/assets/b9ca0ca1-e5ec-4117-9341-12a7d49ac4c6" />


## RESULT:
```
Thus, a Java program was successfully implemented using the DAO behavioral pattern to manage and filter contact details based on the starting letter of the name.
```
