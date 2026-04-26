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

[Program 12d:  Collect the code from the internet for any five programs of the C language and convert them to Java. (Fibonacci).](#Program12d)

[Program 12e:  Collect the code from the internet for any five programs of the C language and convert them to Java. (Pattern).](#Program12e)

[Program 13:  Write a program using three classes to print 1–100, 1–100, 1–100  without a thread, and analyse the output, and repeat the same program using the Runnable interface.](#Program13)

[Program 14:  Write a program using three classes to print 1–100, 1–100, 1–100  with a thread and analyse the output, and repeat the same program using the Runnable interface.](#Program14)

[Program 15:  Using the concept of multithreading, the output of all three threads must be synchronised (use the join method).](#Program15)

[Program 16: Addition of 2 numbers using Swing.](#Program16)

[Program 17:  Make one calculator in Swing.](#Program17)

[Program 18:  Matrix Addition using swing class.](#Program18)

[Program 19:  Create one JFrame with 10 buttons on it. After clicking on each button, a new structure is created (Circle, oval, rectangle, etc). ](#Program19)

[Program 20:  Just using mouse events creates a frame like a paint brush with selection of colour and width.](#Program20)

[Program 21:  Create a package of any 5 classes of your choice and import it.](#Program21)

[Program 22:  Create one package and a sub-package, import and test it.](#Program22)

[Program 23:  Create one small array of size 5, apply array out of bounds exception using try-catch, give a proper message in catch, and demonstrate the exception exactly in the same fashion. 
Demonstrate arithmetic exception also. ](#Program23)

[Program 24:  To test the range of age of one student, write a program using a user-defined exception.](#Program24)

[Program 25: File Handling Programs (given in the PPT).](#Program25)

[Program 26:  Inheritance Programs, using interface and abstract classes.](#Program26)
































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

## Program12d
```
import java.util.Scanner;

class Fibonacci {
    public static void main(String[] args) {
        int n, a = 0, b = 1, c;

        Scanner sc = new Scanner(System.in);
        System.out.print("Enter number of terms: ");
        n = sc.nextInt();

        System.out.println("Fibonacci Series:");
        System.out.print(a + " " + b + " ");

        for (int i = 3; i <= n; i++) {
            c = a + b;
            System.out.print(c + " ");
            a = b;
            b = c;
        }
    }
}
```
<img width="302" height="137" alt="image" src="https://github.com/user-attachments/assets/76bfb919-1d62-4249-88a2-b6d96417f839" />

## Pattern12e
```
class Pattern {
    public static void main(String[] args) {

        for (int i = 1; i <= 5; i++) {
            for (int j = 1; j <= i; j++) {
                System.out.print("* ");
            }
            System.out.println();
        }
    }
}
```
<img width="303" height="176" alt="image" src="https://github.com/user-attachments/assets/d02bbfe4-08f5-4adf-81b6-7fcfed0228d3" />

## Program13
```
class PrintOneToHundred {
    void display() {
        System. out.println("Printing 1 to 100:");
        for (int i = 1; i <= 100; i++) {
            System.out.print(i + " ");
        }
        System.out.println();
    }
}

class PrintHundredToOne {
    void display() {
        System. out.println("Printing 100 to 1:");
        for (int i = 100; i >= 1; i--) {
            System.out.print(i + " ");
        }
        System.out.println();
    }
}

class PrintOneToHundredAgain {
    void display() {
        System. out.println("Printing 1 to 100 again:");
        for (int i = 1; i <= 100; i++) {
            System.out.print(i + " ");
        }
        System.out.println();
    }
}

public class Main {
    public static void main(String[] args) {
        PrintOneToHundred obj1 = new PrintOneToHundred();
        PrintHundredToOne obj2 = new PrintHundredToOne();
        PrintOneToHundredAgain obj3 = new PrintOneToHundredAgain();

        obj1.display();
        obj2.display();
        obj3.display();
    }
}
```
<img width="1136" height="600" alt="image" src="https://github.com/user-attachments/assets/e413391d-4072-447a-b574-7fd6aee1b700" />

## Program14
```
class ThreadOne extends Thread {
    public void run() {
        System. out.println("Thread 1: Printing 1 to 100");
        for (int i = 1; i <= 100; i++) {
            System.out.print(i + " ");
        }
        System.out.println();
    }
}

class ThreadTwo extends Thread {
    public void run() {
        System. out.println("Thread 2: Printing 100 to 1");
        for (int i = 100; i >= 1; i--) {
            System.out.print(i + " ");
        }
        System.out.println();
    }
}

class ThreadThree extends Thread {
    public void run() {
        System. out.println("Thread 3: Printing 1 to 100");
        for (int i = 1; i <= 100; i++) {
            System.out.print(i + " ");
        }
        System.out.println();
    }
}

public class Main {
    public static void main(String[] args) {

        ThreadOne t1 = new ThreadOne();
        ThreadTwo t2 = new ThreadTwo();
        ThreadThree t3 = new ThreadThree();

        t1.start();
        t2.start();
        t3.start();
    }
}
```
<img width="1143" height="535" alt="image" src="https://github.com/user-attachments/assets/462d3a91-6b5d-413c-af55-6a9ae7b2ff2e" />

## Program15
```
class ThreadOne extends Thread {
    public void run() {
        System. out.println("Thread 1: Printing 1 to 100");
        for (int i = 1; i <= 100; i++) {
            System.out.print(i + " ");
        }
        System.out.println();
    }
}

class ThreadTwo extends Thread {
    public void run() {
        System. out.println("Thread 2: Printing 100 to 1");
        for (int i = 100; i >= 1; i--) {
            System.out.print(i + " ");
        }
        System.out.println();
    }
}

class ThreadThree extends Thread {
    public void run() {
        System. out.println("Thread 3: Printing 1 to 100");
        for (int i = 1; i <= 100; i++) {
            System.out.print(i + " ");
        }
        System.out.println();
    }
}

public class Main {
    public static void main(String[] args) {

        ThreadOne t1 = new ThreadOne();
        ThreadTwo t2 = new ThreadTwo();
        ThreadThree t3 = new ThreadThree();

        try {
            t1.start();
            t1.join();   

            t2.start();
            t2.join();  

            t3.start();
            t3.join();  

        } catch (InterruptedException e) {
            System. out.println("Exception: " + e);
        }
    }
}
```
<img width="1141" height="582" alt="image" src="https://github.com/user-attachments/assets/b82efa29-d204-4ac8-b6ba-b3cc20584524" />

## Program16
```
import javax.swing.*;
import java.awt.event.*;

public class Main extends JFrame implements ActionListener {
    JLabel l1, l2, l3;
    JTextField t1, t2, t3;
    JButton b1;

    Main() {
        l1 = new JLabel("Enter First Number:");
        l2 = new JLabel("Enter Second Number:");
        l3 = new JLabel("Result:");

        t1 = new JTextField();
        t2 = new JTextField();
        t3 = new JTextField();
        t3.setEditable(false);

        b1 = new JButton("Add");
        b1.addActionListener(this);

        l1.setBounds(50, 50, 150, 30);
        t1.setBounds(200, 50, 150, 30);

        l2.setBounds(50, 100, 150, 30);
        t2.setBounds(200, 100, 150, 30);

        l3.setBounds(50, 150, 150, 30);
        t3.setBounds(200, 150, 150, 30);

        b1.setBounds(140, 220, 100, 30);

        add(l1); add(t1);
        add(l2); add(t2);
        add(l3); add(t3);
        add(b1);

        setTitle("Addition of Two Numbers");
        setSize(450, 350);
        setLayout(null);
        setVisible(true);
        setDefaultCloseOperation(JFrame.EXIT_ON_CLOSE);
    }

    public void actionPerformed(ActionEvent e) {
        int num1 = Integer.parseInt(t1.getText());
        int num2 = Integer.parseInt(t2.getText());
        int sum = num1 + num2;
        t3.setText(String.valueOf(sum));
    }

    public static void main(String[] args) {
        new Main();
    }
}
```
<img width="588" height="392" alt="image" src="https://github.com/user-attachments/assets/4b9053b7-7480-4507-8bd5-45d2464b7c8e" /> 

## Program17
```
import javax.swing.*;
import java.awt.event.*;

public class Main extends JFrame implements ActionListener {
    JLabel l1, l2, l3;
    JTextField t1, t2, t3;
    JButton b1, b2, b3, b4, b5;

    Main() {
        l1 = new JLabel("First Number:");
        l2 = new JLabel("Second Number:");
        l3 = new JLabel("Result:");

        t1 = new JTextField();
        t2 = new JTextField();
        t3 = new JTextField();
        t3.setEditable(false);

        b1 = new JButton("Add");
        b2 = new JButton("Sub");
        b3 = new JButton("Mul");
        b4 = new JButton("Div");
        b5 = new JButton("Clear");

        b1.addActionListener(this);
        b2.addActionListener(this);
        b3.addActionListener(this);
        b4.addActionListener(this);
        b5.addActionListener(this);

        l1.setBounds(50, 50, 100, 30);
        t1.setBounds(170, 50, 150, 30);

        l2.setBounds(50, 100, 100, 30);
        t2.setBounds(170, 100, 150, 30);

        l3.setBounds(50, 150, 100, 30);
        t3.setBounds(170, 150, 150, 30);

        b1.setBounds(30, 220, 70, 30);
        b2.setBounds(110, 220, 70, 30);
        b3.setBounds(190, 220, 70, 30);
        b4.setBounds(270, 220, 70, 30);
        b5.setBounds(150, 270, 80, 30);

        add(l1); add(t1);
        add(l2); add(t2);
        add(l3); add(t3);
        add(b1); add(b2); add(b3); add(b4); add(b5);

        setTitle("Calculator Using Swing");
        setSize(400, 380);
        setLayout(null);
        setVisible(true);
        setDefaultCloseOperation(JFrame.EXIT_ON_CLOSE);
    }

    public void actionPerformed(ActionEvent e) {
        try {
            double num1 = Double.parseDouble(t1.getText());
            double num2 = Double.parseDouble(t2.getText());
            double result = 0;

            if (e.getSource() == b1) {
                result = num1 + num2;
            } else if (e.getSource() == b2) {
                result = num1 - num2;
            } else if (e.getSource() == b3) {
                result = num1 * num2;
            } else if (e.getSource() == b4) {
                if (num2 == 0) {
                    JOptionPane.showMessageDialog(this, "Division by zero is not allowed");
                    return;
                }
                result = num1 / num2;
            } else if (e.getSource() == b5) {
                t1.setText("");
                t2.setText("");
                t3.setText("");
                return;
            }

            t3.setText(String.valueOf(result));

        } catch (NumberFormatException ex) {
            JOptionPane.showMessageDialog(this, "Please enter valid numbers");
        }
    }

    public static void main(String[] args) {
        new Main();
    }
}
```
<img width="615" height="567" alt="image" src="https://github.com/user-attachments/assets/d895f3db-086d-40f7-a792-7792c9f38f6c" />

## program18
```
import javax.swing.*;
import java.awt.event.*;

public class Main extends JFrame implements ActionListener {

    JTextField a11, a12, a21, a22;
    JTextField b11, b12, b21, b22;
    JTextField r11, r12, r21, r22;
    JButton addBtn, clearBtn;

    Main() {
        setTitle("Matrix Addition (2x2)");
        setSize(420, 320);
        setLayout(null);

        JLabel la = new JLabel("Matrix A");
        la.setBounds(60, 10, 100, 20);
        add(la);

        a11 = new JTextField(); a11.setBounds(40, 40, 50, 30);
        a12 = new JTextField(); a12.setBounds(100, 40, 50, 30);
        a21 = new JTextField(); a21.setBounds(40, 80, 50, 30);
        a22 = new JTextField(); a22.setBounds(100, 80, 50, 30);

        JLabel lb = new JLabel("Matrix B");
        lb.setBounds(250, 10, 100, 20);
        add(lb);

        b11 = new JTextField(); b11.setBounds(230, 40, 50, 30);
        b12 = new JTextField(); b12.setBounds(290, 40, 50, 30);
        b21 = new JTextField(); b21.setBounds(230, 80, 50, 30);
        b22 = new JTextField(); b22.setBounds(290, 80, 50, 30);

        JLabel lr = new JLabel("Result");
        lr.setBounds(150, 120, 100, 20);
        add(lr);

        r11 = new JTextField(); r11.setBounds(120, 150, 50, 30); r11.setEditable(false);
        r12 = new JTextField(); r12.setBounds(180, 150, 50, 30); r12.setEditable(false);
        r21 = new JTextField(); r21.setBounds(120, 190, 50, 30); r21.setEditable(false);
        r22 = new JTextField(); r22.setBounds(180, 190, 50, 30); r22.setEditable(false);

        addBtn = new JButton("Add");
        clearBtn = new JButton("Clear");
        addBtn.setBounds(90, 240, 80, 30);
        clearBtn.setBounds(200, 240, 80, 30);

        addBtn.addActionListener(this);
        clearBtn.addActionListener(this);

        add(a11); add(a12); add(a21); add(a22);
        add(b11); add(b12); add(b21); add(b22);
        add(r11); add(r12); add(r21); add(r22);
        add(addBtn); add(clearBtn);

        setVisible(true);
        setDefaultCloseOperation(JFrame.EXIT_ON_CLOSE);
    }

    public void actionPerformed(ActionEvent e) {
        if (e.getSource() == addBtn) {
            try {
                int A11 = Integer.parseInt(a11.getText());
                int A12 = Integer.parseInt(a12.getText());
                int A21 = Integer.parseInt(a21.getText());
                int A22 = Integer.parseInt(a22.getText());

                int B11 = Integer.parseInt(b11.getText());
                int B12 = Integer.parseInt(b12.getText());
                int B21 = Integer.parseInt(b21.getText());
                int B22 = Integer.parseInt(b22.getText());

                r11.setText(String.valueOf(A11 + B11));
                r12.setText(String.valueOf(A12 + B12));
                r21.setText(String.valueOf(A21 + B21));
                r22.setText(String.valueOf(A22 + B22));

            } catch (NumberFormatException ex) {
                JOptionPane.showMessageDialog(this, "Enter valid integers");
            }
        }

        if (e.getSource() == clearBtn) {
            JTextField[] fields = {
                a11,a12,a21,a22, b11,b12,b21,b22, r11,r12,r21,r22
            };
            for (JTextField f: fields) f.setText("");
        }
    }

    public static void main(String[] args) {
        SwingUtilities.invokeLater(() -> new Main());
    }
}

```

<img width="514" height="394" alt="image" src="https://github.com/user-attachments/assets/bba719ab-60c3-4a54-955b-358a772f20cd" />

## Program19
```
import javax.swing.*;
import java.awt.*;
import java.awt.event.*;

class ShapePanel extends JPanel {
    String shape = "";

    public void setShape(String shape) {
        this.shape = shape;
        repaint();
    }

    protected void paintComponent(Graphics g) {
        super.paintComponent(g);

        if (shape.equals("Line")) {
            g.drawLine(50, 50, 200, 50);
        } 
        else if (shape.equals("Rectangle")) {
            g.drawRect(50, 50, 120, 80);
        } 
        else if (shape.equals("Square")) {
            g.drawRect(50, 50, 100, 100);
        } 
        else if (shape.equals("Oval")) {
            g.drawOval(50, 50, 150, 100);
        } 
        else if (shape.equals("Circle")) {
            g.drawOval(50, 50, 100, 100);
        } 
        else if (shape.equals("RoundRect")) {
            g.drawRoundRect(50, 50, 150, 100, 30, 30);
        } 
        else if (shape.equals("Arc")) {
            g.drawArc(50, 50, 150, 100, 0, 180);
        } 
        else if (shape.equals("Triangle")) {
            int x[] = {100, 50, 150};
            int y[] = {50, 150, 150};
            g.drawPolygon(x, y, 3);
        } 
        else if (shape.equals("Polygon")) {
            int x[] = {100, 150, 130, 70, 50};
            int y[] = {50, 90, 150, 150, 90};
            g.drawPolygon(x, y, 5);
        } 
        else if (shape.equals("Clear")) {
        }
    }
}

public class Main extends JFrame implements ActionListener {
    JButton b1, b2, b3, b4, b5, b6, b7, b8, b9, b10;
    ShapePanel panel;

    Main() {
        setTitle("Shapes using 10 Buttons");
        setSize(700, 500);
        setLayout(null);

        panel = new ShapePanel();
        panel.setBounds(200, 30, 450, 400);
        panel.setBackground(Color.WHITE);

        b1 = new JButton("Line");
        b2 = new JButton("Rectangle");
        b3 = new JButton("Square");
        b4 = new JButton("Oval");
        b5 = new JButton("Circle");
        b6 = new JButton("RoundRect");
        b7 = new JButton("Arc");
        b8 = new JButton("Triangle");
        b9 = new JButton("Polygon");
        b10 = new JButton("Clear");

        JButton[] buttons = {b1, b2, b3, b4, b5, b6, b7, b8, b9, b10};

        int y = 30;
        for (JButton b: buttons) {
            b.setBounds(30, y, 130, 30);
            b.addActionListener(this);
            add(b);
            y += 35;
        }

        add(panel);

        setVisible(true);
        setDefaultCloseOperation(JFrame.EXIT_ON_CLOSE);
    }

    public void actionPerformed(ActionEvent e) {
        String cmd = e.getActionCommand();
        panel.setShape(cmd);
    }

    public static void main(String[] args) {
        new Main();
    }
}
```
<img width="1012" height="710" alt="image" src="https://github.com/user-attachments/assets/51896231-7b81-4ea8-8e76-3f2ed986b762" />

## Program20
```
import javax.swing.*;
import java.awt.*;
import java.awt.event.*;
import java.util.ArrayList;

class DrawPoint {
    int x, y, size;
    Color color;

    DrawPoint(int x, int y, Color color, int size) {
        this.x = x;
        this.y = y;
        this.color = color;
        this.size = size;
    }
}

class PaintPanel extends JPanel implements MouseMotionListener {
    ArrayList<DrawPoint> points = new ArrayList<>();
    Color currentColor = Color.BLACK;
    int brushSize = 5;

    PaintPanel() {
        setBackground(Color.WHITE);
        addMouseMotionListener(this);
    }

    public void setCurrentColor(Color c) {
        currentColor = c;
    }

    public void setBrushSize(int size) {
        brushSize = size;
    }

    protected void paintComponent(Graphics g) {
        super.paintComponent(g);

        for (DrawPoint p: points) {
            g.setColor(p.color);
            g.fillOval(p.x, p.y, p.size, p.size);
        }
    }

    public void mouseDragged(MouseEvent e) {
        points.add(new DrawPoint(e.getX(), e.getY(), currentColor, brushSize));
        repaint();
    }

    public void mouseMoved(MouseEvent e) {
    }

    public void clearCanvas() {
        points.clear();
        repaint();
    }
}

//Main

public class Main extends JFrame implements ActionListener {
    JButton redBtn, blueBtn, greenBtn, blackBtn, clearBtn;
    JComboBox<String> widthBox;
    PaintPanel panel;

    Main() {
        setTitle("Paint Brush Program");
        setSize(800, 600);
        setLayout(null);

        redBtn = new JButton("Red");
        blueBtn = new JButton("Blue");
        greenBtn = new JButton("Green");
        blackBtn = new JButton("Black");
        clearBtn = new JButton("Clear");

        String widths[] = {"5", "10", "15", "20", "25"};
        widthBox = new JComboBox<>(widths);

        redBtn.setBounds(20, 20, 80, 30);
        blueBtn.setBounds(110, 20, 80, 30);
        greenBtn.setBounds(200, 20, 80, 30);
        blackBtn.setBounds(290, 20, 80, 30);
        clearBtn.setBounds(380, 20, 80, 30);
        widthBox.setBounds(480, 20, 80, 30);

        redBtn.addActionListener(this);
        blueBtn.addActionListener(this);
        greenBtn.addActionListener(this);
        blackBtn.addActionListener(this);
        clearBtn.addActionListener(this);
        widthBox.addActionListener(this);

        add(redBtn);
        add(blueBtn);
        add(greenBtn);
        add(blackBtn);
        add(clearBtn);
        add(widthBox);

        panel = new PaintPanel();
        panel.setBounds(20, 70, 740, 470);
        add(panel);

        setDefaultCloseOperation(JFrame.EXIT_ON_CLOSE);
        setVisible(true);
    }

    public void actionPerformed(ActionEvent e) {
        if (e.getSource() == redBtn) {
            panel.setCurrentColor(Color.RED);
        } else if (e.getSource() == blueBtn) {
            panel.setCurrentColor(Color.BLUE);
        } else if (e.getSource() == greenBtn) {
            panel.setCurrentColor(Color.GREEN);
        } else if (e.getSource() == blackBtn) {
            panel.setCurrentColor(Color.BLACK);
        } else if (e.getSource() == clearBtn) {
            panel.clearCanvas();
        } else if (e.getSource() == widthBox) {
            int size = Integer.parseInt((String) widthBox.getSelectedItem());
            panel.setBrushSize(size);
        }
    }

    public static void main(String[] args) {
        new Main();
    }
}
```
<img width="1228" height="755" alt="image" src="https://github.com/user-attachments/assets/2acc7dea-b38f-4ace-b845-7ccea2e1ed4d" />

## Program21
```
package mypack;

public class Add {
    public int sum(int a, int b) {
        return a + b;
    }
}
package mypack;

public class Sub {
    public int subtract(int a, int b) {
        return a - b;
    }
}
package mypack;

public class Mul {
    public int multiply(int a, int b) {
        return a * b;
    }
}
package mypack;

public class Div {
    public int divide(int a, int b) {
        return a / b;
    }
}
package mypack;

public class Square {
    public int square(int a) {
        return a * a;
    }
}

//Main Method

import mypack.*;

public class Main {
    public static void main(String[] args) {
        Add a = new Add();
        Sub s = new Sub();
        Mul m = new Mul();
        Div d = new Div();
        Square sq = new Square();

        System.out.println("Addition: " + a.sum(10, 5));
        System.out.println("Subtraction: " + s.subtract(10, 5));
        System.out.println("Multiplication: " + m.multiply(10, 5));
        System.out.println("Division: " + d.divide(10, 5));
        System.out.println("Square: " + sq.square(5));
    }
}
```

<img width="197" height="131" alt="image" src="https://github.com/user-attachments/assets/b77abf75-198f-419b-8912-c61c9941f0b4" />


## Program22
```
package mypack;

public class Add {
    public int sum(int a, int b) {
        return a + b;
    }
}
package mypack.subpack;

public class Square {
    public int square(int a) {
        return a * a;
    }
}
import mypack.Add;
import mypack.subpack.Square;

//Main

public class Main {
    public static void main(String[] args) {

        Add a = new Add();
        Square s = new Square();

        System.out.println("Addition: " + a.sum(10, 5));
        System.out.println("Square: " + s.square(5));
    }
}
```
<img width="117" height="53" alt="image" src="https://github.com/user-attachments/assets/b9ec9ad4-bb00-46e8-abf2-1e1d05658405" />

## Program23
```
public class Main {
    public static void main(String[] args) {

        try {
            int arr[] = new int[5];

            arr[0] = 10;
            arr[1] = 20;
            arr[2] = 30;
            arr[3] = 40;
            arr[4] = 50;

            System.out.println("Accessing array elements:");
            for (int i = 0; i <= 5; i++) {  
                System.out.println("Element at index " + i + " = " + arr[i]);
            }

        } catch (ArrayIndexOutOfBoundsException e) {
            System. out.println("Array Index Out Of Bounds Exception caught!");
            System. out.println("You tried to access an invalid index in the array.");
        }

        try {
            int a = 10;
            int b = 0;

            int result = a / b;  
            System.out.println("Result = " + result);

        } catch (ArithmeticException e) {
            System. out.println("Arithmetic Exception caught!");
            System. out.println("Division by zero is not allowed.");
        }

        System.out.println("Program continues after handling exceptions.");
    }
}
```
<img width="452" height="291" alt="image" src="https://github.com/user-attachments/assets/4879c69b-d826-4c32-b2e5-215b544e82f1" />

## Program24
```
class InvalidAgeException extends Exception {
    public InvalidAgeException(String message) {
        super(message);
    }
}

public class Main {

    static void checkAge(int age) throws InvalidAgeException {
        if (age < 18 || age > 25) {
            throw new InvalidAgeException("Age must be between 18 and 25.");
        } else {
            System. out.println("Valid age. Student allowed.");
        }
    }

    public static void main(String[] args) {

        int age = 16;  

        try {
            checkAge(age);
        } catch (InvalidAgeException e) {
            System. out.println("Exception caught: " + e.getMessage());
        }

        System.out.println("Program continues...");
    }
}
```
<img width="490" height="138" alt="image" src="https://github.com/user-attachments/assets/d4ea12d6-9e35-4375-b4b3-2e9d48410422" />

## Program25
```
//Character-by-Character

import java.io.*;

public class CharFileCopy {
    public static void main(String[] args) {
        try {
            FileReader fr = new FileReader("source.txt");
            FileWriter fw = new FileWriter("dest_char.txt");

            int ch;

            while ((ch = fr.read()) != -1) {
                fw.write(ch);
            }

            fr.close();
            fw.close();

            System. out.println("File copied using character stream");
        } catch (Exception e) {
            System.out.println(e);
        }
    }
}

//Byte-by-Byte

import java.io.*;

public class ByteFileCopy {
    public static void main(String[] args) {
        try {
            FileInputStream fis = new FileInputStream("source.txt");
            FileOutputStream fos = new FileOutputStream("dest_byte.txt");

            int b;

            while ((b = fis.read()) != -1) {
                fos.write(b);
            }

            fis.close();
            fos.close();

            System. out.println("File copied using byte stream");
        } catch (Exception e) {
            System.out.println(e);
        }
    }
}
```
<img width="596" height="638" alt="image" src="https://github.com/user-attachments/assets/6959fe80-f151-4c91-9eeb-a3d1471608ea" />

## Program26
```
interface Printer {
    void print();
}

abstract class Device {
    abstract void start();

    void stop() {
        System.out.println("Device stopped");
    }
}

class Computer extends Device implements Printer {
    void start() {
        System. out.println("Computer started");
    }

    public void print() {
        System.out.println("Printing from computer");
    }
}

public class Main {
    public static void main(String[] args) {
        Computer c = new Computer();
        c.start();
        c.print();
        c.stop();
    }
}
```
<img width="243" height="157" alt="image" src="https://github.com/user-attachments/assets/c5a922d3-bc7b-44ec-9554-83774dc28bad" />





































