# Solution (No peeking!)


<details> <summary> 👀 Answer  </summary>

```java

import mycolor.color;
import java.util.Scanner;

public class Main {
    public static void main(String[] args) {
        Scanner scanner = new Scanner(System.in);
        while (true) {
            displayMenu();
            System.out.print("Enter your choice: ");
            int choice = scanner.nextInt();
            scanner.nextLine();
            switch (choice) {
                case 1:
                    System.out.print("Enter your message: ");
                    String redMessage = scanner.nextLine();
                    color.printColored(redMessage, color.RED);
                    break;
                case 2:
                    System.out.print("Enter your message: ");
                    String greenMessage = scanner.nextLine();
                    color.printColored(greenMessage, color.GREEN);
                    break;
                case 3:
                    System.out.print("Enter your message: ");
                    String blueMessage = scanner.nextLine();
                    color.printColored(blueMessage, color.BLUE);
                    break;
                case 4:
                    System.out.println("Exiting...");
                    System.exit(0);
                    break;
                default:
                    System.out.println("Invalid choice.");
            }
        }
    }

    public static void displayMenu() {
        System.out.println("====== Colorful Console Menu ======");
        System.out.println("1. Print Red Message");
        System.out.println("2. Print Green Message");
        System.out.println("3. Print Blue Message");
        System.out.println("4. Exit");
        System.out.println("===================================");
    }
}


```

</details>