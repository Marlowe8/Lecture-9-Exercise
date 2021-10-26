# Lecture-9-Exercise

//Reverse 9 times table
		#include <iostream> 
		using namespace std;
		int main() {
			int num = 108;
			while (num != 0) {
				cout << num << endl;
				num -= 9;
			}

			return 0;
		}
	
//The Pointless Box
	#include <iostream> 
using namespace std;
int main() {
	char input;
	int counter = 0;
	while (counter !=5) {
	cout << "Only 5 attempts. Attempts Entered: " <<counter << endl;
	cout << "Enter 1 or 2 to see the message: "; cin >> input;
		if (input == '1') {
			cout << "you have entered the number 1" << endl;
			return 0;
		} else if (input == '2') {
			cout << "you have entered the number 2" << endl;
			return 0;
		}
		else {
		system("cls");
			counter++;
		}

	}

	return 0;
}


//Brute-Force Attack I
#include <iostream>
using namespace std;



int main() {

	string pw = "246";
	string inputUser;
	
	cout << "Enter Password to Enter:"; cin >> inputUser;
	while (inputUser != pw) {
		system("cls");
		cout << "Try again" << endl;
		cout << "Enter Password to Enter:"; cin >> inputUser;
		if (inputUser == pw) {
		system("cls");
		cout << "Access Granted" << endl;
		return 0;
	}
		}

	return 0;
}




//Brute-Force Attack II
#include <iostream>
using namespace std;



int main() {

	string pw = "246";
	string inputUser;
	int attempts = 1;
	while (attempts < 6) {
		cout << "Only 5 attempts" << endl;
	cout << "Enter Password to Enter:"; cin >> inputUser;
	
	if (inputUser != pw) {
		system("cls");
		cout << "Try again" << endl;
		cout << "Number of Attempts: " << attempts << endl;
		attempts++;
	}
	else if (inputUser == pw) {
		system("cls");
	cout << "Access Granted" << endl;
	return 0;
	}
	if(attempts==6) {
		system("cls");
		cout << "Number attempts exceeded ";
		return 0;
	}

	}

	return 0;
}
	
	
//Input Improvement
	#include <iostream> 
using namespace std;
int main() {
	char input;
	do {
		cout << "Would you like to Quit (Y/N)?" <<
			endl;
		cin >> input;
		if (input == 'n' || input == 'N') {
			system("cls");
			cout << "okay you don't want to quit" << endl;
		}
	} while ((input != 'Y') && (input != 'y'));
	return 0;
}
	
//Loopy
	#include <iostream> 
using namespace std;
int main() {
	int myInt;
	int counter =0;

	cout << "Enter number where the program will start to count: "; cin >> myInt;
	while (counter< myInt) {
		cout << counter + 1 << endl;
		counter++;
	}

	return 0;
}

