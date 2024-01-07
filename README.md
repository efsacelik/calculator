# calculator
Calculates the situation of two numbers.
package patikaAcademy;

import java.util.Scanner;

public class calculator {

	public static void main(String[] args) {
		int n1, n2, selection;
		
		Scanner input= new Scanner(System.in);
		
		System.out.println("Enter the first number:");
		n1 = input.nextInt();
		
		System.out.println("Enter the second number:");
		n2 = input.nextInt();
		
		System.out.println("1- Toplama\n1-Çıkarma\n3-Çarpma\n4-Bölme");
		System.out.println("Make a selection:");
		selection=input.nextInt();
		
		
		switch (selection) {
		case 1: {
			System.out.println(n1+n2);
			break;
		}
		case 2: {
			System.out.println(n1-n2);
			break;
		}
		case 3: {
			System.out.println(n1*n2);
			break;
		}
		case 4: {
			switch (n2) {
			  case 0:
				  System.out.println("Invalid choice, please try again");
				break;
			default:
				  System.out.println(n1/n2);
			}break;
		}
		default:
			System.out.println("Invalid choice, please try again.");
			
		}
		
	}

}
