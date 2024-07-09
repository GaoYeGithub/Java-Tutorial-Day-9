# Color in the Console 

You might wonder if you can add color to your console and the answer is of course

And today we are going use what we learn before to do it.
To begin let see normal color changing without a packages it like this

```java
public class Main {
    public static void main(String[] args) {
        System.out.print("\033[0;31mHello\033[0m");
    }
}
```
Very efficent as you will need to constanly search up the color and add thoose readom \ and [ and more but we can label them like this

Here are some common colors

```java
      String RESET = "\033[0m";      // White
      String RED = "\033[0;31m";     // RED
      String GREEN = "\033[0;32m";   // GREEN
      String YELLOW = "\033[0;33m";  // YELLOW
      String BLUE = "\033[0;34m";    // BLUE
      String PURPLE = "\033[0;35m";  // PURPLE
      String CYAN = "\033[0;36m";    // CYAN
```
With this we can do this 

```java
public class Main {
    public static void main(String[] args) {
      String RESET = "\033[0m";      // White
      String RED = "\033[0;31m";     // RED
      String GREEN = "\033[0;32m";   // GREEN
      String YELLOW = "\033[0;33m";  // YELLOW
      String BLUE = "\033[0;34m";    // BLUE
      String PURPLE = "\033[0;35m";  // PURPLE
      String CYAN = "\033[0;36m";    // CYAN
      System.out.println(RED + "This text is red!" + RESET);
    }
}
```
Try using other colors or decorateing your old project with these colors.
