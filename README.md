# Praktikum6

### Name   :   Azhyka Rizki Ramadhan
### NIM     :   312110469
### Class   :   TI.22.A3

# Tugas Bahasa Pemrograman 


## Latihan 1


<p> This is the program code <p>

```python
import math

a = lambda x: x ** 2
print(a(46))

b = lambda x,y: x**2 + y**2
print(b(4,6))

c = lambda *args : sum(args)/len(args)
print(c(5,7,9,11,10))

d = lambda s: "".join(set(s))
print(d("Tertimpa")) 
```


<p> The output will be like this <p>

<img width="194" alt="salah" src="https://user-images.githubusercontent.com/118233561/205201377-f86383ee-f2bf-424a-84a3-befb2eaa36c0.png">



## Tugas Praktikum
<img width="554" alt="3" src="https://user-images.githubusercontent.com/118233561/204752446-3289e1d2-7395-4f23-810c-eaa1c4c8323b.png">

<p> This is the program code <p>

```python
x = {}

def tambah():
    print("Tambah Data")
    nama = input("Masukkan Nama Mahasiswa   : ")
    nim = input("Masukkan NIM              : ")
    tugas = int(input("Masukkan Nilai Tugas      : "))
    uts = int(input("Masukkan Nilai UTS        : "))
    uas = int(input("Masukkan Nilai UAS        : "))
    akhir = tugas * 30/100 + uts * 35/100 + uas * 35/100
    x[nama] = nim , tugas, uts , uas , akhir
def tampilkan():
    if x.items():
        print("---------------------------------------------------------------------------------")
        print("\n                               DAFTAR NILAI MAHASISWA                    ")
        print("---------------------------------------------------------------------------------")
        print("| No |      Nama      |     NIM     |  Tugas  |   UTS   |   UAS   |    Akhir    |")
        print("---------------------------------------------------------------------------------")
        i = 0                                                                         
        for b in x.items():                                                             
             i += 1
             print("| {no:2d} | {0:14s} | {1:11s} | {2:7d} | {3:7d} | {4:7d} | {5:7f}   |"
                . format ( b [ 0 ][: 14 ], b [ 1 ][ 0 ], b [ 1 ][ 1 ], b [ 1 ][ 2 ], b [ 1 ][ 3 ], b [ 1 ][ 4 ] , no = i ))
        print("---------------------------------------------------------------------------------")
    else :
        print("---------------------------------------------------------------------------------")
        print("\n                               DAFTAR NILAI MAHASISWA                    ")
        print("---------------------------------------------------------------------------------")
        print("| No |      Nama      |     NIM     |  Tugas  |   UTS   |   UAS   |    Akhir    |")
        print("---------------------------------------------------------------------------------")
        print("|                                TIDAK ADA DATA                                 |")
        print("---------------------------------------------------------------------------------")
def hapus():
    print ( "Hapus Data" )
    nama = input("Masukkan Nama Mahasiswa   : ")
    if  nama in  x . keys ():
        del  x [ nama ]
    else :
        print ( "Nama {0} Tidak Ditemukan" . format ( nama ))
def ubah():
    print ( "Ubah Data" )
    nama = input("Masukkan Nama Mahasiswa   : ")
    if nama in  x . keys ():
        nim = input("Masukkan NIM              : ")
        tugas = int(input("Masukkan Nilai Tugas      : "))
        uts = int(input("Masukkan Nilai UTS        : "))
        uas = int(input("Masukkan Nilai UAS        : "))
        akhir = tugas * 30/100 + uts * 35/100 + uas * 35/100
        x[nama] = nim , tugas, uts , uas , akhir
    else :
        print ( "Nama{0} Tidak Ditemukan" . format(nama ))

while True:
    print("")
    print("===========================")
    print("|   Program Input Nilai   |")
    print("===========================")
    c = input("L)ihat, T)ambah, U)bah, H)apus, K)eluar: ")
    if c.lower() == "l":
        tampilkan()
    elif c.lower() == "t":
        tambah()
    elif c.lower() == "u":
        ubah()
    elif c.lower() == "h":
        hapus()
    elif c.lower() == "k":
        print()
        print("---------------------------------------------------------------------------------")
        print("                                 PROGRAM TELAH SELESAI                    ")
        print("---------------------------------------------------------------------------------")
        break

    else:
        print()
        print("Kode yang anda masukkan salah!")
```


<p> Run and the option like this will pop up <p>
<img width="253" alt="Screenshot 2022-11-30 160214" src="https://user-images.githubusercontent.com/118233561/204752806-a0d9bd9b-c788-4aa3-84a6-d4ed996c5aca.png">

<p> then click the font you want to use <p>
<p> L = for see/show data <p>
<p> T = for added data <p>
<p> U = for change data <p>
<p> H = for remove data <p>
<p> K = for close the program <p>

### T)ambah
<p> Click t, and then input the data. for example input 2 data <p>
<img width="310" alt="4" src="https://user-images.githubusercontent.com/118233561/204754398-ea5e5f4c-91c1-4827-b1a9-cff251daf3eb.png">


### L)ihat
<p> click l to show the data you just input <p>
<img width="502" alt="5" src="https://user-images.githubusercontent.com/118233561/204754667-038df8b1-e363-48e4-955c-5a1fbe3c4938.png">


### U)bah
<p> Click u and the choose which one you want to change the <p>
<img width="527" alt="6" src="https://user-images.githubusercontent.com/118233561/204758347-a1ec792b-f022-4950-8961-8ca95d332fcb.png">



### H)apus
<p> Click h and the write which data you want to remove <p>

<img width="506" alt="7" src="https://user-images.githubusercontent.com/118233561/204758767-e8d35b63-366b-45c7-a768-969766fa26b2.png">


### K)eluar
  
<p> Click k if you want to ended the program <p>
  
<img width="495" alt="8" src="https://user-images.githubusercontent.com/118233561/204759254-4afe3e68-c0e0-44f8-8de2-51f1671645f2.png">
