# Lecture-9-Exercise

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
