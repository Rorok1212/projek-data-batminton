import os
import random
import string

# Membersihkan layar
os.system("cls")  # WIN
# os.system("clear")  # mac/linux

print(f" {'DATA PEMAIN BADMINTON':#^35}")

data = dict()

while True:
    # Membuat kunci acak
    keyFinal = "".join(random.choice(string.ascii_uppercase) for i in range(3))
    
    # Mengambil input dari pengguna
    nama = input("Enter nama pemain\t: ")
    kategori = input("Enter kategori (misal: Tunggal, Ganda): ")
    bahasa = input("Enter Rank\t: ")
    
    # Menyimpan data dalam dictionary
    data[keyFinal] = {
        'nama': nama,
        'kategori': kategori,
        'bahasa': bahasa
    }
    
    # Menanyakan apakah ingin input data lagi
    opsi = input("Input data LAGI (y/t) : ").lower()
    if opsi == 't':
        break
  
# Menampilkan hasil data
print("-" * 40)
print(f"{'Key':<5} {'Nama Pemain':<20} {'Kategori':<15} {'Rank':<15}")
print("-" * 40)
for k, v in data.items():
    print(f"{k:<5} {v['nama']:<20} {v['kategori']:<15} {v['Rank']:<15}")

# Menampilkan semua data
print("-" * 40)
print("Data lengkap pemain:")
print(data)
