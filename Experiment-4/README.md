## Experiment-4a
## Title :Implement Single Inheritance
## Source code:
``` java
class Person {
   String name;
   int age;
   Person(String name,int age) {
     this.name = name;
     this.age = age;
   }
   void displayPersonDetails() {
     System.out.println("Name: "+name);
     System.out.println("Age: "+age);
   }
 }
 class Employee extends Person {
   double annualSalary;
   int yearOfJoining;
   String nationalInsuranceNumber;

   Employee(String name,int age,double annualSalary,int yearOfJoining,String nationalInsuranceNumber) {
     super(name,age);
     this.annualSalary = annualSalary;
     this.yearOfJoining = yearOfJoining;
     this.nationalInsuranceNumber = nationalInsuranceNumber;
   }
   void displayEmployeeDetails() {
     displayPersonDetails();
     System.out.println("AnnualSalary: "+annualSalary);
     System.out.println("YearOfJoining: "+yearOfJoining);
     System.out.println("NationalInsuranceNumber: "+nationalInsuranceNumber);
   }
}
class Main {
   public static void main(String args[]) {
     Employee emp = new Employee("Suvarna",28,55000.0,2026,"NI122345");
     emp.displayEmployeeDetails();
  }
}
```
## Output:
![Exp-4a Output](exp4a.png)

                              
