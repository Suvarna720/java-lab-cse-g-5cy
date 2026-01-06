# Add Experiment-2
## Title:Find the sum of first Fibonacci Numbers
## Source code:
``` java
class Fibonacci {
    int a=0,b=1,c,n;
    int sum=0;
    Fibonacci(int n) {
        this.n=n;
    }
    void printFib() {
        for(int i=1;i<=n;i++) {
            if (i==1)
                c=a;
            else if (i==2)
                c=b;
            else {
                c=a+b;
                a=b;
                b=c;
            }
            sum+=c;
            if (i==n)
                System.out.print(c + ".");
            else
                System.out.print(c + ",");
      }
    }
    int getSum(){
        return sum;
    }
  }
import java.util.Scanner;
class Main {
    public static void main(String[] args) {
        Scanner sc = new Scanner(System.in);
        System.out.print("\nenter no.of Fibonacis terms:");
        int n = sc.nextInt();
        if(n>0){
        Fibonacci f = new Fibonacci(n);
        System.out.println("Fibnacci series are:");
        f.printFib();
        System.out.println("\nThe sum of Fibonacis series: " + f.getSum());
        }
        else{
            System.out.println("Fibonacci sequence and sum can not be calculated");
        }
   }
}
```
## Output:
![ADDEXP-2 Output](Fib.png)
