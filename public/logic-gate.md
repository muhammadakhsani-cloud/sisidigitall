# Laporan Praktikum Rangkaian Gerbang Logika Digital

- **Link Tinkercad** : [Sirkuit Gerbang Logika IC](https://www.tinkercad.com/things/9QlM81qomQB-gerbang-logika-ic?sharecode=CVY2bzqg5vE3qek5wNBQwEZxSso6vzww3tzUkDW_ukw)
- **Link Repositori GitHub** : [github.com/muhammadakhsani-cloud/sisidigitall](https://github.com/muhammadakhsani-cloud/sisidigitall)


## Rangkaian Gerbang Logika

### 1. Gerbang AND
Gerbang AND menghasilkan output bernilai 1 hanya jika kedua input bernilai 1. Jika salah satu atau kedua input bernilai 0, maka output akan bernilai 0.

#### Komponen yang Digunakan
- Power Supply DC
- IC 74HC08
- LED
- Resistor 220Ω
- DIP Switch

#### Skema Rangkaian & Simulasi
<img width="723" height="512" alt="Screenshot From 2026-05-15 09-03-38" src="https://github.com/user-attachments/assets/d41c9f02-0c5f-4e8a-a99a-a4688ec5847f" />


#### Penjelasan Diagram Pin IC
Rangkaian ini menggunakan IC 74HC08 yang berisi 4 gerbang AND mandiri. Chip ini dilengkapi dengan paket 14 pin.

---

### 2. Gerbang OR
Gerbang OR menghasilkan output bernilai 1 jika salah satu atau kedua input bernilai 1. Output hanya bernilai 0 ketika seluruh input bernilai 0.

#### Komponen yang Digunakan
- Power Supply DC
- IC 74HC32
- LED
- Resistor 220Ω
- DIP Switch

#### Skema Rangkaian & Simulasi
<img width="755" height="556" alt="Screenshot From 2026-05-15 09-24-40" src="https://github.com/user-attachments/assets/30037175-a2e9-485b-a290-05a400c169a7" />


#### Penjelasan Diagram Pin IC
Rangkaian ini menggunakan chip IC 74HC32 yang memiliki 4 gerbang OR di dalamnya. Chip IC ini tersedia dalam paket 14 pin dengan tata letak standar.

---

### 3. Gerbang NOT (Inverter)
Gerbang NOT berfungsi membalikkan nilai input (operasi inversi). Jika input bernilai 1 maka output menjadi 0, dan sebaliknya jika input 0 maka output menjadi 1.

#### Komponen yang Digunakan
- Power Supply DC
- IC 74HC04
- LED
- Resistor 220Ω
- DIP Switch

#### Skema Rangkaian & Simulasi
<img width="700" height="494" alt="Screenshot From 2026-05-15 09-29-18" src="https://github.com/user-attachments/assets/66fa91f4-ef76-495e-9c7e-7c1772229bc1" />


#### Penjelasan Diagram Pin IC
IC 74HC04 merupakan chip yang memuat 6 gerbang NOT (inverter) mandiri di dalamnya. Komponen ini adalah salah satu blok bangunan paling dasar dalam elektronik digital dan dikemas dalam bentuk IC 14 pin.

---

### 4. Gerbang NAND
Gerbang NAND (Not AND) merupakan kebalikan langsung dari gerbang AND. Outputnya akan bernilai 0 hanya ketika semua input bernilai 1.

#### Komponen yang Digunakan
- Power Supply DC
- IC 74HC00 (Quad 2-Input NAND Gates)
- LED
- Resistor 220Ω
- DIP Switch

#### Skema Rangkaian & Simulasi
<img width="603" height="494" alt="Screenshot From 2026-05-15 13-26-30" src="https://github.com/user-attachments/assets/06ada1e5-306a-483e-a221-73fc06fe2c63" />


#### Penjelasan Diagram Pin IC
NAND merupakan *inverse* dari gerbang AND, sehingga output pada NAND menghasilkan keadaan yang berlawanan dari AND dengan input yang sama. IC 74HC00 memiliki 14 pin yang komposisinya terdiri dari 4 gerbang NAND.

---

### 5. Gerbang NOR
Gerbang NOR (Not OR) merupakan kebalikan dari gerbang OR. Outputnya akan bernilai 1 hanya jika seluruh input berada pada kondisi rendah (0).

#### Komponen yang Digunakan
- Power Supply DC
- IC 74HC02
- LED
- Resistor 220Ω
- DIP Switch

#### Skema Rangkaian & Simulasi
<img width="603" height="494" alt="Screenshot From 2026-05-15 14-13-32" src="https://github.com/user-attachments/assets/3569ec5d-b84b-484c-83de-ad81e6870174" />


#### Penjelasan Diagram Pin IC
Gerbang NOR akan menghasilkan keadaan yang berlawanan dengan gerbang OR meski diberikan input yang sama. Salah satu IC yang mengimplementasikan konfigurasi ini adalah seri 74HC02 yang membawa 4 gerbang NOR di dalamnya. Note: Perlu diperhatikan bahwa susunan input-output pin pada IC NOR umumnya terbalik dibanding gerbang dasar lainnya.

---

### 6. Gerbang XOR (Exclusive OR)
Gerbang XOR akan menghasilkan output bernilai 1 jika kedua input memiliki kondisi logika yang berbeda. Jika inputnya sama, maka output akan bernilai 0.

#### Komponen yang Digunakan
- Power Supply DC
- IC 74HC86
- LED
- Resistor 220Ω
- DIP Switch

#### Skema Rangkaian & Simulasi
<img width="603" height="494" alt="Screenshot From 2026-05-15 17-02-19" src="https://github.com/user-attachments/assets/4fb12e53-cce0-42bb-8c0a-b125a325a8d3" />


#### Penjelasan Diagram Pin IC
Gerbang XOR bisa diaktifkan apabila salah satu input bernilai 1, namun gerbang XOR akan non-aktif / LOW saat semua input bernilai 1, sehingga gerbang XOR menghilangkan fungsi AND pada gerbang OR. Rangkaian di atas menggunakan IC 74HC86 dengan konfigurasi 4 gerbang XOR mandiri dalam paket 14 pin.

---

### 7. Gerbang XNOR (Exclusive NOR)
Gerbang XNOR menghasilkan output bernilai 1 jika kedua input bernilai sama (keduanya 0 atau keduanya 1).

#### Komponen yang Digunakan
- Power Supply DC
- IC 74HC86 (XOR)
- IC 74HC04 (NOT)
- LED
- Resistor 220Ω
- DIP Switch

#### Skema Rangkaian & Simulasi
<img width="692" height="494" alt="Screenshot From 2026-05-15 17-14-01" src="https://github.com/user-attachments/assets/1e9273e2-c353-4cd5-94cd-ee0d412b6cd0" />


#### Penjelasan Modifikasi Rangkaian
Gerbang XNOR akan memberikan output yang berlawanan dengan gerbang XOR meskipun diberikan kondisi input yang sama. Karena keterbatasan komponen atau tidak adanya chip IC XNOR murni yang tersedia secara default di library Tinkercad, maka fungsi rangkaian XNOR dimanipulasi secara cerdas dengan menggabungkan IC XOR (74HC86) yang kemudian keadaannya di inverse (dibalik) menggunakan gerbang NOT yang terdapat pada IC 74HC04. Kombinasi tersebut berhasil membentuk fungsi gerbang logis XNOR seutuhnya.
