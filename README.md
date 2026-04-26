[Program 1: Create a class with four methods: Addition, Subtraction, Multiplication, and Division. Now, test all four methods in the public static void main. ](#Program1)

[Program 2: Write a Program in Java using OOPs concept for the addition of two distances where each distance is given in metres, centimetres, and millimeters.](#Program2)

[Program 3: Write a Program to test for loop, while loop, do while loop. ](#Program3)

[Program 4: Write a Program using if-else to print the grade of input marks.](#Program4)

[Program 5: Write a Program in Java using objects and classes to get the square of stars for dynamic width and height.](#Program5)

[Program 6: Write a Program in Java using objects and classes to get the pyramid of stars or triangle of stars.](#Program6)

[Program 7: Write a Program in Java using OOPs concept for the addition of two distances where each distance is given in metres and centimetres.](#Program7)

[Program 8: Write a Program in Java using OOPs concept for the addition of two times, where each time is given in hours and minutes.](#Program8)

[Program 9: Write a Program in Java using OOPs concept for the addition of two times, where each time is given in hours, minutes, and seconds.](#Program9)

[Program 10: Write a class with four methods for a 1-dimensional array.(Input, output 1,out2, reverse).](#Program10)

[Program 11:  Write a class with multiple methods to perform matrix operations (transpose, addition, sum of rows, sum of columns, sum of diagonal).](#Program11)

[Program 12a:  Collect the code from the internet for any five programs in the C language and convert them to Java. (Factorial).](#Program12a)

[Program 12b:  Collect the code from the internet for any five programs of the C language and convert them to Java. (Armstrong).](#Program12b)

[Program 12c:  Collect the code from the internet for any five programs of the C language and convert them to Java. (Palindrome).](#Program12c)















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

## Program7
```
import java.util.Scanner;

class Distance {
    int meters;
    int centimeters;

    void input() {
        Scanner sc = new Scanner(System.in);
        System.out.print("Enter meters: ");
        meters = sc.nextInt();
        System.out.print("Enter centimeters: ");
        centimeters = sc.nextInt();
    }

    Distance add(Distance d) {
        Distance sum = new Distance();
        sum.centimeters = this.centimeters + d.centimeters;
        sum.meters = this.meters + d.meters + sum.centimeters / 100;
        sum.centimeters = sum.centimeters % 100;  
        return sum;
    }

    void display() {
        System.out.println("Distance = " + meters + " meters and " + centimeters + " centimeters");
    }

    public static void main(String[] args) {
        Distance d1 = new Distance();
        Distance d2 = new Distance();

        System.out.println("Enter first distance:");
        d1.input();

        System.out.println("Enter second distance:");
        d2.input();

        Distance sum = d1.add(d2);

        System.out.print("Sum of distances: ");
        sum.display();
    }
}
```
<img width="553" height="245" alt="image" src="https://github.com/user-attachments/assets/afd38f40-8e09-4266-9d1d-1824095db0f5" />

## Program8
```
import java.util.Scanner;

class Time {
    int hours;
    int minutes;

    void input() {
        Scanner sc = new Scanner(System.in);
        System.out.print("Enter hours: ");
        hours = sc.nextInt();
        System.out.print("Enter minutes: ");
        minutes = sc.nextInt();
    }

    Time add(Time t) {
        Time sum = new Time();
        sum.minutes = this.minutes + t.minutes;
        sum.hours = this.hours + t.hours + sum.minutes / 60; // 60 min = 1 hr
        sum.minutes = sum.minutes % 60;
        return sum;
    }

    void display() {
        System.out.println("Time = " + hours + " hours and " + minutes + " minutes");
    }

    public static void main(String[] args) {
        Time t1 = new Time();
        Time t2 = new Time();

        System.out.println("Enter first time:");
        t1.input();

        System.out.println("Enter second time:");
        t2.input();

        Time sum = t1.add(t2);

        System.out.print("Sum of times: ");
        sum.display();
    }
}
```
<img width="441" height="262" alt="image" src="https://github.com/user-attachments/assets/7a427628-7a52-4947-94cb-69b2a0973497" />

## Program9
```
import java.util.Scanner;

class Time {
    int hours;
    int minutes;
    int seconds;

    void input() {
        Scanner sc = new Scanner(System.in);
        System.out.print("Enter hours: ");
        hours = sc.nextInt();
        System.out.print("Enter minutes: ");
        minutes = sc.nextInt();
        System.out.print("Enter seconds: ");
        seconds = sc.nextInt();
    }

    Time add(Time t) {
        Time sum = new Time();

        sum.seconds = this.seconds + t.seconds;
        sum.minutes = this.minutes + t.minutes + sum.seconds / 60;
        sum.seconds = sum.seconds % 60;

        sum.hours = this.hours + t.hours + sum.minutes / 60;
        sum.minutes = sum.minutes % 60;

        return sum;
    }

    void display() {
        System.out.println("Time = " + hours + " hours, " + minutes + " minutes, " + seconds + " seconds");
    }

    public static void main(String[] args) {
        Time t1 = new Time();
        Time t2 = new Time();

        System.out.println("Enter first time:");
        t1.input();

        System.out.println("Enter second time:");
        t2.input();

        Time sum = t1.add(t2);

        System.out.print("Sum of times: ");
        sum.display();
    }
}
```
<img width="547" height="320" alt="image" src="https://github.com/user-attachments/assets/bc3fa835-4515-43b0-964f-f069bd6dbf85" />

## Program10
```
import java.util.Scanner;

class OneDArray {
    int arr[];
    int n;

    void input() {
        Scanner sc = new Scanner(System.in);
        System. out.print("Enter size of array: ");
        n = sc.nextInt();

        arr = new int[n];
        System.out.println("Enter elements:");

        for (int i = 0; i < n; i++) {
            arr[i] = sc.nextInt();
        }
    }

    void output1() {
        System.out.println("Array elements:");
        for (int i = 0; i < n; i++) {
            System.out.print(arr[i] + " ");
        }
        System.out.println();
    }

    void output2() {
        System.out.println("Even elements:");
        for (int i = 0; i < n; i++) {
            if (arr[i] % 2 == 0) {
                System.out.print(arr[i] + " ");
            }
        }
        System.out.println();
    }

    void reverse() {
        System.out.println("Reversed array:");
        for (int i = n - 1; i >= 0; i--) {
            System.out.print(arr[i] + " ");
        }
        System.out.println();
    }

    public static void main(String[] args) {
        OneDArray obj = new OneDArray();
        obj.input();
        obj.output1();
        obj.output2();
        obj.reverse();
    }
}
```
<img width="286" height="327" alt="image" src="https://github.com/user-attachments/assets/afc8b620-5a04-4022-b1b6-045f284a409b" />

## Program11
```
import java.util.Scanner;

class MatrixOperations {
    int a[][], b[][];
    int r, c;

    void input() {
        Scanner sc = new Scanner(System.in);

        System.out.print("Enter rows and columns: ");
        r = sc.nextInt();
        c = sc.nextInt();

        a = new int[r][c];
        b = new int[r][c];

        System.out.println("Enter first matrix:");
        for (int i = 0; i < r; i++) {
            for (int j = 0; j < c; j++) {
                a[i][j] = sc.nextInt();
            }
        }

        System.out.println("Enter second matrix:");
        for (int i = 0; i < r; i++) {
            for (int j = 0; j < c; j++) {
                b[i][j] = sc.nextInt();
            }
        }
    }

    void addition() {
        System.out.println("Matrix Addition:");
        for (int i = 0; i < r; i++) {
            for (int j = 0; j < c; j++) {
                System.out.print((a[i][j] + b[i][j]) + " ");
            }
            System.out.println();
        }
    }

    void transpose() {
        System.out.println("Transpose of first matrix:");
        for (int i = 0; i < c; i++) {
            for (int j = 0; j < r; j++) {
                System.out.print(a[j][i] + " ");
            }
            System.out.println();
        }
    }

    void sumRows() {
        System. out.println("Sum of rows:");
        for (int i = 0; i < r; i++) {
            int sum = 0;
            for (int j = 0; j < c; j++) {
                sum += a[i][j];
            }
            System.out.println("Row " + i + ": " + sum);
        }
    }

    void sumColumns() {
        System. out.println("Sum of columns:");
        for (int j = 0; j < c; j++) {
            int sum = 0;
            for (int i = 0; i < r; i++) {
                sum += a[i][j];
            }
            System.out.println("Column " + j + ": " + sum);
        }
    }

    void sumDiagonal() {
        int sum = 0;
        for (int i = 0; i < r; i++) {
            sum += a[i][i]; // main diagonal
        }
        System.out.println("Sum of diagonal: " + sum);
    }

    public static void main(String[] args) {
        MatrixOperations obj = new MatrixOperations();
        obj.input();
        obj.addition();
        obj.transpose();
        obj.sumRows();
        obj.sumColumns();
        obj.sumDiagonal();
    }
}
```
<img width="623" height="762" alt="image" src="https://github.com/user-attachments/assets/c02dd76f-9477-4e05-bc80-d529f74b1219" />

## Program12a
```
import java.util.Scanner;

class Factorial {
    public static void main(String[] args) {
        int n, fact = 1;

        Scanner sc = new Scanner(System.in);
        System.out.print("Enter a number: ");
        n = sc.nextInt();

        for (int i = 1; i <= n; i++) {
            fact *= i;
        }

        System.out.println("Factorial = " + fact);
    }
}
```
<img width="311" height="111" alt="image" src="https://github.com/user-attachments/assets/be71dcde-8ddd-4885-acb0-b2a9f2a25d22" />

## Program12b
```
import java.util.Scanner;

class Armstrong {
    public static void main(String[] args) {
        int n, temp, rem, sum = 0;

        Scanner sc = new Scanner(System.in);
        System.out.print("Enter a number: ");
        n = sc.nextInt();

        temp = n;

        while (n > 0) {
            rem = n % 10;
            sum += rem * rem * rem;
            n = n / 10;
        }

        if (temp == sum)
            System. out.println("Armstrong Number");
        else
            System. out.println("Not an Armstrong Number");
    }
}
```
<img width="296" height="145" alt="image" src="https://github.com/user-attachments/assets/52eafa4d-52d7-4095-a4ad-dd09b3f57dd0" />

## Program12c
```
import java.util.Scanner;

class Palindrome {
    public static void main(String[] args) {
        int n, rev = 0, rem, temp;

        Scanner sc = new Scanner(System.in);
        System.out.print("Enter a number: ");
        n = sc.nextInt();

        temp = n;

        while (n > 0) {
            rem = n % 10;
            rev = rev * 10 + rem;
            n = n / 10;
        }

        if (temp == rev)
            System. out.println("Palindrome Number");
        else
            System. out.println("Not a Palindrome Number");
    }
}
```
<img width="298" height="130" alt="image" src="https://github.com/user-attachments/assets/2379507e-dc12-4359-96ab-79129f7ccdbb" />

















