# Java Packages

Java packages are often used to group related classes and interfaces. Helping to organize your code and avoid name conflicts. 

Like a folder that store different files.

## Importing Classes and Packages from Java API

The Java API provides a vast library of classes and packages that you can use in your programs. To use these classes, you need to import them.

There are ones we used alread like Scanner

```java
import java.util.Scanner;

public class Main {
    public static void main(String[] args) {
        Scanner scanner = new Scanner(System.in);
        System.out.println("Enter your name:");
        String name = scanner.nextLine();
        System.out.println("Hello, " + name + "!");
    }
}
```

But you can import all java parkages using *

```java
import java.util.*;

public class Main {
    public static void main(String[] args) {
        Scanner scanner = new Scanner(System.in);
        System.out.println("Enter your name:");
        String name = scanner.nextLine();
        System.out.println("Hello, " + name + "!");

        ArrayList<String> list = new ArrayList<String>();
        list.add(name);
        System.out.println("List: " + list);
    }
}
```