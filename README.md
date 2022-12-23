## Ujian Akhir Semester 

	<br>Mata Kuliah 	: Dasar Pemrograman
	<br> Nama		: Saftana Fitri
	<br>NIM		        : 1227050120
	<br>Jurusan		: [Teknik Informatika](http://if.uinsgd.ac.id/) [UIN Sunan Gunung Djati Bandung](https://uinsgd.ac.id/) 

## Deskripsi Umum

	Array adalah variable yang memiliki indeks sehingga dapat menyimpan sejumlah data yang bertipe sama. 
	Dimensi array adalah jumlah indeks pada variabel array. Array multi dimensi (lebih dari satu indeks, maksimal 7 indeks). 
	Dalam perhitungan, array sering digunakan untuk operasi matriks.
	Matriks adalah suatu susunan bilangan real atau bilangan kompleks (atau elemen-elemen) yang disusun dalam baris dan kolom sehingga membentuk jajaran persegi panjang. 
	Suatu matriks diberi nama dengan menggunakan huruf kapital seperti A, B, C, dan seterusnya, sedangkan anggotanya dinyatakan dengan huruf kecil.

## Source Code 1

	#include <iostream>
	using namespace std;
	int main() {
	  int b, k, baris, kolom, max, nilai[100][100];
	  cout << "NAMA	: SAFTANA FITRI" << endl;
	  cout << "NIM	: 1227050120" << endl;
	  cout << "==================================================" << endl;
	  cout << "==================SOAL UAS NO 1===================" << endl;
	  cout << "==================================================" << endl << endl;


	  cout << "masukkan jumlah baris matriks: ";
	  cin >> b;
	  cout << "masukkan jumlah kolom matriks: ";
	  cin >> k;
	  cout << "masukkan setiap elemen pada matriks : "<<endl;
	  for (baris = 0; baris < b; baris++) {
	    for (kolom = 0; kolom < k; kolom++) {
	      cout<< "nilai["<<baris+1<<"]["<<kolom+1<<"] : ";
	      cin >> nilai[baris][kolom];
	    }
	    cout <<endl;
	  }

	  cout << "Hasil Penukaran baris ke kolom dan kolom ke baris"<<endl;
	    cout << "==============================================="<<endl;
	  for (kolom = 0; kolom < k; kolom++) {
	    for (baris = 0; baris < b; baris++) {
	      cout << " " << nilai[baris][kolom];
	    }
	      cout <<endl;
	  }
	}
  
## Output 1
  
	NAMA    : SAFTANA FITRI
	NIM     : 1227050120
	==================================================
	==================SOAL UAS NO 1===================
	==================================================

	masukkan jumlah baris matriks: 2
	masukkan jumlah kolom matriks: 2
	masukkan setiap elemen pada matriks :
	nilai[1][1] : 1
	nilai[1][2] : 2

	nilai[2][1] : 3
	nilai[2][2] : 4

	Hasil Penukaran baris ke kolom dan kolom ke baris
	===============================================
	 1 3
	 2 4

	--------------------------------
	Process exited after 11.6 seconds with return value 0
	Press any key to continue . . .

## Source Code 2

	#include <iostream>
	using namespace std;
	int main() {
	  int b, k, baris, kolom, nilai[100][100];
	  cout << "NAMA	: SAFTANA FITRI" << endl;
	  cout << "NIM	: 1227050120" << endl;
	  cout << "==================================================" << endl;
	  cout << "==================SOAL UAS NO 2===================" << endl;
	  cout << "==================================================" << endl << endl;


	  cout << "masukkan jumlah baris matriks: ";
	  cin >> b;
	  cout << "masukkan jumlah kolom matriks: ";
	  cin >> k;
	  cout << "masukkan setiap elemen pada matriks : "<<endl;
	  for (baris = 0; baris < b; baris++) {
	    for (kolom = 0; kolom < k; kolom++) {
	      cout<< "nilai["<<baris+1<<"]["<<kolom+1<<"] : ";
	      cin >> nilai[baris][kolom];
	    }
	    cout <<endl;
	  }


	  cout << "Elemen-elemen pada matriks yang habis dibagi dengan 3,5,dan 7"<<endl;
	  cout << "============================================================="<<endl;
	 bool cek = true;

	for (baris = 0; baris < b; baris++)
	{
		for (kolom = 0; kolom < k; kolom++)
		{
			if (nilai[baris][kolom]%3==0 && nilai[baris][kolom]%5==0 && nilai[baris][kolom]%7==0)
			{
				cout << " " << nilai[baris][kolom];
				cek = false;
			}
		}
	}
	if (cek)
	{
		cout << " Nilai yang anda input tidak habis dibagi 3, 5 dan 7" <<endl;
	}
	return 0;

	}

## Output 2
  
	NAMA    : SAFTANA FITRI
	NIM     : 1227050120
	==================================================
	==================SOAL UAS NO 2===================
	==================================================

	masukkan jumlah baris matriks: 2
	masukkan jumlah kolom matriks: 2
	masukkan setiap elemen pada matriks :
	nilai[1][1] : 105
	nilai[1][2] : 468

	nilai[2][1] : 345
	nilai[2][2] : 210

	Elemen-elemen pada matriks yang habis dibagi dengan 3,5,dan 7
	=============================================================
	 105 210
	--------------------------------
	Process exited after 14.87 seconds with return value 0
	Press any key to continue . . .

