# tugas Sesi-7-dasar-pemrograman

print("NAMA\t= MUHAMAD NUR AIDUL HARPAN")
print("KELAS\t= TI22J")
print("NIM\t= 20220040237")
print("====================================")
print("MENU :\n1.Luas segitiga")
print("2.Luas persegi panjang")
print("3.Menentukan bilangan Ganjil & Genap\n4.quit")

def Luas_segitiga():
	print("==========LUAS SEGITIGA==========")
	alas = int(input("Masukan nilai alas \t: "))
	tinggi = int(input("masukan nilai tinggi \t: "))
	luas = 0.5* alas * tinggi
	
	print("luas segitiga adalah \t=",luas, "cm\n")

def Luas_persegi_panjang():
	print("=========LUAS PERSEGI PANJANG=========")
	panjang = int(input("masukan nilai panjang\t : "))
	lebar = int(input("masukan nilai lebar \t : "))
	luas = panjang * lebar
	
	print("Luas persegi panjang adalah = ",luas,"cm\n")
	
def Bilangan_Ganjil_Genap():
	print("=========BILANGAN GANJIL & GENAP=======")
	awal = int(input("masukan angka awal \t: "))
	akhir = int(input("masukan angka akhir\t: "))
	x = [ ]
	y = [ ]
	
	for i in range(awal,akhir+1):
		if i % 2 == 0:
			x.append(i)
		if i % 2 == 1:
			y.append(i)
	print("Angka genap \t= ",x)
	print("Angka ganjil \t= ", y,"\n")
		
while True:
		inputUser = int(input("Masukan pilihan anda = "))
		
		if (inputUser == 1):
			Luas_segitiga()
		elif (inputUser == 2):
			Luas_persegi_panjang()
		elif(inputUser == 3):
			Bilangan_Ganjil_Genap()
		else :
			print("PROGRAM SELESAI TERIMAKASIH")
			break	
			
