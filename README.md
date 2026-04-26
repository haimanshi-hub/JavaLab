[Program 1: Create a class with four methods: Addition, Subtraction, Multiplication, and Division. Now, test all four methods in the public static void main. ](#Program1)



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


## code-3
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


## code-4
```
