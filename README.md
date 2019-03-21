# Unique-Calculator

#include <iostream>
#include <cmath>
using namespace std;


// Present list of options for the user to choose from that are all connected to a switch statement


int main()
{
	int choice;
	bool gameOn = true;
	while (gameOn != false){
	cout << "	M E N U \n";
	cout << " 1 - Calculate Square Root\n";
	cout << " 2 - Calculate Cube\n";
	cout << " 3 - Calculate Natural Logarithm\n";
	cout << " 4 - Calculate Inverse\n";
	cout << " 5 - Calculate Absolute Value\n ";
	cout << "0 - Exit Program\n";

	cin >> choice;


// Each case is connected to each cout input that the user enters


	switch (choice)
{

		
	case 1:
		cout <<"Please enter a floating number!";
		double inputnumber;
		cin >> inputnumber;
		cout <<"The square of " << inputnumber << " is " << sqrt(inputnumber) << endl; 
		break;
		
	case 2:
		cout <<"Please enter a floating number!";
		cin >> inputnumber;
		cout << inputnumber << " raised to the third power is " << pow(inputnumber,3) << endl;
		
		break;
	
	case 3:
		cout << "Please enter a floating number!";
		cin >> inputnumber;
		cout << "The natural log of " << inputnumber << " is " << log(inputnumber) << endl;
		break;
	
	case 4:
		cout << "Please enter a floating number!";
		cin >> inputnumber;
		cout << "The inverse of " << inputnumber << " is " << 1.0/inputnumber << endl;
		break;

	case 5:
		cout << "Please enter a floating number!";
		cin >> inputnumber;
		cout << "The absolute value of " << inputnumber << " is " << fabs(inputnumber) << endl;
		
		break;
		
	case 0:
		cout <<"Exiting Program.\n";
		gameOn = false;
		break;


// Prompt the user to enter a valid input if the one they entered is incorrect or can not be read


default:		
cout << "Not a Valid Choice. \n";
cout << "Choose again.\n";
cin >> choice;
break;
}

}
return 0;
}
