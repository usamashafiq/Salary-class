#include<iostream>
#include<conio.h>
using namespace std;
class sale {
private:
	double sal[12];

public:
	void getsale();
	void sum();
	void print();

};
void sale::getsale() {

	cout << "Enter a sale of 12 month" << endl;
	for (int i = 0; i <= 12; i++) {

		cin >> sal[i];
	}
}
void sale::sum() {
	double sum = 0;
	for (int i = 0; i <= 12; i++) {
		sum = sum + sal[i];

	}
	cout << endl << "Total sale of year : " << sum << endl;
}

void sale::print() {
	cout << "sale of 12 month" << endl;
	for (int i = 0; i <= 11; i++) {
		cout << "sale of month " << i + 1 << " :- " << sal[i] << endl;
	}



}
void main() {
	sale s;
	int a;
	cout << "enter you want to show sale" << endl;

	cin >> a;
	for (int i = 0; i < a; i++) {
		s.getsale();
		s.sum();
		s.print();
	}



	_getch();

}
