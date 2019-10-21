# GPA_CALCULATOR
This is a program to calculate the GPA of a student 
// GPA_CALCULATOR.cpp : This file contains the 'main' function. Program execution begins and ends there.
//

#include <iostream>
#include <string>
using namespace std;

int main()
{

	string name, major;
	char courseA, courseB, courseC, courseD, courseE;
	double GPA_Course1=0, GPA_Course2=0, GPA_Course3=0, GPA_Course4=0, GPA_Course5=0;
	//int GPACourse1.... 
	double average;
	cout << "Enter student name: ";
	getline(cin, name);
	cout << "Enter student major ";
	getline(cin, major);
	cout << "Please take not you can only input A,B,C,D,E,F \n";
	cout << "Please input a grade for courseA: ";
	cin >> courseA;
	
	cout << "Please input a grade for courseB: ";
	cin >> courseB;
	cout << "Please input a grade for courseC: ";
	cin >> courseC;
	cout << "Please input a grade for courseD: ";
	cin >> courseD;
	cout << "Please input a grade for courseE: ";
	cin >> courseE;

	if (courseA == 'A' || courseA == 'a') 
		GPA_Course1 = 4.0;
	else if (courseA == 'B' || courseA == 'b')
		GPA_Course1 = 3.0;
	else if (courseA == 'C' || courseA == 'c')
		GPA_Course1 = 2.0;
	else if (courseA == 'D' || courseA == 'd')
		GPA_Course1 = 1.0;
	else if (courseA == 'F' || courseA == 'f')
		GPA_Course1 = 0.0;

	
	if (courseB == 'A' || courseB == 'a')
		GPA_Course2 = 4.0;
	else if (courseB == 'B' || courseB == 'b')
		GPA_Course2 = 3.0;
	else if (courseB == 'C' || courseB == 'c')
		GPA_Course2 = 2.0;
	else if (courseB == 'D' || courseB == 'd')
		GPA_Course2 = 1.0;
	else if (courseB == 'F' || courseB == 'f')
		GPA_Course2 = 0.0;

	if (courseC == 'A' || courseC == 'a')
		GPA_Course3 = 4.0;
	else if (courseC == 'B' || courseC == 'b')
		GPA_Course3 = 3.0;
	else if (courseC == 'C' || courseC == 'c')
		GPA_Course3 = 2.0;
	else if (courseC == 'D' || courseC == 'd')
		GPA_Course3 = 1.0;
	else if (courseC == 'F' || courseC == 'f')
		GPA_Course3 = 0.0;

	if (courseA == 'A' || courseA == 'a')
		GPA_Course4 = 4.0;
	else if (courseD == 'B' || courseD == 'b')
		GPA_Course4 = 3.0;
	else if (courseD == 'C' || courseD == 'c')
		GPA_Course4 = 2.0;
	else if (courseD == 'D' || courseD == 'd')
		GPA_Course4 = 1.0;
	else if (courseD == 'F' || courseD == 'f')
		GPA_Course4 = 0.0;

	if (courseE == 'A' || courseE == 'a')
		GPA_Course5 = 4.0;
	else if (courseE == 'B' || courseE == 'b')
		GPA_Course5 = 3.0;
	else if (courseE == 'C' || courseE == 'c')
		GPA_Course5 = 2.0;
	else if (courseE == 'D' || courseE == 'd')
		GPA_Course5 = 1.0;
	else if (courseE == 'F' || courseE == 'f')
		GPA_Course5 = 0.0;




	//caculate the average GPA of the student GPAcourseA+... 
	average = (GPA_Course1 + GPA_Course2 + GPA_Course3 + GPA_Course4 + GPA_Course5) / 5;

	cout << "My name is " << name << endl;
	cout << "My major is " << major << endl;
	cout << courseA << endl;
	cout << courseB << endl;
	cout << courseC << endl;
	cout << courseD << endl;
	cout << courseE << endl;
	cout << "My final GPA for this Semester is " << average << endl;

	return 0;
}
