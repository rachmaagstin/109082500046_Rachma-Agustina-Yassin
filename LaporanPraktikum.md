# <h1 align="center">Laporan Praktikum Modul 2 - REVIEW ALGORITMA DAN PEMROGRAMAN 1 </h1>
<p align="center">Rachma Agustina Yassin - 109082500046</p>

## Unguided 

### 1. Telusuri program berikut dengan cara mengkompilasi dan mengeksekusi program. Silakan masukan data yang sesuai sebanyak yang diminta program. Perhatikan keluaran yang diperoleh. Coba terangkan apa sebenarnya yang dilakukan program tersebut?
#### soal1.go

```go
package main

import "fmt"

func main() {
var (
	satu, dua, tiga string
	temp string
	)

	fmt.Print("Masukan input string: ")
	fmt.Scanln(&satu)
	fmt.Print("Masukan input string: ")
	fmt.Scanln(&dua)
	fmt.Print("Masukan input string: ")
	fmt.Scanln(&tiga)
	fmt.Println("Output awal = " + satu + " " + dua + " " + tiga)
	temp = satu
	satu = dua
	dua = tiga
	tiga = temp
	fmt.Println("Output akhir = " + satu + " " + dua + " " + tiga)
}
```
### Output Unguided :

##### Output 
![Screenshot Output Unguided 1_1](https://github.com/rachmaagstin/109082500046_Rachma-Agustina-Yassin/blob/main/MODUL 2/output/output-no1.png)
Program tersebut digunakan untuk menerima tiga input string dari pengguna, kemudian menampilkan urutan nilai sebelum dan sesudah dilakukan pertukaran. Nilai dari variabel satu, dua, dan tiga ditukar menggunakan variabel sementara temp. Proses pertukaran nilai variabel dengan cara memindahkan nilai variabel satu ke variabel temp, kemudian nilai variabel dua dipindahkan ke variabel satu, nilai variabel tiga dipindahkan ke variabel dua, dan nilai variabel yang disimpan di variabel temp dipindahkan ke variabel tiga. Proses ini menghasilkan perubahan urutan secara rotasi, sehingga nilai yang awalnya pertama menjadi terakhir. Program kemudian menampilkan hasil akhir setelah pertukaran nilai dilakukan.