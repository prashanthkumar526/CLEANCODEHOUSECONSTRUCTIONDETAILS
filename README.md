# CLEANCODEHOUSECONSTRUCTIONDETAILS
import java.util.Scanner;
import java.io.IOException;
import java.io.PrintStream;
import java.io.FileDescriptor;
import java.io.FileOutputStream;
class Material
{
Material()
{
double Total_cost;
Scanner sc=new Scanner(System.in);
PrintStream myoutput=new PrintStream(new FileOutputStream(FileDescriptor.out));
myoutput.print("HOUSE CONSTRUCTION CALCULATOR \n");
myoutput.print("<<<<<<<<<<<<<<<<<<**************************>>>>>>>>>>>>>>>>>> \n");
System.out.printf("different requirements needed \n");
System.out.printf("***************************************** \n");
System.out.printf("1.Standard material costs 1200 INR per square feet \n");
System.out.printf("2.Above standard material costs 1500 INR per square feet\n");
System.out.printf("3.High standard material costs 1800 INR per square feet\n");
System.out.printf("4.High standard material with full Automated house costs 2500 INR per square feet\n");
System.out.printf("<<-------------------**********************-------------------------->> \n");
System.out.format("%S","Enter your choice for ur house construction standard material\n");
int MaterialChoosen=sc.nextInt();
System.out.format("%S","Enter Total Area Of House In Square Feet \n");
double TotalArea=sc.nextDouble();
switch(MaterialChoosen)
{
case 1:Total_cost=TotalArea*1200;
       myoutput.print("Total cost of construction of house with standard material is:" +Total_cost+"INR");
       break;
case 2:Total_cost=TotalArea*1500;
       myoutput.print("Total cost of construction of house with above standard material is:" +Total_cost+"INR");
       break;
case 3:Total_cost=TotalArea*1800;
       myoutput.print("Total cost of construction of house with high standard material is:" +Total_cost+"INR");
       break;
case 4:Total_cost=TotalArea*2500;
       myoutput.print("Total cost of construction of house with high standard and fully automated material is:" +Total_cost+"INR");
       break;
default:myoutput.print("choose a valid number of  choice");
}
}
}

class HouseConstructionCost
{
public static void main(String[] args) 
{
Material material=new Material();
}
}
