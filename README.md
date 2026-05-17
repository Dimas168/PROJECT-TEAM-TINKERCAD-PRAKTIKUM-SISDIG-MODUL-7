# PROJECT-TEAM-TINKERCAD-PRAKTIKUM-SISDIG-MODUL-7
Ini merupakan tugas praktikum sistem digital pertemuan 8 dengan modul 7. Di pertemuan ini membahas mengenai gerbang logika dasar dan membuatnya menggunakan IC di simulasi tinkercad.

Kelompok 4

Anggota kelompok: 
1. Rizma Yusfa Maharani H1H025009 "Menulis buku catatan praktikum"
2. Dani Prayogi H1H025014 "Membuat laporan praktikum"
3. Dimas Adi Saputra H1H025026 "Membuat file README.md di github yang berisi penjelasan ketujuh rangkaian, screenshoot rangkaian, link tinkercad. Membuat rangkaian gerbang logika di tinkercad."

Link Tinkercad:
https://www.tinkercad.com/things/1BZPTAeGtrM-cool-albar-kasi?sharecode=HZ3cMUdos3U1jT0QfJSFYZIQnsdwGDDYN04_cS_KzgI

Materi Pembahasan: 

## 1. Gerbang Logika AND
   Komponen yang diperlukan:
   * Power Supply: Sumber listrik yang memberikan tegangan sebesar 5.00 V. 
   * IC 74HC08: IC ini berisi 4 buah gerbang logika AND (Quad 2-input AND gate).
   * DIP Switch (Saklar): Digunakan untuk memberikan sinyal input (Logika 1 / HIGH jika saklar dinaikkan, dan Logika 0 / LOW jika diturunkan).
   * Resistor & LED Hijau: Berfungsi sebagai indikator output. Jika output gerbang logika menyala (HIGH), LED akan ikut menyala. Resistor digunakan untuk menahan arus agar LED tidak putus/terbakar.

   Wiring kabel:
   * Daya (VCC & GND): Kabel dari kutub positif (merah) masuk ke Pin 14 (VCC) pada IC 74HC08. Kabel dari kutub negatif (hitam) masuk ke Pin 7 (GND) pada IC. 
   * Input (Saklar ke IC): Saklar 1 terhubung ke arus positif dan diteruskan ke Pin 1 (Input 1A) pada IC.
   * Saklar 2 terhubung ke arus positif dan diteruskan ke Pin 2 (Input 1B) pada IC.
   * Output (IC ke LED): Hasil perhitungan logika dikeluarkan melalui Pin 3 (Output 1Y). Arus ini mengalir melewati resistor, masuk ke kaki positif (anoda) LED, lalu keluar dari kaki negatif (katoda) LED menuju       Ground (negatif).

   Karakteristik utama dari gerbang logika AND adalah: Output hanya akan bernilai 1 (HIGH/Menyala) jika semua inputnya bernilai 1 (HIGH/Menyala). Jika salah satu atau kedua input mati, maka output akan mati.
   Karena kedua input bernilai 1 (1 AND 1), maka IC 74HC08 mengeluarkan sinyal 1 (HIGH) pada Pin 3. Arus listrik pun mengalir dan membuat LED hijau menyala.
   
   <img width="732" height="603" alt="image" src="https://github.com/user-attachments/assets/27b803ea-f331-4667-bd0a-c12d6acbe654" />
   
## 2. Gerbang Logika OR
   Komponen yang diperlukan:
   * Power Supply: Sumber listrik yang memberikan tegangan sebesar 5.00 V.
   * IC 74HC32: IC ini berisi 4 buah gerbang logika OR (Quad 2-input OR gate).
   * DIP Switch (Saklar): Digunakan untuk memberikan sinyal input (Logika 1 / HIGH jika saklar dinaikkan, dan Logika 0 / LOW jika diturunkan).
   * Resistor & LED Kuning: Berfungsi sebagai indikator output. Jika output gerbang logika menyala (HIGH), LED akan ikut menyala. Resistor digunakan untuk menahan arus agar LED tidak putus/terbakar.

   Wiring kabel:
   * Daya (VCC & GND): Kabel kuning dari kutub positif masuk ke Pin 14 (VCC) pada IC 74HC32. Kabel kuning dari kutub negatif masuk ke Pin 7 (GND) pada IC.
   * Input (Saklar ke IC): Saklar 1 terhubung ke arus positif dan diteruskan ke Pin 1 (Input 1A) pada IC. Saklar 2 terhubung ke arus positif dan diteruskan ke Pin 2 (Input 1B) pada IC.
   * Output (IC ke LED): Hasil perhitungan logika dikeluarkan melalui Pin 3 (Output 1Y). Arus ini mengalir melewati resistor, masuk ke kaki positif (anoda) LED, lalu keluar dari kaki negatif (katoda) LED menuju       Ground (negatif).

   Karakteristik utama dari gerbang logika OR adalah: Output akan bernilai 1 (HIGH/Menyala) jika salah satu atau kedua inputnya bernilai 1 (HIGH/Menyala). Output hanya akan mati jika semua input mati (0).
   Pada gambar, saklar 1 diturunkan (0) dan saklar 2 dinaikkan (1). Karena salah satu input bernilai 1 (0 OR 1), maka IC 74HC32 mengeluarkan sinyal 1 (HIGH) pada Pin 3. Arus listrik pun mengalir dan                 membuat LED kuning menyala.
   
   <img width="673" height="580" alt="image" src="https://github.com/user-attachments/assets/3d6b728b-4707-47fd-ad5b-c2055f1a4f85" />

