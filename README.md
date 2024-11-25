# Biodata

NAMA = RAFLI ANUGRAH RAMADHAN

KELAS = TI 24, A4

NIM = 312410351

MATKUL = PEMROGRAMAN

# Latihan 1

<img width="416" alt="image" src="https://github.com/user-attachments/assets/20ebb622-9f9f-49f1-8635-9fdef32e665e">

# kodenya

<img width="359" alt="image" src="https://github.com/user-attachments/assets/1de4d9d7-5270-4c0d-a010-a2f5e87bbadd">

<img width="314" alt="image" src="https://github.com/user-attachments/assets/23b88cde-dbd0-4287-8856-0d7c59b633af">

# Penjelasan Pogram

1. Inisialisasi Dictionary kosong
```python
daftar_kontak = {}
Pada awalnya, kita membuat sebuah Dictionary kosong yang akan digunakan untuk menyimpan data kontak. Di dalam dictionary ini, key adalah nama kontak, dan value adalah nomor telepon dari kontak tersebut.

2. Fungsi Menampilkan Semua Kontak
```python
def tampilkan_kontak():
    print("\nDaftar Kontak:")
    if daftar_kontak:
        print("Nama  | No Telpon")
        print("===================")
        for nama, nomor in daftar_kontak.items():
            print(f"{nama}    | {nomor}")
    else:
        print("Tidak ada kontak dalam daftar.")
````

Fungsi ini digunakan untuk menampilkan seluruh kontak yang ada di dalam dictionary. Fungsi items() digunakan untuk mendapatkan pasangan key (nama) dan value (nomor). Jika dictionary kosong, akan menampilkan pesan "Tidak ada kontak dalam daftar."

3. Fungsi Menambah Kontak Baru
```python
def tambah_kontak():
    nama = input("Masukkan nama kontak: ")
    nomor = input("Masukkan nomor telepon: ")
    daftar_kontak[nama] = nomor
    print(f"Kontak {nama} berhasil ditambahkan.")
````
Fungsi ini meminta pengguna untuk menginputkan nama dan nomor telepon kontak yang ingin ditambahkan ke dalam daftar. Nilai-nilai ini kemudian disimpan ke dalam dictionary dengan nama sebagai key dan nomor sebagai value.

4. Fungsi Mengubah Kontak
```python
def ubah_kontak():
    nama = input("Masukkan nama kontak yang ingin diubah: ")
    if nama in daftar_kontak:
        nomor_baru = input(f"Masukkan nomor baru untuk {nama}: ")
        daftar_kontak[nama] = nomor_baru
        print(f"Kontak {nama} berhasil diubah.")
    else:
        print(f"Kontak {nama} tidak ditemukan.")
````
Fungsi ini memungkinkan pengguna untuk mengubah nomor telepon kontak yang sudah ada. Pertama, program meminta nama kontak yang ingin diubah. Jika kontak tersebut ditemukan dalam dictionary, maka nomor lama akan digantikan dengan nomor baru yang dimasukkan oleh pengguna.

5. Fungsi Menghapus Kontak
```python
def hapus_kontak():
    nama = input("Masukkan nama kontak yang ingin dihapus: ")
    if nama in daftar_kontak:
        del daftar_kontak[nama]
        print(f"Kontak {nama} berhasil dihapus.")
    else:
        print(f"Kontak {nama} tidak ditemukan.")
````
Fungsi ini memungkinkan pengguna untuk menghapus kontak dari daftar. Pengguna diminta memasukkan nama kontak yang ingin dihapus. Jika nama ditemukan dalam dictionary, maka entri tersebut dihapus menggunakan perintah del.

6. Fungsi Menampilkan Semua Nama Kontak
```python
def tampilkan_semua_nama():
    print("\nSemua Nama:")
    for nama in daftar_kontak.keys():
        print(nama)
````
Fungsi ini menampilkan semua nama yang ada dalam daftar kontak. Fungsi keys() digunakan untuk mengambil semua key (nama) yang ada dalam dictionary dan menampilkannya satu per satu.

7. Fungsi Menampilkan Semua Nomor Kontak
```python
def tampilkan_semua_nomor():
    print("\nSemua Nomor:")
    for nomor in daftar_kontak.values():
        print(nomor)
````
Fungsi ini menampilkan semua nomor telepon yang ada dalam daftar kontak. Fungsi values() digunakan untuk mengambil semua value (nomor telepon) yang ada dalam dictionary dan menampilkannya satu per satu.

# Hasil Kodenya

<img width="248" alt="image" src="https://github.com/user-attachments/assets/8ac80bc9-38b0-44d5-8205-ca531342cac8">

<img width="241" alt="image" src="https://github.com/user-attachments/assets/c8806c3a-c376-4b2a-a240-840ac1f762af">

# Tugas Praktikum

<img width="509" alt="image" src="https://github.com/user-attachments/assets/aafeef5a-f3a5-4e7d-b58e-61908dd44b40">

# Kodenya

<img width="596" alt="image" src="https://github.com/user-attachments/assets/4e3814a9-57cd-48d8-97fb-fa65f19e950b">

<img width="690" alt="image" src="https://github.com/user-attachments/assets/7ad81009-abd1-482a-bde5-7d4f81ff228f">

<img width="347" alt="image" src="https://github.com/user-attachments/assets/9a0b6543-65c2-4b08-9a8a-21ac18553f21">

# Penjelasan Program

1. Struktur Data (Dictionary)
Data mahasiswa disimpan dalam dictionary dengan format:

```python
data_mahasiswa = {
    "NIM": {
        "Nama": "Nama Mahasiswa",
        "Tugas": nilai_tugas,
        "UTS": nilai_uts,
        "UAS": nilai_uas,
        "Nilai Akhir": nilai_akhir
    }
}
````
Key utama adalah NIM.
Value adalah dictionary lain yang berisi data mahasiswa (nama, nilai tugas, UTS, UAS, dan nilai akhir).

