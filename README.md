## Tugas bahasa pemrograman pertemuan 15
## BIODATA
NAMA: Mochamad Nabil Kurnia

KELAS TI 24,A,4

NIM:312410307

MATKUL:BAHASA PEMOGRAMAN

Dosen : Agung Nugroho, S.Kom., M.Kom.

![Screenshot 2025-01-06 131545](https://github.com/user-attachments/assets/efa5e897-28cb-487c-89d8-b3208683c9d9)

# kode program yang dijalankan

```python
def validasi_nama(nama):
    if not nama.isalpha():
        return "Nama hanya boleh berisi huruf."
    return None

def validasi_telepon(telepon):
    if not telepon.isdigit():
        return "Nomor telepon hanya boleh berisi angka."
    return None

def validasi_email(email):
    if "@" not in email or "." not in email:
        return "Email harus mengandung karakter '@' dan '.'."
    return None

def validasi_form(nama, telepon, email):
    errors = []

    error_nama = validasi_nama(nama)
    if error_nama:
        errors.append(error_nama)

    error_telepon = validasi_telepon(telepon)
    if error_telepon:
        errors.append(error_telepon)
    
    error_email = validasi_email(email)
    if error_email:
        errors.append(error_email)
    
    if errors:
        for error in errors:
            print("Error:", error)
    else:
        print("Data pendaftaran valid.")

nama = input("Masukkan nama lengkap: ")
telepon = input("Masukkan nomor telepon: ")
email = input("Masukkan email: ")

validasi_form(nama, telepon, email)
````

![image](https://github.com/user-attachments/assets/84c73d20-09c6-434d-9b3f-8965c8310b8c)


# penjelasan

1. Fungsi validasi_nama:

Mengecek apakah nama hanya berisi huruf dengan metode .isalpha().

2. Fungsi validasi_telepon:

Mengecek apakah telepon hanya berisi angka dengan metode .isdigit().

3. Fungsi validasi_email:

Mengecek apakah email mengandung karakter @ dan ..

4. Fungsi validasi_form:

Memanggil setiap fungsi validasi dan menampilkan pesan kesalahan jika ada.

Jika tidak ada kesalahan, menampilkan pesan bahwa data valid.


# hasil kode

![Screenshot 2025-01-06 131800](https://github.com/user-attachments/assets/531e3695-e7e9-44f5-bcb2-022cf6cb9b76)