## 3. Gerbang Logika NOT

  Komponen yang diperlukan:
  * Power Supply: Sumber listrik yang memberikan tegangan sebesar 5.00 V.
  * IC 74HC04: IC ini berbeda dari sebelumnya, ia berisi 6 buah gerbang logika NOT (Hex Inverter). Setiap gerbang NOT hanya membutuhkan 1 input.
  * DIP Switch (Saklar): Digunakan untuk memberikan sinyal input (Logika 1 / HIGH jika saklar dinaikkan, dan Logika 0 / LOW jika diturunkan).
  * Resistor & LED Oranye: Berfungsi sebagai indikator output. Jika output gerbang logika menyala (HIGH), LED akan ikut menyala. Resistor digunakan untuk menahan arus agar LED tidak putus/terbakar.

  Wiring kabel:
  * Daya (VCC & GND): Kabel oranye dari kutub positif masuk ke Pin 14 (VCC) pada IC 74HC04. Kabel oranye dari kutub negatif masuk ke Pin 7 (GND) pada IC.
  * Input (Saklar ke IC): Karena gerbang NOT hanya butuh satu input, hanya Saklar 1 yang digunakan. Saklar 1 terhubung ke arus positif dan sinyalnya diteruskan ke Pin 1 (Input 1A) pada IC.
  * Output (IC ke LED): Hasil perhitungan logika dikeluarkan melalui Pin 2 (Output 1Y) (berbeda dengan IC sebelumnya yang menggunakan Pin 3 untuk output pertama). Arus ini mengalir melewati resistor, masuk ke        kaki positif (anoda) LED, lalu keluar dari kaki negatif (katoda) LED menuju Ground (negatif).

Karakteristik utama dari gerbang logika NOT (Inverter) adalah pembalik keadaan: Output akan selalu berlawanan dengan inputnya. Jika input bernilai 1 (ON), maka output akan 0 (OFF). Sebaliknya, jika input 0 (OFF), maka output akan 1 (ON).
Pada gambar, Saklar 1 diturunkan yang berarti memberikan sinyal 0 (OFF). Karena inputnya 0, IC 74HC04 membalik sinyal tersebut dan mengeluarkan sinyal 1 (HIGH) pada Pin 2. Arus listrik pun mengalir dan membuat LED oranye menyala.

   <img width="663" height="601" alt="image" src="https://github.com/user-attachments/assets/77689fed-3e97-4110-8360-982ae331d838" />

## 4. Gerbang Logika NAND

  Komponen yang diperlukan:
  * Power Supply: Sumber listrik yang memberikan tegangan sebesar 5.00 V.
  * IC 74HC00: IC ini berisi 4 buah gerbang logika NAND (Quad 2-input NAND gate).
  * DIP Switch (Saklar): Digunakan untuk memberikan sinyal input (Logika 1 / HIGH jika saklar dinaikkan, dan Logika 0 / LOW jika diturunkan).
  * Resistor & LED Biru: Berfungsi sebagai indikator output. Jika output gerbang logika menyala (HIGH), LED akan ikut menyala.

  Wiring kabel:
  * Daya (VCC & GND): Kabel biru dari kutub positif masuk ke Pin 14 (VCC) pada IC 74HC00. Kabel biru dari kutub negatif masuk ke Pin 7 (GND) pada IC.
  * Input (Saklar ke IC): Saklar 1 terhubung ke arus positif dan diteruskan ke Pin 1 (Input 1A) pada IC. Saklar 2 terhubung ke arus positif dan diteruskan ke Pin 2 (Input 1B) pada IC.
  * Output (IC ke LED): Hasil perhitungan logika dikeluarkan melalui Pin 3 (Output 1Y). Arus ini mengalir melewati resistor, masuk ke kaki positif (anoda) LED, lalu keluar dari kaki negatif (katoda) LED menuju       Ground (negatif).

