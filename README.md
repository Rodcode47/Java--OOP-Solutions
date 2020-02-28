# Java-OOP-Solutions

1. ### EraseSecurely
```Java
import java.util.Scanner;

public class EraseSecurely {
    public static void main(String[] args) {
    
        Scanner in = new Scanner(System.in);
        int x = in.nextInt();
        String l1 = in.next();
        String l2 = in.next();
        in.close();
        
        if (x%2==0) {
            if (l1.equals(l2)) {
                System.out.println("Deletion succeeded");
            } else {
                System.out.println("Deletion failed");
            }
        } else {
            String result = "Deletion succeeded";
            for (int i = 0; i < l1.length(); i++) {
                if (l1.charAt(i) == l2.charAt(i)) {
                    result = "Deletion failed";
                    break;
                }
            }
            System.out.println(result);
        }
    }
}
```

1. ### FizzBuzz

```Java
import java.util.Scanner;

public class FizzBuzz {
    public static void main(String[] args) {
        Scanner sc = new Scanner(System.in);

        int a = sc.nextInt();
        int b = sc.nextInt();
        int c = sc.nextInt();
        sc.close();

        for (int i = 1; i <= c; i++) {
            if (i % a == 0 && i % b == 0) {
                System.out.println("FizzBuzz");
            } else if (i % a == 0) {
                System.out.println("Fizz");
            } else if (i % b == 0) {
                System.out.println("Buzz");
            } else {
                System.out.println(i);
            }
        }
    }
}
```
