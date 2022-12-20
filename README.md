#ujian semester 
<br>mata kuliah  : dasar pemrograman
<br>nama         : adil zukhruf firdaus
<br>nim          : 1227050005
<br>jurusan      : [Teknik Informatika](http://if.uinsgd.ac.id/) [UIN Sunan Gunung Djati Bandung](https://uinsgd.ac.id/) 

## deskripsi umum
membuat array menggunakan bahasa c++,input banyak baris dan banyak kolom array dimensi 2 dan isi dengan nilai, di ubah baris menjadi kolom, kolom menjadi baris.

## source code
#include <iostream>
using namespace std;

int main(){
	int i, j, b, k, matriks[20][20], transpose[20][20];
  
  cout << "adil zukhruf firdaus \n";
  cout << "1227050005 \n";
  cout << "UAS NOMOR 1 DASAR PEMROGRAMAN (Transpose matriks)\n";
  cout << "========================================= \n\n";

  cout << "Masukkan jumlah baris matriks: ";
  cin >> b;
  cout << "Masukkan jumlah kolom matriks: ";
  cin >> k;
  cout << endl;

  cout << "Masukkan elemen matriks \n";
  for (i = 0; i < b; i++) {
    for (j = 0; j < k; j++) {
      cout << "Nilai baris ke-" << i+1 << " kolom ke-" << j+1 << " = " ;
	  cin  >> matriks[i][j];
    }
  }
  cout << "\n";

  cout << "Matriks pertama : \n";
  for (i = 0; i < b; i++){
    for (j = 0; j < k; j++){
      cout << matriks[i][j] << "\t";
    }
    cout << endl;
  }
  
  
  for (i = 0; i < b; i++){
    for (j = 0; j < k; j++){
      transpose[j][i] = matriks[i][j];
    }
  }

  cout << "Hasil Matriks (Transpose): \n";
  for (i = 0; i < k; i++){
    for (j = 0; j < b; j++){
      cout << transpose[i][j] << "\t";
    }
    cout << endl;
  }
}

## output
![Screenshot (2)](https://user-images.githubusercontent.com/121107393/208690663-e76173e5-4c3d-45ea-b856-008eaffe4961.png)
