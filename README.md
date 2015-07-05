//# Object-creation

//Here is a simple program which tell you how to create a object

package labexercise;

import java.util.*;

public class ObjectCreation {

	Scanner s=new Scanner(System.in);//default class present in util package to get input from user

	int Rollno;

	String Name;

	public void getinput()

	{

		System.out.print("Please Enter The Name : ");

		Name = s.nextLine();

		System.out.print("Please Enter The RollNo : ");

		Rollno = s.nextInt();

	}

	public void display()

	{

		System.out.println("Name :"+Name+"\tRollno :"+Rollno);

	}

	public static void main(String[] args) {

		ObjectCreation obj=new ObjectCreation();//Object creation using new key word

		obj.getinput();

		obj.display();

		System.out.println(obj.getClass());/*This getclass() method is present in ObjectCreation class parent class that is Object class method where object class is the supermost class in java*/

	}

}

OUTPUT:

Please Enter The Name : Surendar

Please Enter The RollNo : 1011

Name :Surendar	Rollno :1011

class labexercise.ObjectCreation

