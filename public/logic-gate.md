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
*[Tempat Gambar: Simulasi Rangkaian Gerbang AND]*

#### Penjelasan Diagram Pin IC
Rangkaian ini menggunakan IC 74HC08 (catatan teks dokumen menyebutkan tipe 74HC08 di komponen namun ada referensi ketik manual 74HC04, layout yang benar untuk AND adalah keluarga 7408) yang berisi 4 gerbang AND mandiri. Chip ini dilengkapi dengan paket 14 pin.
*[Tempat Gambar: Diagram Pin IC 7408]*

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
*[Tempat Gambar: Simulasi Rangkaian Gerbang OR]*

#### Penjelasan Diagram Pin IC
Rangkaian ini menggunakan chip IC 74HC32 yang memiliki 4 gerbang OR di dalamnya. Chip IC ini tersedia dalam paket 14 pin dengan tata letak standar.
*[Tempat Gambar: Diagram Pin IC 7432]*

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
*[Tempat Gambar: Simulasi Rangkaian Gerbang NOT]*

#### Penjelasan Diagram Pin IC
IC 74HC04 merupakan chip yang memuat 6 gerbang NOT (inverter) mandiri di dalamnya. Komponen ini adalah salah satu blok bangunan paling dasar dalam elektronik digital dan dikemas dalam bentuk IC 14 pin.
*[Tempat Gambar: Diagram Pin IC 7404]*

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
*[Tempat Gambar: Simulasi Rangkaian Gerbang NAND]*

#### Penjelasan Diagram Pin IC
NAND merupakan *inverse* dari gerbang AND, sehingga output pada NAND menghasilkan keadaan yang berlawanan dari AND dengan input yang sama. IC 74HC00 memiliki 14 pin yang komposisinya terdiri dari 4 gerbang NAND.
*[Tempat Gambar: Diagram Pin IC 7400]*

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
*[Tempat Gambar: Simulasi Rangkaian Gerbang NOR]*

#### Penjelasan Diagram Pin IC
Gerbang NOR akan menghasilkan keadaan yang berlawanan dengan gerbang OR meski diberikan input yang sama. Salah satu IC yang mengimplementasikan konfigurasi ini adalah seri 74HC02 yang membawa 4 gerbang NOR di dalamnya. Note: Perlu diperhatikan bahwa susunan input-output pin pada IC NOR umumnya terbalik dibanding gerbang dasar lainnya.
*[Tempat Gambar: Diagram Pin IC 7402]*

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
*[Tempat Gambar: Simulasi Rangkaian Gerbang XOR]*

#### Penjelasan Diagram Pin IC
Gerbang XOR bisa diaktifkan apabila salah satu input bernilai 1, namun gerbang XOR akan non-aktif / LOW saat semua input bernilai 1, sehingga gerbang XOR menghilangkan fungsi AND pada gerbang OR. Rangkaian di atas menggunakan IC 74HC86 dengan konfigurasi 4 gerbang XOR mandiri dalam paket 14 pin.
*[Tempat Gambar: Diagram Pin IC 7486]*

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
*[Tempat Gambar: Simulasi Rangkaian Gerbang XNOR]*

#### Penjelasan Modifikasi Rangkaian
Gerbang XNOR akan memberikan output yang berlawanan dengan gerbang XOR meskipun diberikan kondisi input yang sama. Karena keterbatasan komponen atau tidak adanya chip IC XNOR murni yang tersedia secara default di library Tinkercad, maka fungsi rangkaian XNOR dimanipulasi secara cerdas dengan menggabungkan IC XOR (74HC86) yang kemudian keadaannya di inverse (dibalik) menggunakan gerbang NOT yang terdapat pada IC 74HC04. Kombinasi tersebut berhasil membentuk fungsi gerbang logis XNOR seutuhnya.
*[Tempat Gambar: Skema Diagram Kombinasi IC 74HC86 & 74HC04]*