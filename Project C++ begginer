#include <iostream>
#include <cstdlib>
#include <math.h>
using namespace std;

bool eprim(int n)
{
	bool prim = true;
	if (n < 2)
		prim = false;
	for (int d = 2; d * d <= n; d++)
		if (n % d == 0)
			prim = false;
	return prim;
}
bool epalindrom(int n)
{
	int oglinda;  int tmpn = n;
	while (n!=0)
	{
		oglinda = oglinda * 10 + n % 10;
		n = n / 10;

	}
	if (tmpn == oglinda) return true;
	return false;

}

bool ePatrat(int numar)
{
	if ((int)sqrt(numar) == sqrt(numar))
		return true;
	return false;

}

int cmmdc(int n1, int n2)
{
	while (n1 != n2)
		if (n1 > n2)
			n1 -= n2;
		else
			n2 -= n1;
	return n1;

}
int cmmdcRec(int a, int b) {
	if (a == 0 || b == 0)
	{
		return 0;
	}
	if (a == b)
	{
		return a;
	}
	if (a > b) {
		return cmmdcRec(a - b, b);
	}
	else{
		return cmmdcRec(a, b - a);

	}
}
int cmmmc(int a, int b)
{
	int x, y;
	x = a;
	y = b;
	while (x != y)
	{
		if (x > y)
			x = x - y;
		else
			y = y - x;

	}
	return (a * b) / x;
}

int main()
{
	int opt, i, j, k, n, m;
	do
	{
		cin.clear(); fflush(stdin);
		system("cls");
		system("Color 0A");
		cout << "Main Menu" << endl;
		cout << "1. Prim Number" << endl;
		cout << "2.Palindrome Number" << endl;
		cout << "3.Perfect Square" << endl;
		cout << "4.Greatest Common Factor" << endl;
		cout << "5.The least Common Factor" << endl;
		cout << ".............................." << endl;
		cout << "End Program" << endl;
		cout << "....................." << endl;
		cin >> opt;

		switch (opt)
		{
		case 1:
			system("cls");
			system("Color 0A");
			cout << "Prim Number :" << endl;
			cout << "Give the number :" << endl;
			cin >> n;
			if (eprim(n))  cout << "The number is PRIM" << endl;
			else
				cout << "The number is not PRIM" << endl;
			cout << endl;
			system("pause");
			break;

		case 2:
			system("cls");
			system("Color 0A");
			cout << "Palindrome Number" << endl;
			cout << "Give the number :" << endl;
			cin >> n;
			if (eprim(n)) cout << "The number is palindrome" << endl;
			else
				cout << "The number is not palindrome" << endl;
			cout << endl;
			system("pause");
			break;

		case 3:
			system("cls");
			system("Color 0A");
			cout << "Perfect Square :" << endl;
			cout << "Give the number" << endl;
			cin >> n;
			if (ePatrat(n)) cout << "The number is a perfect square" << endl;
			else
				cout << "the number is not a perfect square" << endl;
			cout << endl;
			system("pause");
			break;

		case 4:
			system("cls");
			system("Color 0A");
			cout << "Greatest common factor :" << endl;
			cout << "Give the first number" << endl;
			cin >> n;
			cout << "Give the second number" << endl;
			cin >> m;
			cout << "GCF=" << cmmdc(n, m);
			cout << endl;
			system("pause");
			break;

		case 5:
			system("cls");
			system("Color 0A");
			cout << "Greatest common factor recursiv:" << endl;
			cout << "Give the first number :" << endl;
			cin >> n;
			cout << "Give the second number :" << endl;
			cin >> m;
			cout << "LCF=" << cmmdcRec(n, m);
			cout << endl;
			system("pause");
			break;


		case 6:
			system("cls");
			system("Color 0A");
			cout << "LGF" << endl;
			cout << "Give the first number :" << endl;
			cin >> n;
			cout << "Give the second number :" << endl;
			cin >> m;
			cout << "LGF=" << cmmmc(n, m);
			cout << endl;
			system("pause");
			break;

		case 0:
			cout << "Thank You for trying my program" << endl;
			system("pause");
			break;

		default:
			cout << "The option you selected is not there" << endl;
		}
	}while (opt != 0);
	return 0;



	
}


