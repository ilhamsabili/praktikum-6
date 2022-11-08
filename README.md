# praktikum-6
Nama  : ilham sabili

NIM   : 312210120

Kelas : TI.22.A1

# KONDISI DAN PERULANGAN
## Lab 2 Struktur Kondisi
### Latihan 1
- Buat program sederhana dengan input 2 buah bilangan, kemudian tentukan bilangan terbesar dari kedua bilangan tersebut menggunakan statement if!

Langkah - langkah :
1. Buat programnya terlebih dahulu seperti gambar di bawah ini

![Screenshot (122)](https://user-images.githubusercontent.com/115867244/200478078-acaa52f6-d7f3-4ec2-b2ef-f44bb852c417.png)

    # menentukan bilangan
    print('Menentukan bilangan terbesar dari 2 bilangan')
    a = int(input("Masukkan nilai A:"))
    b = int(input("Masukkan nilai B:"))
    if a > b:
        print("A =", a, "yang terbesar")
    elif b > a:
        print("B=", b, "yang terbesar")

2. Hasil Run

![Screenshot (123)](https://user-images.githubusercontent.com/115867244/200478559-901e370f-0707-486d-b6b5-fc58d4ed5995.png)

### Latihan 2
- Buat program untuk mengurutkan data berdasarkan input sejumlah data (minimal 3 variable input atau lebih), kemudian tampilkan hasilnya secara berurutan mulai dari data terkecil.

Langkah - langkah :
1. Buat programnya terlebih dahulu seperti gambar di bawah ini

![Screenshot (124)](https://user-images.githubusercontent.com/115867244/200478742-fb61dba1-81b5-4302-87b7-ff744fc68794.png)

    print("____Mengurutkan bilangan dari yang terkecil ke yang terbesar____")
    print("Masukan 3 bilangan yang akan diurutkan:")
    a = int(input("masukkan bilangan 1 = "))
    b = int(input("masukkan bilangan 2 = "))
    c = int(input("masukkan bilangan 3 = "))

    if a < b and a < c:
        if b < c:
            print(a, b, c)
        else:
            print(a, c, b)
    elif b < a and b < c:
        if a < c:
            print(b, a, c)
        else:
            print(b, c, a)
    else:
        if a < b:
            print(c, a, b)
        else:
            print(c, b, a)
   
2. Hasil Run

![Screenshot (125)](https://user-images.githubusercontent.com/115867244/200479775-4cae9b30-ad47-406e-af7a-0d1d6fa395ac.png)

## Lab 3 Perulangan
### Latihan 1
- Buat program dengan perulangan bertingkat (nested) for yang menghasilkan output sebagai berikut :
![200156779-cc2eb0c1-293c-4089-84d8-7dde04482340](https://user-images.githubusercontent.com/115867244/200480989-caa9329c-1335-4259-9909-4c070b4d00b4.png)

Langkah - langkah :
1. Buat programnya terlebih dahulu seperti gambar di bawah ini

![Screenshot (126)](https://user-images.githubusercontent.com/115867244/200481158-8bcc8050-0ac7-45b0-a5ee-4d97f593be68.png)

    for i in range(0,10):
        print()
        print(i, end="\t")
        for j in range(1,10):
            print(i+j,end="\t")
            
2. Hasil Run

![Screenshot (127)](https://user-images.githubusercontent.com/115867244/200481338-6abe3ab5-beb8-4600-a7c9-42b6ddb4dda6.png)

### Latihan 2
- Tampilkan n bilangan acak yang lebih kecil dari 0.5.

- Nilai n diisi pada saat runtime

- Anda bisa menggunakan kombinasi while dan for untuk menyelesaikannya

Langkah - langkah :
1. Buatlah programnya terlebih dahulu seperti gambar dibawah ini

![Screenshot (128)](https://user-images.githubusercontent.com/115867244/200481757-1e7fcca4-4d42-456a-ab1d-4e73447b7dce.png)

    from random import random

    n = int(input("Masukan Beberapa perulangan : "))
    while n == n:
        break
    for i in range(n):
        bil = random() % 0.5
        print("Perulangan ke : ", bil)
2. Hasil Run

![Screenshot (129)](https://user-images.githubusercontent.com/115867244/200481882-f8e903c0-3b5a-4c74-bc51-ec68cab9b308.png)

# MODUL PRAKTIKUM 2 DAN 3
## Labpy2 dan Labpy3
### Labpy2
- Buat program sederhana dengan input tiga buah bilangan, dari ketiga bilangan tersebut tampilkan bilangan terbesarnya. Gunakan statement if.

Langkah - langkah :

1. Buatlah flowchart dari mencari angka terbesar dari 3 bilangan seperti gambar dibawah ini

![200159462-6b7e6bcb-8a43-4d48-a4c4-5bf8bda85a42](https://user-images.githubusercontent.com/115867244/200482321-1f6c21a7-2288-4347-8d52-f7d50f20dcc1.png)

2. Buatlah program codenya seperti gambar dibawah ini

![Screenshot (130)](https://user-images.githubusercontent.com/115867244/200482425-a7e9b85f-7de4-41df-bb6c-9b2698a2e546.png)

    a, b, c = (
        int(input('Masukkan nilai a: ')),
        int(input('Masukkan nilai b: ')),
        int(input('Masukkan nilai c: '))
    )
    if a > b and a > c:
        print('A yang terbesar')
    elif b > a and b > c:
        print('B yang terbesar')
    else:
        print('C yang terbesar')
        
3. Hasil Run

![Screenshot (131)](https://user-images.githubusercontent.com/115867244/200482639-0bb7a2d5-4c01-442a-bdf0-736076e77365.png)

## Labpy3
### Latihan 1
Flowchart latihan 1

![200159707-ccb1abdb-be69-4849-96c8-6c02c439d199](https://user-images.githubusercontent.com/115867244/200483087-8c454d84-e476-4dd7-96a1-591ed611c4bf.png)

### Algoritma latihan 1
Menampilkan n bilangan acak yang lebih kecil dari 0,5, nilai n diisi pada saat runtime.

1. Memasukan/ import fungsi RANDOM terlebih dahulu

2. Deklarasi integer , masukkan jumlah n :

3. Memasukan deskripsi kombinasi for untuk menyelesaikannya.

4. Memasukan nilai jumlah (n) : 5

5. Mencetak data ke 1 sampai 5 dengan hasil nilai kurang dari 0,5.

6. Selesai

Langkah - langkah :

1. Buat program codenya seperti gambar dibawah ini

![Screenshot (132)](https://user-images.githubusercontent.com/115867244/200490320-4ac1d601-c3ae-4082-929a-a3e578d999c7.png)

    print("bilangan acak yang lebih kecil dari o.5")
    import random

    n = int(input("masukan nilai:"))
    a = 0
    for c in range(n):
        a += 1
        b = random.uniform(.0, .5)
        print("data ke:", a, "==>", b)

    print("selesai")

2. Hasil Run 

![Screenshot (133)](https://user-images.githubusercontent.com/115867244/200491112-68478144-0cb1-4a3a-afc1-20a2826a98ab.png)

### Latihan 2
Flowchart latihan 2

![200159970-42dd1c12-2af8-416d-b808-822ed3c3c7fc](https://user-images.githubusercontent.com/115867244/200491857-23239d93-dc61-49ed-95f4-534a4469c54c.png)

### Algoritma latihan 2
Membuat program untuk menampilkan bilangan terbesar dari n buah data yang diinputkan.Masukkan angka 0 untuk berhenti

1. Mulai

2. Mencetak "latihan 2"

3. Mencetak "menampilkan bilangan, berhenti ketika bilangan 0, menampilkan bilangan terbesar"

4. integer max = 0

5. Menggunakan fungsi perulangan while true, hingga menampilkan perulangan sampai batas tertentu.

6. Memasukan bilangan integer pada "a"

7. Menggunakan fungsi if jika max kurang dari nilai a, maka max sama dengan a

8. Mengunakan fungsi if jika nilai a adalah 0 maka fungsi break artinya perulangan berhenti jika menulis nilai 0.

9. Mencetak nilai paling terbesarv setelah break, sehingga menampilkan nilai terbesar diantara bilangan tersebut dalam perulangan.

10. Selesai

Langkah - langkah :

1. Buatlah program code seperti gambar dibawah ini

![Screenshot (134)](https://user-images.githubusercontent.com/115867244/200492333-8b21eade-bff5-4bad-a28f-f9f562a7c334.png)

    print("menampilkan bilangan, berhenti ketika bilangan 0, dan menampilkan bilangan terbesar")

    max = 0
    while True:
        angka = int(input("masukan bilangan : "))
        if max < angka:
            max = angka
        if angka == 0:
            break
    print("bilangan terbesarnya adalah = ", max)
    print("======selesai======")

2. Hasil Run 

![Screenshot (135)](https://user-images.githubusercontent.com/115867244/200492485-02dd2d8c-f7b6-4488-a654-d93de79f02df.png)

### Program 1
Flowchart program 1

![200160200-2f3db728-7d3d-48c0-b21a-b8d3bf11438b](https://user-images.githubusercontent.com/115867244/200492739-0b575aa2-ee9d-411f-a768-46402ddd5a22.png)

### Algoritma dari program 1
1. Mulai

2. Mencetak latihan1

3. Mencetak "Program menghitung laba dengan modal awal 100 juta"

4. Membuat Note

5. Mencetak Bulan pertama dan kedua = 0%

6. Mencetak bulan ke 3 = 1%

7. Mencetak bulan ke 5 = 5%

8. Mencetak bulan ke 8 = 2%

9. integer a = 100.000.000( modal awal)

10. Menggunakan fungsi looping for pada nilai x 1-9 untuk menampilkan bulan 1 sampai bulan 8.

11. Menggunakan fungsi if, untuk menghitung laba bulan 1 sampai 8

12. bulan pertama dan kedua laba adalah 0

13. bulan ke 3 dan ke 4 mendapat laba 1% sehingga modal di kali 1% = keuntungan

14. bulan ke 5 mendapatkan laba 5%, sehingga modal dikali 5% = keuntungan

15. Bulan ke 8 mmendapatkan laba 2% sehingga keuntungan menurun dari bulan sebelumnya, modal dikali 2% = keuntungan.

16. Menghitung jumlah total laba dengan menjumlah keuntungan dari bulan ke 1 sampai bulan 8, hasilnya adalah total keuntungan yang didapat.

17. Selesai

Langkah - langkah :

1. Buatlah program codenya seperti gambar dibawah ini

![Screenshot (136)](https://user-images.githubusercontent.com/115867244/200493286-83755cac-8d82-4c60-ab12-64c1fe05d19a.png)

    x = 100000000
    sum = 0
    y = 0
    lb = [int(0), int(0), int(x) * .1, int(x) * .1, int(x) * .5, int(x) * .5, 
    int(x) * .5, int(x) * .2]
    print("modal awal seorang pengusaha :', x")
    for i in lb:
        sum = sum + i
        y += 1
        print("#laba bulan ke - ", y, "sebesar :", i)

        print("  TOTAL LABA YANG DIDAPAT ADALAH :", sum)
        
2. Hasil Run 

![Screenshot (137)](https://user-images.githubusercontent.com/115867244/200493572-8fbfc3dd-a5c9-46ed-938d-063b2784ce42.png)

### Sekian, Terima kasih
