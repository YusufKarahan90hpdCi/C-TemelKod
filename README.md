# C-TemelKod
#include<iostream>
#include<windows.h>

using namespace std;

int arac_no;

char isim[20];
char soy_isim[20];

int km;
int ilce_adres;
int yil;
int ay;

void isim_soyisim_sorgulama()
{
	cout<<"Lutfen isminizi giriniz:";
	cin>>isim;
	cout<<"Lutfen soyisminizi giriniz:";
	cin>>soy_isim;
	
}

void arac_no_sorgu()
{
	cout<<"Lutfen arac numaranizi giriniz";
	cin>>arac_no;
	switch (arac_no)
	{
		case 0 ... 100:
		cout<<"Arac Adana ilimize kayitlidir!"<<endl;
		cout<<"Lutfen bulundugunuz ilceyi giriniz!!"<<endl;
		cout<<"Saricam=1"<<endl;
		cout<<"Cukurova=2"<<endl;
		cout<<"Yuregir=3"<<endl;
		cout<<"Seyhan=4"<<endl;
		cin>>ilce_adres;
		if(ilce_adres==1)
		{
			cout<<"Aracinizi .....Mah.....Sokak.....No Saricam ADANA adresine goturunuz.";
		}
		else if(ilce_adres==2)
		{
			cout<<"Aracinizi .....Mah.....Sokak.....No Cukurova ADANA adresine goturunuz.";
		}
		else if(ilce_adres==3)
		{
			cout<<"Aracinizi .....Mah.....Sokak.....No Yuregir ADANA adresine goturunuz.";
		}
		else if(ilce_adres==4)
		{
			cout<<"Aracinizi .....Mah.....Sokak.....No Seyhan ADANA adresine götürünüz.";
		}
		break;
		case 101 ... 200:
		cout<<"Arac Ankara iline kayitlidir."<<endl;
		cout<<"Lutfen bulundugunuz ilceyi giriniz."<<endl;
		cout<<"Sincan=1"<<endl;
		cout<<"Yenimahalle=2"<<endl;
		cout<<"Kecioren=3"<<endl;
		cout<<"Etimesgut=4"<<endl;
		cin>>ilce_adres;
		if(ilce_adres==1)
		{
			cout<<"Aracinizi .....Mah.....Sokak.....No Sincan ANKARA adresine goturunuz.";
		}
		else if (ilce_adres==2)
		{
			cout<<"Aracinizi .....Mah.....Sokak.....No Yenimahalle ANKARA adresine goturunuz.";
		}
		else if(ilce_adres==3)
		{
			cout<<"Aracinizi .....Mah.....Sokak.....No Kecioren ANKARA adresine goturunuz.";
		}
		else if (ilce_adres==4)
		{
			cout<<"Aracinizi .....Mah.....Sokak.....No Etimesgut ANKARA adresine goturunuz.";
		}
		break;
		case 201 ... 300:
		cout<<"Arac Istanbul iline kayitlidir"<<endl;
		cout<<"Lutfen bulundugunuz ilceyi giriniz:"<<endl;
		cout<<"Bahcelievler=1"<<endl;
		cout<<"Kadikoy=2"<<endl;
		cout<<"Maltepe=3"<<endl;
		cout<<"Kartal=4"<<endl;
		cin>>ilce_adres;
		if(ilce_adres==1)
		{
			cout<<"Aracinizi .....Mah.....Sokak.....No Bahcelievler ISTANBUL adresine goturunuz.";
		}
		else if(ilce_adres==2)
		{
			cout<<"Aracinizi .....Mah.....Sokak.....No Kadikoy ISTANBUL adresine goturunuz.";
		}
		else if(ilce_adres==3)
		{
			cout<<"Aracinizi .....Mah.....Sokak.....No Maltepe ISTANBUL adresine goturunuz.";
		}
		else if(ilce_adres==4)
		{
			cout<<"Aracinizi .....Mah.....Sokak.....No KArtal ISTANBUL adresine goturunuz.";
		}
	
	}
	
}
void arac_tarih()
{
	cout<<"Lutfen araci aldiginiz yili giriniz:";
	cin>>yil;
	cout<<"Lutfen araci aldiginiz ayi giriniz:";
	cin>>ay;
	if(yil<2023)
	{
		cout<<"Bu tarihte ABC1 adli model uretilmistir"<<endl;
		cout<<"Araciniza uygun olan servis aglari sisteme ekleniyor."<<endl;
		cout<<"Lutfen bekleyiniz!!!!!"<<endl;
		cout<<"*************************************************************************"<<endl;
		Sleep(5000);
		
	}
	else
	{
		cout<<"Bu tarihte ABC2 adli model uretilmistir"<<endl;
		cout<<"Araciniza uygun olan servis aglari sisteme ekleniyor."<<endl;
		cout<<"Lutfen bekleyiniz!!!!!"<<endl;
		cout<<"*************************************************************************"<<endl;
		Sleep(5000);
	}
}

 void km_sorgulama()
{
	cout<<"Lutfen aracinizin onceki bakimindan bu yana gittigi mesafeyi km cinsinden giriniz:"<<endl;
	cin>>km;
	if(km>10000)
	{
		cout<<"Aracinizin servise gitmesi gereklidir.!!!!"<<endl;
		
	}
	else 
	
		cout<<"Aracinizin servise gitmesine gerek yoktur"<<endl;
	
}
	


	
int main()
{
	isim_soyisim_sorgulama();
	cout<<"Merhaba" " "<<isim<<" "<<soy_isim<< " ""sistemimize hos geldiniz. Size en iyi sekilde yardimci olabilmemiz icin lutfen bilgileri eksiksiz giriniz:"<<endl;
	
	
	km_sorgulama();
	arac_tarih();
	arac_no_sorgu();
	
	
}