Karakteristik utama dari gerbang logika NAND adalah kebalikan persis dari gerbang AND. Output hanya akan bernilai 0 (Mati) jika semua inputnya bernilai 1 (HIGH). Jika ada salah satu saja input yang bernilai 0 (OFF), atau keduanya 0, maka output justru akan bernilai 1 (Menyala).
Pada gambar, Saklar 1 dinaikkan (1) dan Saklar 2 juga dinaikkan (1). Karena kedua input bernilai 1 (1 NAND 1), maka IC 74HC00 mengeluarkan sinyal 0 (LOW) pada Pin 3. Akibatnya, arus listrik tidak mengalir ke output dan LED biru dalam kondisi mati (tidak menyala).

   <img width="708" height="542" alt="image" src="https://github.com/user-attachments/assets/9e660bde-1ddc-45fb-a8cd-10c9f85055cd" />

## 5. Gerbang Logika NOR

  Komponen yang diperlukan:
  * Power Supply: Sumber listrik yang memberikan tegangan sebesar 5.00 V.
  * IC 74HC02: IC ini berisi 4 buah gerbang logika NOR (Quad 2-input NOR gate).
  * DIP Switch (Saklar): Digunakan untuk memberikan sinyal input (Logika 1 / HIGH jika saklar dinaikkan, dan Logika 0 / LOW jika diturunkan).
  * Resistor & LED Merah: Berfungsi sebagai indikator output. Jika output gerbang logika menyala (HIGH), LED akan ikut menyala.

  Wiring kabel:
  * Daya (VCC & GND): Kabel merah dari kutub positif masuk ke Pin 14 (VCC) pada IC 74HC02. Kabel merah dari kutub negatif masuk ke Pin 7 (GND) pada IC.
  * Input (Saklar ke IC): Perlu dicatat bahwa susunan pin pada IC 74HC02 sedikit berbeda dari gerbang logika lain. Saklar 1 terhubung ke arus positif dan diteruskan ke Pin 2 (Input 1A) pada IC. Saklar 2
    terhubung ke arus positif dan diteruskan ke Pin 3 (Input 1B) pada IC.
  * Output (IC ke LED): Hasil perhitungan logika dikeluarkan melalui Pin 1 (Output 1Y). Arus ini mengalir melewati resistor, masuk ke kaki positif (anoda) LED, lalu keluar dari kaki negatif (katoda) LED menuju       Ground (negatif).

    Karakteristik utama dari gerbang logika NOR adalah kebalikan persis dari gerbang OR. Output hanya akan bernilai 1 (Menyala) jika semua inputnya bernilai 0 (OFF). Jika ada salah satu saja input yang bernilai      1 (ON), atau keduanya 1, maka output justru akan bernilai 0 (Mati).
    Pada gambar, Saklar 1 dinaikkan (1) dan Saklar 2 diturunkan (0). Karena ada salah satu input yang bernilai 1 (1 NOR 0), maka IC 74HC02 mengeluarkan sinyal 0 (LOW) pada Pin 1. Akibatnya, arus listrik tidak        mengalir ke output dan LED merah dalam kondisi mati (tidak menyala).
    
    <img width="727" height="578" alt="image" src="https://github.com/user-attachments/assets/9b99f4e4-8659-43a6-b5a3-83c3921a9b1c" />

