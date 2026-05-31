# pertemuan-11
# Program Pendaftaran Pasien Rawat Jalan Menggunakan Array 1 Dimensi dan 2 Dimensi
# Algoritma Pendaftaran Pasien Rawat Jalan (dari Pendaftaran hingga Pengambilan Hasil Lab dan Obat)
1.	Pasien datang ke rumah sakit
2.	Pasien menuju loket pendaftaran rawat jalan.
3.	Petugas menanyakan apakah pasien sudah pernah berobat (pasien lama atau baru). 
	  Jika pasien baru: Petugas mencatat data identitas pasien (nama, tanggal lahir, alamat, nomor KTP/BPJS) dan membuat nomor rekam medis baru.
    Jika pasien lama: Petugas mencari data pasien berdasarkan nomor rekam medis atau KTP.
5.	Petugas menanyakan keluhan/tujuan poliklinik yang dituju.
6.	Petugas mendaftarkan pasien ke poliklinik yang sesuai dan mencetak nomor antrian.
7.	Pasien menunggu di ruang tunggu poliklinik yang dituju.
8.	Perawat memanggil pasien sesuai nomor antrian dan melakukan pemeriksaan awal (tekanan darah, berat badan, suhu tubuh).
9.	 Dokter memanggil dan memeriksa pasien. 
10.	Dokter menentukan diagnosis.
    Jika pasien memerlukan pemeriksaan laboratorium: Dokter membuat surat pengantar lab, pasien diarahkan ke laboratorium. 
    Petugas lab menerima pasien dan surat pengantar.
•	Petugas lab mengambil sampel (darah, urine, dll) sesuai kebutuhan.
•	Pasien menunggu proses pemeriksaan sampel.
•	Setelah selesai, hasil laboratorium dicetak dan diserahkan ke pasien/dikirim ke dokter.
•	Pasien kembali ke dokter dengan membawa hasil lab.
•	Dokter membaca hasil lab dan memberikan penjelasan serta diagnosis akhir.
    Jika tidak perlu lab: Langsung ke langkah berikutnya.
11.	Dokter menulis resep obat untuk pasien. 
12.	Pasien menuju loket administrasi untuk menyelesaikan pembayaran (tunai/BPJS/asuransi). 
13.	Pasien membawa resep ke apotek/farmasi rumah sakit.
14.	Petugas farmasi menerima dan memproses resep.
15.	Pasien menunggu obat disiapkan.
16.	Petugas farmasi memanggil pasien, menyerahkan obat, dan memberikan penjelasan cara penggunaan obat.
17.	Pasien menerima obat dan proses selesai.
18.	Pasien pulang.
# Data yang sudah di ubah ke arrray 1d 
DATA	          ARRAY 1D
Nama Pasien 	  nama_pasien[] 
Tanggal Lahir	  tanggal_lahir[]
Alamat	        alamat_pasien[]
No KTP	        no_identitas[]
Keluhan	        keluhan_pasien[]
Poliklinik	    poliklinik[]
Diagnosis	      diagnosis[]
Obat	          obat_pasien[]
# Data yang sudah di ubah ke arrray 2d
DATA                           ARRAY 2 DIMENSI
Seluruh Data Pasien            data_pasien[][] 
Format penyimpanan            
                               [
                                nama,
                                tanggal_lahir,
                                alamat,
                                no_identitas, 
                                keluhan,
                                poliklinik
# ouput ke file (array 1d )
nama_pasien = ["eka","tuti","buna"]
keluhan_pasien = ["Demam", "Batuk", "asma"]
obat_pasien = ["Paracetamol", "OBH", "teofilin"]
with open("hasil_array1.txt", "w") as file:
    file.write("=== DATA PASIEN (ARRAY 1 DIMENSI) ===\n\n")
    file.write("Nama Pasien:\n")
    for n in nama_pasien:
        file.write(n + "\n")
    file.write("\nKeluhan Pasien:\n")
    for k in keluhan_pasien:
        file.write(k + "\n")
    file.write("\nObat Pasien:\n")
    for o in obat_pasien:
        file.write(o + "\n")
# output ke console ( array 1d )
=== DATA PASIEN (ARRAY 1 DIMENSI) ===

Nama Pasien:
eka
tuti
buna

Keluhan Pasien:
asma
demam
batuk

Obat Pasien:
teofilin
paracetamol
obh
File hasil_array1.txt berhasil dibuat!
# ouput ke file (array 2d)
nama_pasien = ["eka","tuti","buna"]
keluhan_pasien = ["Demam", "Batuk", "asma"]
obat_pasien = ["Paracetamol", "OBH", "teofilin"]
with open("hasil_array2.txt", "w") as file:
    file.write("=== DATA PASIEN (ARRAY 2 DIMENSI) ===\n\n")
    for pasien in data_pasien:
        file.write(
            "Nama: " + pasien[0] +
            ", Keluhan: " + pasien[1] +
            ", Obat: " + pasien[2] + "\n"
            )
# output ke console ( array 2d )
=== DATA PASIEN (ARRAY 2 DIMENSI) ===
Nama : eka
Keluhan : asma
Obat : teofilin
----------------
Nama : tuti
Keluhan : demam
Obat : paracetamol
----------------
Nama : buna
Keluhan : batuk
Obat : obh
----------------
File hasil_array2.txt berhasil dibuat!










    
