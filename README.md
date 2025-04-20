# Tugas2
https://studio.firebase.google.com/tugas2-43866008


#applikasi sedernaha
def tambah(x, y):
    return x + y

def kurang(x, y):
    return x - y

def kali(x, y):
    return x * y

def bagi(x, y):
    if y == 0:
        return "Tidak bisa dibagi dengan nol!"
    return x / y

print("Pilih operasi:")
print("1. Penjumlahan (+)")
print("2. Pengurangan (-)")
print("3. Perkalian (*)")
print("4. Pembagian (/)")

while True:
    pilihan = input("Masukkan pilihan (1/2/3/4): ")

if pilihan in ('1', '2', '3', '4'):
      try:
          angka1 = float(input("Masukkan bilangan pertama: "))
          angka2 = float(input("Masukkan bilangan kedua: "))
      except ValueError:
          print("Input tidak valid. Masukkan angka.")
          continue

      if pilihan == '1':
          print(angka1, "+", angka2, "=", tambah(angka1, angka2))

      elif pilihan == '2':
          print(angka1, "-", angka2, "=", kurang(angka1, angka2))

      elif pilihan == '3':
          print(angka1, "*", angka2, "=", kali(angka1, angka2))

      elif pilihan == '4':
          print(angka1, "/", angka2, "=", bagi(angka1, angka2))

      ulangi = input("Lakukan perhitungan lagi? (ya/tidak): ")
      if ulangi.lower() != "ya":
            break
  else:
        print("Input tidak valid. Masukkan pilihan antara 1 dan 4.")
