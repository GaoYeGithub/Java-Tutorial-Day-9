# Making our Package

To make a package let first create folder thats our package and create another java in the directory or files

It should already be there

```java
package mycolor;

public class color {
    public static final String RESET = "\033[0m";
    public static final String RED = "\033[0;31m";
    public static final String GREEN = "\033[0;32m";
    public static final String YELLOW = "\033[0;33m";
    public static final String BLUE = "\033[0;34m";
    public static final String PURPLE = "\033[0;35m";
    public static final String CYAN = "\033[0;36m";

    public static void printColored(String message, String color) {
        System.out.println(color + message + RESET);
    }
}

```

It works like this 
![](resources/03image.PNG)

Then here how you call it
```java
import mycolor.color;

public class Main {
    public static void main(String[] args) {
        color.printColored("This is a red message", color.RED);
        color.printColored("This is a green message", color.GREEN);
        color.printColored("This is a blue message", color.BLUE);
    }
}

```