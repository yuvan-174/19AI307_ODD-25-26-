# Ex.No:1(A) INTRODUCTION TO JAVA PROGRAMMING, DATA TYPES, VARIABLES AND OPERATORS

## QUESTION:
Lovely is preparing a countdown for her rocket launch game. She has a starting number and wants to understand how subtracting with -- works in Java. But she's puzzled by the two types:
Post-decrement (a--) → value is used first, then decreased
Pre-decrement (--a) → value is decreased first, then used

## AIM:
To write a Java program that accepts an integer input and demonstrates the difference between post-decrement (a--) and pre-decrement (--a) operators.


## ALGORITHM :
1. Initialize the program and the Scanner class.
2. Read an integer from the user and store it in variable a.
3. Print the initial value of a.
4. Print the value of a (before change), decrement it, then print the updated a.
5. Decrement a first, then print the new value and the final a.


## PROGRAM:
 ```
/*
Program to implement variables and Operators using Java
Developed by: Yuvan Sundar S
RegisterNumber:  212223040250
*/
```

## Sourcecode.java:

```
import java.util.*;
public class Main{
    public static void main(String args[]){
        Scanner sc=new Scanner(System.in);
        int a=sc.nextInt();
        System.out.println("Initial countdown = "+a);
        System.out.println("After post-decrement (a--) = "+(a--)+", Now a = "+a);
        System.out.println("After pre-decrement (--a) = "+(--a)+", Now a = "+a);
    }
}
```

## OUTPUT:
<img width="500" height="500" alt="image" src="https://github.com/user-attachments/assets/62481bfc-a000-43c2-8411-ec2c1aad5d74" />

## RESULT:

Thus the Java program that does post-decrement and pre-decrement operators are executed successfully.

