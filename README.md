Nama : Bayu Maulana Ayassy

Nim : 312210166

Kelas : TI.22.A1

# Latihan Python di Pycharm
### DAFTAR ISI <br>
| No | Description | Link |
| ----- | ----- | ---- |
| 1 | Cara Installasi Pycharm| [Click Here](#Cara-Installasi-Pycharm)|
| 2 | Latihan 1 | [Click Here](#Latihan-1) |
| 3 | Latihan 2 | [Click Here](#Latihan-2) |
| 4 | Latihan 3 | [Click Here](#Latihan-3) |
| 5 | Menghitung Luas Dan Keliling Lingkaran | [Click Here](#Menghitung-Luas-Dan-Keliling-Lingkaran) |
| 6 | Flowchart Menghitung luas dan keliling lingkaran | [Click Here](#Flowchart-Menghitung-luas-dan-keliling-lingkaran) |


# Cara Installasi Pycharm
1. Anda harus install Pycharm di https://www.jetbrains.com/pycharm/download/#section=windows  , Dan anda pilih yang Community
![Screenshot (76)](https://user-images.githubusercontent.com/115678171/198814989-ba36149f-cf88-492d-bb12-d00398751be4.png)
2. Anda next saja semua perintahnya 
3. Jika sudah selesai maka program siap di gunakan
# Cara Menjalankan Pycharm 
# Latihan 1
1. Pertama-tama anda harus Klik New project lalu kasih nama project anda(sesuai yang anda mau), Dan anda harus pilih yang Previously Configurred interperter lalu klik yang add interperter dan pilih yang System interperter dan anda klik yang versi Python anda seperti gambar di bawah ini
![Screenshot (78)](https://user-images.githubusercontent.com/115678171/198815436-8756894e-4eb0-4b58-81fe-165afda78652.png)
![Screenshot (77)](https://user-images.githubusercontent.com/115678171/198815442-dbfb3a6e-1d2f-4fdf-b205-1f7ddfb8b16c.png)

2. Selanjutnya anda membuat file Python baru di project anda tadi dan anda kasih nama file sesuai yang anda inginkan
![Screenshot (79)](https://user-images.githubusercontent.com/115678171/198815862-fbfc7ae9-dc11-4184-898a-4711596e2e7a.png)
![Screenshot (80)](https://user-images.githubusercontent.com/115678171/198815863-332a5b4f-c020-40b9-8331-4f98f5794ff9.png)

3. anda masukan code dari latihan1 anda lalu Run
```python
# penggunaan end
print('A', end='')
print('B', end='')
print('C', end='')
print()
print('X')
print('Y')
print('Z')

# penggunaan separator
w, x, y, z = 10, 15, 20, 25
print(w, x, y, z)
print(w, x, y, z, sep=',')
print(w, x, y, z, sep='')
print(w, x, y, z, sep=':')
print(w, x, y, z, sep='-----')

# string format
print(0, 10**0)
print(1, 10**1)
print(2, 10**2)
print(3, 10**3)
print(4, 10**4)
print(5, 10**5)
print(6, 10**6)
print(7, 10**7)
print(8, 10**8)
print(9, 10**9)
print(10, 10**10)

# string format
print('{0:>3} {1:>16}'.format(0, 10**0))
print('{0:>3} {1:>16}'.format(1, 10**1))
print('{0:>3} {1:>16}'.format(2, 10**2))
print('{0:>3} {1:>16}'.format(3, 10**3))
print('{0:>3} {1:>16}'.format(4, 10**4))
print('{0:>3} {1:>16}'.format(5, 10**5))
print('{0:>3} {1:>16}'.format(6, 10**6))
print('{0:>3} {1:>16}'.format(7, 10**7))
print('{0:>3} {1:>16}'.format(8, 10**8))
print('{0:>3} {1:>16}'.format(9, 10**9))
print('{0:>3} {1:>16}'.format(10, 10**10)
```
 
 ![Latihan1(1)](https://user-images.githubusercontent.com/115678251/199151672-4ccdca23-e26d-450e-a3d7-75cd297be5ee.png)

![Latihan1(2)](https://user-images.githubusercontent.com/115678251/199151733-d7a6b9d6-31ce-420f-acb1-2a3a5b7e23e8.png)

 
 *Hasil run*
![Run Latihan 1](https://user-images.githubusercontent.com/115678251/199151883-f675f8ad-6c8b-4b7a-8ba4-944748fc9745.png)


# Latihan 2 
1. Anda masukan code latihan 2 anda lalu Run 
```python
a=input("masukkan nilai a:")
b=input("masukkan nilai b:")
print("variable a=",a)
print("variable b=",b)
print("hasil penggabungan {1}&{0}=%s".format(a,b) %(a+b))

#koversi nilai variable
a=int(a)
b=int(b)
print("hasil penjumlahan {1}+{0}=%s".format(a,b) %(a+b))
print("hasil pembagian {1}/{0}=%s".format(a,b) %(a/b))
````
![Latihan 2](https://user-images.githubusercontent.com/115678251/199151998-ea986f81-642c-4a37-9892-f826d7f6dde7.png)

*Hasil Run*
![Run Latihan 2](https://user-images.githubusercontent.com/115678251/199152032-6fe43527-8adc-46e6-ae98-a145b104dd63.png)


# Latihan 3
1. Anda masukan code seperti dibawah ini dan lalu Run
```python
string = ""

x = int(input("Masukkan angka :"))
bar = x
# Looping Baris
while bar >= 0:
	# Looping Kolom Spasi Kosong
	kol = bar
	while kol > 0:
		string = string + "   "
		kol = kol - 1
	# Looping Kolom Bintang Sisi Kiri		
	kiri = 1
	while kiri < (x - (bar-1)):
		string = string + " * "
		kiri = kiri + 1		
	# Looping Kolom Bintang Sisi Kanan
	kanan = 1
	while kanan < kiri -1:
		string = string + " * "
		kanan = kanan + 1	

	string = string + "\n\n"
	bar = bar - 1

bar = 1	
# Looping Baris
while bar <= x:
	kol = bar+1
	# Looping Kolom Spasi Kosong
	while kol > 1:
		string = string + "   "
		kol = kol - 1
	# Looping Kolom Bintang Sisi Kiri	
	kiri = 0
	while kiri < (x - bar):
		string = string + " * "
		kiri = kiri + 1	
	# Looping Kolom Bintang Sisi Kanan
	kanan = kiri	
	while kanan > 1:
		string = string + " * "
		kanan = kanan - 1

	string = string + "\n\n"
	bar = bar + 1
print (string)
````
![Latihan 3 (1)](https://user-images.githubusercontent.com/115678251/199152523-4c061ced-9739-4def-8701-caba9d9e54ed.png)
![Latihan 3 (2)](https://user-images.githubusercontent.com/115678251/199152546-7c5ca23a-f2e4-475a-9b04-2aeabf40c1b0.png)


*Hasil Run*
![Run Latihan 3](https://user-images.githubusercontent.com/115678251/199152626-b6352947-25dd-4f1f-be22-2a43478dbd7a.png)

# Menghitung Luas Dan Keliling Lingkaran
1. Masukan code di bawah ini lalu run
```python
import math

r = float(input("Masukan Jari-jari : "))

luas = math.pi * (r * r)
keliling = 2 * math.pi * r

print("Luas Lingkaran \t\t= ", luas)
print("Keliling Lingkaran\t= ", keliling)
````
![Menghitung Luas Dan Keliling Lingkaran](https://user-images.githubusercontent.com/115678251/199152709-698e75c2-8546-4f0c-8ddd-3e0e6ba43353.png)


*Hasil Run*
![Run Menghitung Luas dan Keliling lingkaran](https://user-images.githubusercontent.com/115678251/199152760-0536d82b-e4f8-4210-b1f5-877c39f298ee.png)


# Flowchart Menghitung luas dan keliling lingkaran
![Flowchart menghitung luas dan keliling lingkaran](https://user-images.githubusercontent.com/115678171/198817259-154fec0b-f2b1-44e5-86c0-4c7ab1ad6142.png)

*Terima Kasih*
