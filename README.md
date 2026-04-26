[Program 1: Create a class with four methods: Addition, Subtraction, Multiplication, and Division. Now, test all four methods in the public static void main. ](#Program1)

[Program 2: Write a Program in Java using OOPs concept for the addition of two distances where each distance is given in metres, centimetres, and millimeters.](#Program2)

[Program 3: Write a Program to test for loop, while loop, do while loop. ](#Program3)

[Program 4: Write a Program using if-else to print the grade of input marks.](#Program4)

[Program 5: Write a Program in Java using objects and classes to get the square of stars for dynamic width and height.](#Program5)

[Program 6: Write a Program in Java using objects and classes to get the pyramid of stars or triangle of stars.](#Program6)






## Program1
```
public class Calc {
        public static void main(String[] args){
        int a=Integer.parseInt(args[0]);
        int b=Integer.parseInt(args[1]);
        add(a,b);
        sub(a,b);
        mul(a,b);
        div(a,b);

    }
    public static void add(int a, int b){
    System.out.println("Addition:"+(a+b));
    }    
   public static void sub(int a, int b){
    System.out.println("Subtraction:"+(a-b));
    }
    public static void mul(int a, int b){
    System.out.println("Multiplication:"+(a*b));
    }
    public static void div(int a, int b){
    System.out.println("Division:"+(a/b));
    }
    
}
```
<img width="398" height="185" alt="image" src="https://github.com/user-attachments/assets/48ff84f1-ad7b-4c7e-a232-a4100538cfd6" />


## Program2
```
import java.util.Scanner;
public class DistanceAdd {
    public static void main(String[] args) {
        Scanner sc = new Scanner(System.in);

        int m1, c1, mm1;
        int m2, c2, mm2;

        System.out.println("Enter first distance (m cm mm):");
        m1 = sc.nextInt();
        c1 = sc.nextInt();
        mm1 = sc.nextInt();

        System.out.println("Enter second distance (m cm mm):");
        m2 = sc.nextInt();
        c2 = sc.nextInt();
        mm2 = sc.nextInt();

        int m = m1 + m2;
        int cm = c1 + c2;
        int mm = mm1 + mm2;

        if (mm >= 10) {
            cm = cm + mm / 10;
            mm = mm % 10;
        }

        if (cm >= 100) {
            m = m + cm / 100;
            cm = cm % 100;
        }

        System.out.println("Total distance = " + m + " m " + cm + " cm " + mm + " mm");
    }
}
```
<img width="343" height="272" alt="image" src="https://github.com/user-attachments/assets/f7de7c48-472d-4677-9b4c-34d968db9f5e" />

## Program3
```
class LoopTest {
    public static void main(String[] args) {

        System.out.println("Using for loop:");
        for (int i = 1; i <= 5; i++) {
            System.out.println(i);
        }

        System.out.println("\nUsing while loop:");
        int j = 1;
        while (j <= 5) {
            System.out.println(j);
            j++;
        }

        System.out.println("\nUsing do-while loop:");
        int k = 1;
        do {
            System.out.println(k);
            k++;
        } while (k <= 5);
    }
}
```
<img width="388" height="532" alt="image" src="https://github.com/user-attachments/assets/94e18dc5-3541-4554-b705-ecb20a8c11bb" />

## Program4
```
import java.util.Scanner;

class GradeCheck {
    public static void main(String[] args) {
        Scanner sc = new Scanner(System.in);

        System. out.print("Enter marks: ");
        int marks = sc.nextInt();

        if (marks >= 90) {
            System.out.println("Grade: A");
        } else if (marks >= 75) {
            System.out.println("Grade: B");
        } else if (marks >= 60) {
            System.out.println("Grade: C");
        } else if (marks >= 50) {
            System.out.println("Grade: D");
        } else {
            System.out.println("Grade: F");
        }

        sc.close();
    }
}
```
<img width="300" height="182" alt="image" src="https://github.com/user-attachments/assets/9fd034f4-22e3-4f9d-ac94-f10384092e1f" />

## Program5
```
import java.util.Scanner;

class SquareStars {

    int width, height;

    void input() {
        Scanner sc = new Scanner(System.in);
        System.out.print("Enter width: ");
        width = sc.nextInt();
        System.out.print("Enter height: ");
        height = sc.nextInt();
    }

    void printSquare() {
        for (int i = 1; i <= height; i++) {
            for (int j = 1; j <= width; j++) {
                System.out.print("* ");
            }
            System.out.println();
        }
    }

    public static void main(String[] args) {
        SquareStars obj = new SquareStars();
        obj.input();
        obj.printSquare();
    }
}
```
<img width="302" height="327" alt="image" src="https://github.com/user-attachments/assets/d3041af1-5dec-4a2a-bacb-336309c2370a" />

## Program6
```
import java.util.Scanner;

class PyramidStars {

    int n;

    void input() {
        Scanner sc = new Scanner(System.in);
        System.out.print("Enter number of rows: ");
        n = sc.nextInt();
    }

    void printPyramid() {
        for (int i = 1; i <= n; i++) {

            for (int j = 1; j <= n - i; j++) {
                System.out.print(" ");
            }

            for (int k = 1; k <= (2 * i - 1); k++) {
                System.out.print("*");
            }

            System.out.println();
        }
    }

    public static void main(String[] args) {
        PyramidStars obj = new PyramidStars();
        obj.input();
        obj.printPyramid();
    }
}
```
<img width="327" height="185" alt="image" src="https://github.com/user-attachments/assets/0a1e4534-c13a-427b-8ca4-36593a39f67f" />









