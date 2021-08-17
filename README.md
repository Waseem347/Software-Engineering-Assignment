# Software-Engineering-Assignment

#include <windows.h> #include <iostream>  using namespace std; 
 
 class employee
 { 	int   emp_number; 	char  emp_name[20]; 	float emp_basic; 	float emp_da; 	float emp_it; 	float emp_net_sal;  	public:  		void get_emp_details(); 		float find_net_salary(float basic, float da, float it); 		void show_emp_details(); };  void employee :: get_emp_details() { 	cout<<"\nEnter employee number: "; 	cin>>emp_number; 	cout<<"\nEnter employee name: "; 	cin>>emp_name; 	cout<<"\nEnter employee basic: "; 	cin>>emp_basic; 	cout<<"\nEnter employee DA: "; 	cin>>emp_da; 	cout<<"\nEnter employee IT: "; 	cin>>emp_it; }  float employee :: find_net_salary(float basic, float da, float it) {     return (basic+da)-it; }  void employee :: show_emp_details() { 	cout<<"\n\n**** Details of  Employee ****"; 	cout<<"\nEmployee Name      :  "<<emp_name; 	cout<<"\nEmployee number    :  "<<emp_number; 	cout<<"\nBasic salary       :  "<<emp_basic; 	cout<<"\nEmployee DA        :  "<<emp_da; 	cout<<"\nIncome Tax         :  "<<emp_it; 	cout<<"\nNet Salary         :  "<<find_net_salary(emp_basic, emp_da, emp_it); 	cout<<"\n-------------------------------\n\n"; }   int main() {     employee emp;          emp.get_emp_details();     emp.show_emp_details();      return 0; }


For creating an array of objects (allocating memory) you have to write down the following statements
for (int i=0; i<6; i++) {
 b[i]  = new  Box();
 // Assigning object to individual reference in the array.
}
PROGRAM
import java.util.Scanner;
 
public class Employee {
 
 int empid;
 String name;
 float salary;
 
 public void getInput() {
 
  Scanner in = new Scanner(System.in);
  System.out.print("Enter the empid :: ");
  empid = in.nextInt();
  System.out.print("Enter the name :: ");
  name = in.next();
  System.out.print("Enter the salary :: ");
  salary = in.nextFloat();
 }
 
 public void display() {
  
  System.out.println("Employee id = " + empid);
  System.out.println("Employee name = " + name);
  System.out.println("Employee salary = " + salary);
 }
 
 public static void main(String[] args) {
 
  Employee e[] = new Employee[5];
  
  for(int i=0; i<5; i++) {
   
   e[i] = new Employee();
   e[i].getInput();
  }
  
  System.out.println("**** Data Entered as below ****");
  
  for(int i=0; i<5; i++) {
   
   e[i].display();
  }
 }
}