## 6. Gerbang Logika XOR

   Komponen yang diperlukan:
   * Power Supply: Sumber listrik yang memberikan tegangan sebesar 5.00 V.
   * IC 74HC86: IC ini berisi 4 buah gerbang logika XOR (Quad 2-input XOR gate).
   * DIP Switch (Saklar): Digunakan untuk memberikan sinyal input (Logika 1 / HIGH jika saklar dinaikkan, dan Logika 0 / LOW jika diturunkan).
   * Resistor & LED Putih: Berfungsi sebagai indikator output. Jika output gerbang logika menyala (HIGH), LED akan ikut menyala.

  Wiring kabel:
  * Daya (VCC & GND): Kabel putih dari kutub positif masuk ke Pin 14 (VCC) pada IC 74HC86. Kabel putih dari kutub negatif masuk ke Pin 7 (GND) pada IC.
  * Input (Saklar ke IC): Saklar 1 terhubung ke arus positif dan diteruskan ke Pin 1 (Input 1A) pada IC. Saklar 2 terhubung ke arus positif dan diteruskan ke Pin 2 (Input 1B) pada IC.
  * Output (IC ke LED): Hasil perhitungan logika dikeluarkan melalui Pin 3 (Output 1Y). Arus ini mengalir melewati resistor, masuk ke kaki positif (anoda) LED, lalu keluar dari kaki negatif (katoda) LED menuju       Ground (negatif).

    Karakteristik utama dari gerbang logika XOR (Exclusive-OR) adalah mendeteksi perbedaan status input. Output hanya akan bernilai 1 (Menyala) jika kedua inputnya memiliki nilai yang berbeda (satu input             bernilai 1 dan input lainnya bernilai 0). Jika kedua input bernilai sama (sama-sama 0 atau sama-sama 1), maka output justru akan bernilai 0 (Mati).
    Pada gambar, Saklar 1 dinaikkan (1) dan Saklar 2 diturunkan (0). Karena kedua input memiliki nilai yang berbeda (1 XOR 0), maka IC 74HC86 mengeluarkan sinyal 1 (HIGH) pada Pin 3. Akibatnya, arus listrik          mengalir ke output dan LED putih dalam kondisi menyala.
    
    <img width="696" height="598" alt="image" src="https://github.com/user-attachments/assets/ab202b34-d883-4c5e-97df-f4ebf7d9977e" />


## 7. Gerbang Logika XNOR
   
  Komponen yang diperlukan:
  * Power Supply: Sumber listrik yang memberikan tegangan sebesar 5.00 V.
  * IC 74HC86 & IC 74HC04: Rangkaian ini menggunakan kombinasi IC 74HC86 yang berisi gerbang logika XOR dan IC 74HC04 yang berisi gerbang logika NOT (Inverter) untuk membentuk fungsi logika XNOR.
  * DIP Switch (Saklar): Digunakan untuk memberikan sinyal input (Logika 1 / HIGH jika saklar dinaikkan, dan Logika 0 / LOW jika diturunkan).
  * Resistor & LED Merah: Berfungsi sebagai indikator output akhir. Jika output gerbang logika menyala (HIGH), LED akan ikut menyala.

  Wiring kabel:
  * Daya (VCC & GND): Kabel hitam dari kutub positif masuk ke Pin 14 (VCC) pada kedua IC. Kabel hitam dari kutub negatif masuk ke Pin 7 (GND) pada kedua IC.
  * Input (Saklar ke IC awal): Saklar 1 terhubung ke arus positif dan diteruskan ke Pin 1 (Input 1A) pada IC 74HC86 (XOR). Saklar 2 terhubung ke arus positif dan diteruskan ke Pin 2 (Input 1B) pada IC 74HC86.
  * Proses Pembalikan (XOR ke NOT): Hasil perhitungan logika dari IC 74HC86 dikeluarkan melalui Pin 3 (Output 1Y) dan langsung diteruskan menjadi input ke Pin 1 (Input 1A) pada IC 74HC04 (NOT).
  * Output Akhir (IC ke LED): Hasil akhir yang sudah dibalik dikeluarkan melalui Pin 2 (Output 1Y) pada IC 74HC04. Arus ini mengalir melewati resistor, masuk ke kaki positif (anoda) LED, lalu keluar dari kaki        negatif (katoda) LED menuju Ground (negatif).

    Karakteristik utama dari gerbang logika XNOR (Exclusive-NOR) adalah mendeteksi kesamaan status input. Output hanya akan bernilai 1 (Menyala) jika kedua inputnya memiliki nilai yang sama persis (sama-sama 0       atau sama-sama 1). Jika kedua input memiliki nilai yang berbeda, maka output justru akan bernilai 0 (Mati).
    Pada gambar, Saklar 1 dinaikkan (1) dan Saklar 2 diturunkan (0). Karena kedua input memiliki nilai yang berbeda, IC 74HC86 (XOR) awalnya menghasilkan sinyal 1. Namun, sinyal 1 ini kemudian masuk ke IC 74HC04     (NOT) dan dibalik menjadi 0 (LOW) pada Pin 2. Akibatnya, arus listrik tidak mengalir ke output akhir dan LED merah dalam kondisi mati (tidak menyala).
    
<img width="1256" height="657" alt="image" src="https://github.com/user-attachments/assets/83460881-3a7f-4b82-93de-ea3eb0033506" />



