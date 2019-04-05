#include <iostream>
using namespace std;

class segi{
protected:
	double alas, tinggi;
public:
	void set (double a, double t){
		alas=a; tinggi=t;
	}
	void menu(){
		cout<<"SELAMAT DATANG DI MESIN PENGHITUNG LUAS"<<endl;
		cout<<"1. Luas persigi empat"<<endl;
		cout<<"2. Luas segitiga"<<endl;
		cout<<"Masukkan Pilihan : ";
	}
};

class cetak{
public:
	void output (double i){
		cout << i << endl;
	}
};

class Persegi: public segi, public cetak{
public:
	double hit (){
		return (alas * tinggi);
	}
};

class Segitiga: public segi, public cetak{
public:
	double hit (){
	return (alas * tinggi / 2);
	}
};

int main (){
awal:
	segi menu;
	int pilihan;
	Persegi segi4;
	Segitiga segi3;
	menu.menu();
	cin>>pilihan;
	if(pilihan==1){
		double p,l;
		cout<<"Masukkan panjang : ";cin>>p;
		cout<<"Masukkan lebar : ";cin>>l;
		segi4.set (p,l);
		cout<<"Luas persegi  : " ;
		segi4.output (segi4.hit());
		cout<<"Masih mau menghitung lagi ?(y/n) : ";
		char opsi;cin>>opsi;
		if(opsi=='y'||opsi=='Y'){
			system("CLS");
			goto awal;
		}
		else cout<<"TERIMA KASIH"<<endl;
	}
	else if(pilihan==2){
		double a,l;
		cout<<"Masukkan alas : ";cin>>a;
		cout<<"Masukkan tinggi : ";cin>>l;
		segi3.set (a,l);
		cout<<"Luas segitiga : ";
		segi3.output (segi3.hit());
		cout<<"Masih mau menghitung lagi ?(y/n) : ";
		char opsi;cin>>opsi;
		if(opsi=='y'||opsi=='Y'){
			system("CLS");
			goto awal;
		}
		else cout<<"TERIMA KASIH"<<endl;
	}
	else cout<<"TERIMA KASIH"<<endl;
}