2. Fungsi Hitung Nilai Akhir
```python
def hitung_nilai_akhir(tugas, uts, uas):
    return (tugas * 0.3) + (uts * 0.35) + (uas * 0.35)
````
Fungsi ini menerima nilai tugas, UTS, dan UAS sebagai input, lalu menghitung nilai akhir berdasarkan bobot:

Tugas: 30%
UTS: 35%
UAS: 35%

3. Menambah Data Mahasiswa
```python
def tambah_data():
    nim = input("Masukkan NIM: ")
    nama = input("Masukkan Nama: ")
    tugas = float(input("Masukkan Nilai Tugas: "))
    uts = float(input("Masukkan Nilai UTS: "))
    uas = float(input("Masukkan Nilai UAS: "))
    nilai_akhir = hitung_nilai_akhir(tugas, uts, uas)
    data_mahasiswa[nim] = {"Nama": nama, "Tugas": tugas, "UTS": uts, "UAS": uas, "Nilai Akhir": nilai_akhir}
    print(f"Data mahasiswa dengan NIM {nim} berhasil ditambahkan.")
````
Fungsi ini meminta input pengguna untuk data NIM, nama, tugas, UTS, dan UAS. Nilai akhir dihitung menggunakan fungsi hitung_nilai_akhir(), lalu data dimasukkan ke dalam dictionary.

4. Mengubah Data Mahasiswa
```python
def ubah_data():
    nim = input("Masukkan NIM mahasiswa yang akan diubah: ")
    if nim in data_mahasiswa:
        print(f"Data saat ini: {data_mahasiswa[nim]}")
        nama = input("Masukkan Nama baru: ")
        tugas = float(input("Masukkan Nilai Tugas baru: "))
        uts = float(input("Masukkan Nilai UTS baru: "))
        uas = float(input("Masukkan Nilai UAS baru: "))
        nilai_akhir = hitung_nilai_akhir(tugas, uts, uas)
        data_mahasiswa[nim] = {"Nama": nama, "Tugas": tugas, "UTS": uts, "UAS": uas, "Nilai Akhir": nilai_akhir}
        print(f"Data mahasiswa dengan NIM {nim} berhasil diubah.")
    else:
        print(f"Data dengan NIM {nim} tidak ditemukan.")
````
Fungsi ini memungkinkan pengguna memperbarui data mahasiswa berdasarkan NIM. Jika NIM ditemukan, pengguna dapat memasukkan data baru.

6. Menghapus Data Mahasiswa
```python
def hapus_data():
    nim = input("Masukkan NIM mahasiswa yang akan dihapus: ")
    if nim in data_mahasiswa:
        del data_mahasiswa[nim]
        print(f"Data mahasiswa dengan NIM {nim} berhasil dihapus.")
    else:
        print(f"Data dengan NIM {nim} tidak ditemukan.")
````
Fungsi ini menghapus data mahasiswa berdasarkan NIM yang diberikan.

7. Menampilkan Semua Data
```python
def tampilkan_data():
    if data_mahasiswa:
        print("\nDaftar Nilai Mahasiswa:")
        print("=" * 50)
        print(f"{'NIM':<10} {'Nama':<15} {'Tugas':<10} {'UTS':<10} {'UAS':<10} {'Nilai Akhir':<10}")
        print("=" * 50)
        for nim, data in data_mahasiswa.items():
            print(f"{nim:<10} {data['Nama']:<15} {data['Tugas']:<10} {data['UTS']:<10} {data['UAS']:<10} {data['Nilai Akhir']:<10.2f}")
    else:
        print("Belum ada data mahasiswa.")
````
Fungsi ini mencetak daftar semua mahasiswa dalam format tabel.

# Hasil Kodenya

<img width="443" alt="image" src="https://github.com/user-attachments/assets/60e1a60d-3383-47ed-9018-05b057151d21">

<img width="374" alt="image" src="https://github.com/user-attachments/assets/f1332ef8-4944-4ff4-809f-e5ac6ccea813">

<img width="169" alt="image" src="https://github.com/user-attachments/assets/d5b4da5f-a358-4c6f-945c-5ff57101bd8b">

# Flowchart

![image](https://github.com/user-attachments/assets/5e8272b5-3933-474a-b435-0a36f47d90d5)
























































