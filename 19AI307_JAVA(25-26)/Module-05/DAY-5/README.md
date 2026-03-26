# Ex.No:5(E) MULTITHREADING -SYNCHRONIZATION

## QUESTION:
Use a thread pool to calculate and print the square of each number from input.

Input :

3 2 4 5
Output:

Square: 4

Square: 16

Square: 25


## AIM:
To write a Java program that calculates and prints the square of n input numbers using a Thread Pool (ExecutorService).
## ALGORITHM :
1. Start the program and import the necessary java.util and java.util.concurrent packages.

2. Initialize a Scanner object to read input from the user.

3. Read an integer n which represents the count of numbers to be processed.

4. Create a thread pool using Executors.newSingleThreadExecutor().

5. Loop n times: Read the next integer from the input.

6. Define a Runnable task using a lambda expression that calculates the square of the number and prints it.

7. Shutdown the executor service to free up resources and close the scanner.

## PROGRAM:
 ```
/*
Program to implement a Synchronization concept using Java
Developed by: YUVAN SUNDAR S
Register Number: 212223040250
*/
```

## SOURCE CODE:
```java
import java.util.Scanner;
import java.util.concurrent.ExecutorService;
import java.util.concurrent.Executors;

public class SquareCalculator {

    public static void main(String[] args) {
        Scanner scanner = new Scanner(System.in);
        int n = scanner.nextInt();

        ExecutorService executor = Executors.newSingleThreadExecutor();

        for (int i = 0; i < n; i++) {
            final int numberToSquare = scanner.nextInt();

            Runnable task = () -> {
                int square = numberToSquare * numberToSquare;
                System.out.println("Square: " + square);
            };

            executor.submit(task);
        }

        executor.shutdown();
        scanner.close();
    }
}
```

## OUTPUT:
<img width="405" height="454" alt="image" src="https://github.com/user-attachments/assets/f7711603-99de-46a9-a22e-bcbd6af72d9f" />


## RESULT:
The program was executed successfully as the squares of the numbers were calculated using a thread pool and printed to the console.




