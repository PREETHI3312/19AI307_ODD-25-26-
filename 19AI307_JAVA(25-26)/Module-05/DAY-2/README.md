# Ex.No:5(B) SERIALIZATION AND DESERIALIZATION 

## QUESTION:
```
Write a Java program to serialize a collection of objects (like ArrayList<Student>) into a file.
```

## AIM:
```
To write a Java program to serialize an ArrayList of Student objects into a file using object serialization.
```

## ALGORITHM :
1.Start the program
2.Create a Student class implementing Serializable
3.Create an ArrayList<Student>
4.Add student objects to the list
5.Create FileOutputStream
6.Wrap it with ObjectOutputStream
7.Write the object list to file
8.Close streams
9.Stop program





## PROGRAM:
 ```
/*
Program to implement a Serialization and Deserialization using Java
Developed by: PREETHI A K
RegisterNumber: 212223230156 
*/
```

## SOURCE CODE:
```
import java.io.*;
import java.util.*;

// Student class must implement Serializable
class Student implements Serializable {
    private static final long serialVersionUID = 1L;

    private int id;
    private String name;
    private double marks;

    public Student(int id, String name, double marks) {
        this.id = id;
        this.name = name;
        this.marks = marks;
    }

    @Override
    public String toString() {
        return "Student{id=" + id + ", name='" + name + "', marks=" + marks + "}";
    }
}

public class StudentSerializationUserInput {

    // Serialize list of students
    public static void serializeStudents(List<Student> students, String fileName) {
        try (ObjectOutputStream oos = new ObjectOutputStream(new FileOutputStream(fileName))) {
            oos.writeObject(students);
            System.out.println("Students serialized successfully into: " + fileName);
        } catch (IOException e) {
            System.out.println("Error during serialization: " + e.getMessage());
        }
    }

    // Deserialize list of students
    @SuppressWarnings("unchecked")
    public static List<Student> deserializeStudents(String fileName) {
        List<Student> students = null;
        try (ObjectInputStream ois = new ObjectInputStream(new FileInputStream(fileName))) {
            students = (List<Student>) ois.readObject();
            System.out.println("Students deserialized successfully from: " + fileName);
        } catch (IOException | ClassNotFoundException e) {
            System.out.println("Error during deserialization: " + e.getMessage());
        }
        return students;
    }

    public static void main(String[] args) {
        Scanner scanner = new Scanner(System.in);
        List<Student> students = new ArrayList<>();

        int n = scanner.nextInt();
        scanner.nextLine(); // consume newline

        // Read student details
        for (int i = 0; i < n; i++) {
            int id = scanner.nextInt();
            scanner.nextLine(); // consume newline

            String name = scanner.nextLine();

            double marks = scanner.nextDouble();
            scanner.nextLine(); // consume newline

            students.add(new Student(id, name, marks));
        }

        String fileName = "students.dat";

        // Serialize students
        serializeStudents(students, fileName);

        // Deserialize students
        List<Student> deserializedStudents = deserializeStudents(fileName);

        // Display deserialized data
        if (deserializedStudents != null) {
            System.out.println("\nDeserialized Students:");
            for (Student s : deserializedStudents) {
                System.out.println(s);
            }
        }

        scanner.close();
    }
}

```




## OUTPUT:
<img width="1189" height="684" alt="image" src="https://github.com/user-attachments/assets/c1f84669-a30f-4706-b658-8a623fdfe591" />



## RESULT:
```
Thus, a Java program was successfully implemented to serialize a collection of Student objects into a file using ObjectOutputStream.
```
