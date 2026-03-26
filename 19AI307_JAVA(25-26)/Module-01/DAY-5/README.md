# Ex.No:1(E) STRINGS AND MATH FUNCTION

## QUESTION:
Write a Java program to compare two strings.



## AIM:
To write a Java program that accepts two strings as input and compares them using the .equals() method to check if they are identical.

## ALGORITHM :
1. Begin the program and initialize the Scanner object to read input.

2. Declare two String variables (s1, s2) and accept their values from the user.

3. Use the condition if(s1.equals(s2)) to compare the content of both strings.

4. If the condition is true, print the message "Strings are equal."

5. If the condition is false (inside the else block), print "Strings are not equal."


## PROGRAM:
 ```
/*
Program to implement a Strings and Math Function using Java
Developed by: YUVAN SUNDAR S
RegisterNumber: 212223040250
*/
```

## SOURCE CODE:
```java
import java.util.*;
public class Main{
    public static void main(String args[]){
        Scanner sc=new Scanner(System.in);
        String s1=sc.next(),s2=sc.next();
        if(s1.equals(s2)){
            System.out.println("Strings are equal.");
        }
        else
        {
            System.out.println("Strings are not equal.");
        }
        
    }
}
```

## OUTPUT:
<img width="500" height="500" alt="image" src="https://github.com/user-attachments/assets/dcea1147-b3c3-4810-acba-dd9f69870b25" />

## RESULT:

Thus the program that reads two strings and compares them is executed successfully.


