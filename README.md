//# Lecture-11
//Execute issue
#include <iostream>
#include <array>
#include <string>
#include <math.h>
using namespace std;

int main() {
	int y;
	cout << "Enter a number you want the table of:" << endl;
	cin >> y;
	while (cin.fail()){
		cin.clear();
		cin.ignore(1000, '\n');
		cout << "Invalid command enter the number again:" << endl;
		cin >> y;
	}
	for (int x = 0; x <= 10; x++) {
		cout << y << " x " << x << "=" << y * x << endl;
	}
}
//Exercise 2
#include <iostream>
#include <array>
#include <string>
#include <math.h>
using namespace std;

int main() {
	for (int i = 5; i >= 1; i--) {
		for (int c = 1; c <= i; c++) {
			cout << "*";
		}
		cout << endl;
	}
	return 0;
}
//Exercise 3   
#include <iostream>
#include <string>
#include <iomanip>
#include <array>

using namespace std;

int main() {

	for (int i = 1; i <= 5; i++) {
		for (int c = i; c <= 5; c++)
		{
			cout << '*';
		}
		cout << endl;
	}
	return 0;
} 
//Exercise 4
#include <iostream>
#include <string>
#include <iomanip>
#include <array>

using namespace std;

int main() {

	for (int i = 1; i <= 5; i++) {
		for (int c = i; c <= 5; c++)
		{
			cout << '*';
		}
		cout << endl;
	}
	for (int i = 1; i <= 5; i++) {
		for (int c = 1; c <= i; c++)
		{
			cout << '*';
		}
		cout << endl;
	}
	return 0;
}
//Factorial
#include <iostream>
#include <string>
#include <iomanip>
#include <array>

using namespace std;

int main() {

	long double f = 1, i , number;
	cout << "Enter a number: ";
	cin >> number;
	while (cin.fail())
	{
		cin.clear();
		cin.ignore(1000, '\n');
		cout << "Invalid Input, Try again\nEnter a number: ";
		cin >> number;
	}
	for (i = 1; i <= number; i++) {
		f = f * i;
	}
	cout << "Factorial of " << number << " is " << f;
	return 0;
} 
//For Multiplication Table                                                
#include <iostream>

using namespace std;

int main()
{
	int userInp;
	cout << "Write a number to print the table of it: " << endl;
	cin >> userInp;
	if(cin.fail()){		
		cout << "Invalid Input" << endl; 
		return 0;
	}
	for (int i = 1; i < 11; i++) {
		cout << userInp << " * " << i << " = " << userInp * i << endl;
	}
	return 0;
}
//While Multiplication Table                                                                 
#include <iostream>
using namespace std;

int main() {
	int userInp;
	cout << "Write a number to print the table of it: ";
	cin >> userInp;
	if (cin.fail()) {
		cout << "Invalid Input!";
		return 0;
	}
	int i = 1;
	while (i < 11) {
		cout << userInp << " * " << i << " = " << userInp * i << endl;
		i++;
	}
	return 0;
} 
//For Loop
#include <iostream>
using namespace std;

int main(){

	int userInp1;
	int userInp2;

	cout << "Enter the number you want table of: ";
	cin >> userInp1;
	if (cin.fail()) {
		cout << "Invalid Input" << endl;
		return 0;
	}
	cout << "Enter till what number the table should end: ";
	cin >> userInp2;
	if (cin.fail()) {
		cout << "Invalid Input" << endl;
		return 0;
	}
	for (int i = 1; i < userInp2 + 1; i++){
		cout << userInp1 << " * " << i << " = " << userInp1 * i << endl;
	}
	return 0;
}                                                                 
//Find 9s
#include <iostream>
#include <string>
#include <iomanip>
#include <array>

using namespace std;

int main() {
	int sum = 0;
	for (int i = 0; i <= 200; i++) {		
		if (i % 9 == 0)
		{
			cout << i << " Divided 9 = " << i / 9 << endl;
			sum = sum + i;
			
		}	
	}
	cout << "\nThe sum of all the integers that are divisible by 9 are = " << sum << endl;
	return 0;
}                                                   
