# 📑 Draf Coretan 02: Panduan Metodologi, Solusi Penulisan & Sistematika BAB I–III

Dokumen ini berisi daftar 12 isu penulisan skripsi beserta jawaban metodologis yang komprehensif, mencakup perbaikan naskah BAB I (Latar Belakang), BAB II (Landasan Teori), dan BAB III (Analisis & Perancangan).

---

## ❓ Daftar 12 Pertanyaan & Isu Penulisan Skripsi

1. **Use Case Description**: Belum ada template standar. Bagaimana bentuk template yang sesuai standar, dan bagaimana penyajiannya per aktor serta per iterasi?
2. **Parafrasa Latar Belakang**: Latar belakang perlu disesuaikan dengan alur permasalahan baru (Fragmentasi Data ➔ Subjektivitas Penugasan ➔ Perhitungan Manual ➔ Pelaporan Tidak Terstruktur).
3. **Subbab 3.1 "Penelitian Sebelumnya"**: Apa landasan metodologis keberadaan subbab ini di BAB III atau sebaiknya dipindah ke BAB II?
4. **Subbab 2.5 "Metode Pengumpulan Data"**: Rangkaian sitasi dan runtutan metodologi (Wawancara Etnografis, Observasi, Studi Dokumentasi) belum terstruktur rapi.
5. **Keterkaitan BAB III dan BAB II**: Bagaimana pola pemanggilan Landasan Teori di BAB II pada setiap tahapan di BAB III?
6. **Rumus Perhitungan Honor Bersih**: Di mana posisi yang tepat untuk memasukkan rumus ini (BAB II atau BAB III)? Apakah ada landasan baku?
7. **Use Case Diagram vs Use Case Description**: Apakah pada tahap *Quick Design* cukup menggunakan diagram saja, atau perlu dipadukan dengan deskripsi tekstual?
8. **Activity Edge Connector (OMG UML)**: Apakah dasar penggunaan konektor ini sudah cukup kuat dan ada rujukan bukunya?
9. **Low-Fidelity Design**: Apakah sampel desain sudah mewakili kebutuhan sistem? Adakah standar jumlah minimalnya?
10. **High-Fidelity Prototype**: Bagaimana standar kelayakan dan perbedaannya dengan Low-Fidelity menurut literatur?
11. **Customer Evaluation & Review/Update**: Apakah prosedur evaluasi dan tabel revisi iterasi pertama sudah sesuai dengan model Pressman?
12. **Standar Development, Testing, & Maintain**: Apa saja standar teknis dan ISO yang relevan untuk tahap akhir ini?

---

## 💡 Jawaban & Solusi Metodologis Komprehensif

### 1. Use Case Description: Template & Pola Penyajian

#### a) Template Standar Use Case Description
Tidak ada format tunggal yang diwajibkan oleh UML (Kulak & Guiney, 2000; Rupp, 2009). Diperlukan konsistensi penggunaan format ringkas namun komprehensif:

| Elemen | Keterangan |
| :--- | :--- |
| **Use Case Name** | Nama Use Case |
| **Unique ID** | Kode unik (misal: UC-01) |
| **Iteration** | Iterasi pengembangan (misal: Iterasi 1) |
| **Summary / Description** | Deskripsi singkat peran dan tujuan Use Case |
| **Primary Actor** | Aktor utama yang menginisiasi Use Case |
| **Supporting Actor** | Aktor pendukung (jika ada) |
| **Preconditions** | Kondisi prasyarat sebelum Use Case dijalankan |
| **Triggers** | Kejadian yang memicu dimulainya Use Case |
| **Basic Course of Events** | Alur utama langkah demi langkah |
| **Alternative Paths** | Alur alternatif (jika terjadi variasi proses) |
| **Exception Paths** | Alur penanganan kesalahan / error |
| **Postconditions** | Kondisi akhir sistem setelah Use Case selesai |
| **Related Business Rules** | Aturan bisnis terkait |

*(Rujukan: Kulak & Guiney, 2000, p. 42; Rupp, 2009, p. 215).*

#### b) Pola Penyajian Per Aktor & Iterasi
Disarankan mengelompokkan subbab per aktor dan iterasi:
- **3.3.1.1 Use Case Description — Iterasi 1**
  - *a) Sisi Guest*
  - *b) Sisi Humas*
  - *c) Sisi SDM (Diklat)*
  - *d) Sisi Talent*
  - *e) Sisi Bendahara*
- **3.3.1.2 Use Case Description — Iterasi 2** *(dst.)*

Setiap aktor cukup menampilkan tabel deskripsi untuk use case yang relevan. Use case umum (Login, Logout, Ubah Profile, Lihat Notifikasi) dapat dikelompokkan dalam satu tabel tersendiri karena polanya sama untuk semua aktor.

#### c) Penambahan pada BAB II
Tambahkan Subbab `2.7.1 Use Case Diagram dan Use Case Description` di BAB II untuk menjelaskan bahwa pemodelan Use Case terdiri dari dua elemen: visual (diagram) dan tekstual (deskripsi). *(Sitasi: Rosa A.S. & Shalahuddin, 2022; Satzinger et al., 2005).*

---

### 2. Parafrasa Latar Belakang (BAB I)

Gunakan narasi yang menghubungkan fenomena digitalisasi organisasi dengan 4 poin permasalahan nyata di Paguyuban Cak & Ning Surabaya:

> Transformasi digital telah berlangsung masif di berbagai sektor. Organisasi kepemudaan dan sosial tidak terkecuali—mereka dituntut mengadopsi teknologi informasi untuk meningkatkan efektivitas operasional, kualitas layanan, dan transparansi manajerial (Sari et al., 2025). Realitas di lapangan menunjukkan bahwa organisasi yang masih mengandalkan pencatatan manual dan platform komunikasi terfragmentasi menghadapi risiko tinggi: duplikasi data, asimetri informasi, dan inefisiensi pengambilan keputusan (Syahrizal, 2025).
>
> Permasalahan tersebut secara spesifik terjadi pada Paguyuban Duta Wisata Cak & Ning Surabaya. Berdasarkan hasil observasi awal, terdapat empat permasalahan utama: (1) **fragmentasi data**—data penugasan, profil anggota, dan finansial tersebar di WhatsApp, Excel, Google Drive, dan Google Form; (2) **subjektivitas penugasan**—plotting talent bergantung pada penilaian subjektif SDM tanpa metrik keaktifan yang terukur; (3) **perhitungan manual**—rekonsiliasi kas dan potongan honor 10% dihitung secara manual sehingga rawan selisih; dan (4) **dokumentasi & pelaporan tidak terstruktur**—laporan kegiatan tersebar di Google Form dan WhatsApp, serta tidak memiliki rekam jejak validasi yang formal.
>
> Untuk mengatasi komplikasi operasional tersebut, diperlukan intervensi strategis melalui perancangan Sistem Informasi Manajemen Talent terpadu berbasis web (Aprilisa & Aulia, 2024). Sistem ini dirancang untuk mendigitalisasi dan mengotomatisasi seluruh alur proses bisnis organisasi, mulai dari pemetaan parameter keaktifan secara objektif, standardisasi penugasan, hingga rekapitulasi finansial secara dinamis. Melalui implementasi basis data terpusat, pengurus dapat mengalokasikan tugas secara adil dan terukur, sementara talent memperoleh otonomi penuh untuk memantau riwayat penugasan melalui platform digital yang terintegrasi (Sari et al., 2025).
>
> Dalam merealisasikan perancangan sistem tersebut, penelitian ini menggunakan model rekayasa perangkat lunak Prototyping. Model ini dipilih karena memiliki keunggulan dalam memfasilitasi pengembangan sistem interaktif yang adaptif terhadap kebutuhan nyata dan fluktuatif dari pengguna akhir (Alfahri et al., 2025). Melalui siklus pembuatan purwarupa yang dievaluasi secara iteratif, metode ini memungkinkan pelibatan pemangku kepentingan secara langsung di fase perancangan awal untuk memvalidasi kelayakan antarmuka dan logika bisnis (Nurhadi & Can, 2024).

---

### 3. Landasan Teori Subbab "3.1 Penelitian Sebelumnya"

- **Analisis Metodologis**: Penempatan *Penelitian Sebelumnya* di BAB III berfungsi sebagai dasar komparatif sebelum peneliti masuk ke analisis dan perancangan sistem.
- **Rekomendasi Struktur**:
  - **Opsi A (Sesuai Konvensi Umum)**: Pindahkan ke BAB II sebagai Subbab `2.x Penelitian Terdahulu (Literature Review)` untuk memetakan *research gap* dan kontribusi kebaruan penelitian *(Sitasi: Sugiyono, 2022; Creswell, 2018)*. Pada BAB III cukup dipanggil kembali: *"Berdasarkan penelitian terdahulu yang telah diuraikan pada subbab 2.x, maka..."*.
  - **Opsi B**: Jika tetap di BAB III, pastikan disajikan dalam bentuk tabel matriks komparasi minimal 3 jurnal rujukan.

---

### 4. Perbaikan Struktur & Sitasi "Metode Pengumpulan Data" (Subbab 2.5)

Restrukturisasi urutan deskripsi agar memiliki kerangka metodologis yang kuat:

```text
2.5 Metode Pengumpulan Data
    ├── 2.5.1 Wawancara Etnografis (Albina & Nasution, 2025)
    ├── 2.5.2 Observasi (Dzikra & Wijaya, 2026)
    └── 2.5.3 Studi Dokumentasi (Widyastuti et al., 2024)
```

- **2.5 Metode Pengumpulan Data (Pengantar)**: Merupakan tahapan krusial dalam rekayasa kebutuhan sistem untuk memperoleh data empiris mengenai operasional objek penelitian *(Sitasi: Sugiyono, 2022; Creswell, 2018)*.
- **2.5.1 Wawancara Etnografis**: Menekankan interaksi langsung dalam konteks alami untuk menggali kebutuhan *tacit* yang tidak muncul dalam wawancara formal *(Albina & Nasution, 2025)*.
- **2.5.2 Observasi**: Pengamatan langsung terhadap sirkulasi administrasi, transaksi keuangan, dan plotting penugasan talent *(Dzikra & Wijaya, 2026)*.
- **2.5.3 Studi Dokumentasi**: Analisis terhadap berkas fisik dan *spreadsheet* internal untuk pemetaan skema basis data *(Dzikra & Wijaya, 2026; Widyastuti et al., 2024)*.

---

### 5. Pola Pemanggilan Landasan Teori (BAB II) di BAB III

Setiap tahapan BAB III wajib merujuk secara eksplisit ke landasan teori di BAB II:
- **3.3.1 Quick Design**: *"Berdasarkan landasan teori pada subbab 2.4.2 mengenai Quick Design, tahap ini bertujuan menerjemahkan kebutuhan teridentifikasi menjadi representasi desain awal sistem..."*
- **3.3.1.1 Use Case Diagram**: *"Sesuai dengan landasan teori pada subbab 2.7.1 mengenai Use Case Diagram, pemodelan ini menyajikan perilaku sistem per aktor..."*
- **3.3.2 Build Prototype**: *"Mengacu pada landasan teori subbab 2.4.3, Build Prototype merupakan pengimplementasian desain cepat ke dalam bentuk purwarupa interaktif..."*
- **3.5 Testing**: *"Berdasarkan landasan teori subbab 2.4.7 mengenai Software Testing, pengujian dilakukan untuk memverifikasi fungsionalitas sistem..."*

---

### 6. Perhitungan Honor Bersih: Posisi di BAB II atau BAB III?

- **Rekomendasi**: Cukup dicantumkan di **BAB III**.
- **Alasan Metodologis**:
  1. Rumus ini bukan rumus baku matematika/statistik (seperti *sigmoid* atau *phi function*), melainkan aturan bisnis (*business rule*) internal organisasi hasil dari wawancara/observasi.
  2. Berfungsi sebagai data empiris proses bisnis dan spesifikasi kebutuhan fungsional (bukan sebagai teori baku).
- **Penguat di BAB II (Opsional)**: Cukup sebutkan prinsip umum otomatisasi keuangan: *"Otomatisasi perhitungan finansial bertujuan mengurangi human error dan meningkatkan transparansi transaksi (Syahrizal, 2025)."*

---

### 7. Penggunaan Use Case Diagram vs Use Case Description

Gunakan **keduanya secara berpasangan**:
1. **Use Case Diagram**: Menyajikan visualisasi hubungan antar-aktor dan batasan sistem (*global overview*).
2. **Use Case Description**: Menyajikan rincian alur kerja tekstual (*Basic Flow, Alternative Flow, Exception Flow*).
- **Landasan BAB II**: Jelaskan kedua notasi ini di subbab `2.7.1` dengan sitasi Rosa A.S. & Shalahuddin (2022) dan Kulak & Guiney (2000).

---

### 8. Penggunaan Activity Edge Connector (OMG UML)

- **Dasar Kekuatan**: Penggunaan *Activity Edge Connector* memiliki landasan ilmiah yang sangat kuat dari sumber primer OMG (Object Management Group).
- **Definisi OMG UML Specification v2.5.1 (p. 375)**:
  > *"An ActivityEdge is a directed connection between two ActivityNodes along which tokens can flow, from the source ActivityNode to the target ActivityNode."*
- **Referensi Buku Rujukan**:
  - OMG. (2017). *Unified Modeling Language (UML) Specification Version 2.5.1*. Object Management Group.
  - Fowler, M. (2003). *UML Distilled: A Brief Guide to the Standard Object Modeling Language (3rd ed.)*. Addison-Wesley.

---

### 9. Kelayakan Low-Fidelity Design

- **Kelayakan Desain**: Pembuatan 3 pola *wireframe* (Form Input, Modal/Pop-up, dan Dashboard) sudah merepresentasikannya secara memadai:
  - *Form*: Mengwakili seluruh halaman pencatatan & pengisian data (CRUD).
  - *Modal*: Mengwakili interaksi responsif & konfirmasi cepat.
  - *Dashboard*: Mengwakili seluruh halaman rekapitulasi & pemantauan data.
- **Standar Jumlah Minimal**: Dalam literatur Usability Engineering, tidak ada kuota jumlah minimal halaman wireframe. Yang utama adalah keterwakilan pola interaksi utama (*Usage-Centered Design*).
- **Referensi Rujukan**:
  - Constantine, L. L., & Lockwood, L. A. D. (1999). *Software for Use: A Practical Guide to the Models and Methods of Usage-Centered Design*. Addison-Wesley.
  - Sanders, E. B.-N., & Stappers, P. J. (2012). *Convivial Toolbox: Generative Research for the Front End of Design*. BIS Publishers.

---

### 10. Kelayakan High-Fidelity Prototype

- **Standardisasi**: Purwarupa berpresisi tinggi (High-Fidelity) menggunakan Figma telah memenuhi standar evaluasi antarmuka karena mencakup aspek tata letak visual, responsivitas warna, komponen terstruktur, dan simulasi interaksi yang menyerupai produk akhir.
- **Rujukan Teoretis**:
  > *"High-fidelity prototypes are detailed representations of designs, including appearance and interaction behavior, allowing users to evaluate complete design details."* (Rettig, 1994; Beaudouin-Lafon & Mackay, 2003).

---

### 11. Customer Evaluation & Review/Update

- **Standardisasi Istilah**: Ganti atau perjelas istilah *"Customer"* menjadi **Pengurus & Talent (Stakeholder Internal)** agar sesuai dengan konteks organisasi non-profit.
- **Kelengkapan Instrumen**: Tambahkan penjelasan bahwa evaluasi menggunakan 3 instrumen:
  1. *Task Scenario Guide* (Panduan Skenario Pengujian).
  2. *Open Interview Guide* (Panduan Wawancara Terbuka).
  3. *Observation Sheet* (Lembar Catatan Evaluasi).
- **Penyambung Narasi**:
  - Pada *Customer Evaluation*: *"Hasil evaluasi ini menjadi dasar revisi pada tahap Review & Update sesuai siklus iteratif Prototyping (Pressman, 2012)."*
  - Pada *Review & Update*: *"Seluruh revisi dipetakan kembali ke tabel masukan dan telah dikonfirmasikan ulang kepada stakeholder."*

---

### 12. Standardisasi Development, Testing, & Maintenance

#### a) Development (Pengembangan)
Arsitektur berbasis MVC (*Model-View-Controller*) dengan *Laravel Framework* (PHP), *MySQL Database*, dan *Tailwind CSS*. Mengacu pada prinsip rekayasa perangkat lunak terstruktur *(Pressman, 2012)*.

#### b) Software Testing (Pengujian)
1. **Black-Box Testing**: Menguji fungsionalitas *input-output* per Use Case (skenario normal, alternatif, dan *boundary*) dengan target keberhasilan 100% *(Pressman, 2012)*.
2. **System Usability Scale (SUS)**: Pengujian persepsi kebergunaan antarmuka menggunakan 10 item kuesioner skala Likert (Brooke, 1996) pada minimal 30 responden *(Sauro & Lewis, 2016)*. Target skor SUS $\ge 70$ (Kategori *"Good"* / Bangor et al., 2009).
3. **Standar Usability International**: Mengacu pada **ISO 9241-11:2018** (*Ergonomics of Human-System Interaction — Usability: Effectiveness, Efficiency, and Satisfaction*).

#### c) Maintenance (Pemeliharaan Sistem)
- **Rencana Operasional Pemeliharaan**:
  - *Pemeliharaan Fungsional*: Perbaikan bug, pembaruan keamanan, dan optimasi performa.
  - *Pemeliharaan Non-Fungsional*: Pembaruan konten, backup otomatis database per 24 jam, dan audit trail aktivitas user.
  - *Masa Pemantauan*: 3 bulan pasca-deploy.
- **Rujukan Standar ISO (Opsional)**: Evaluasi kualitas pemeliharaan merujuk pada aspek *Maintainability* **ISO/IEC 25010:2023** (*modularity, reusability, analysability, modifiability, testability*).

---

## 📚 Matriks Referensi Tambahan & Sitasi Ilmiah

| Topik / Aspek | Penulis & Tahun | Judul Buku / Artikel Ilmiah | Penerbit / Media |
| :--- | :--- | :--- | :--- |
| **Use Case Description** | Kulak, D., & Guiney, E. (2000) | *Use Cases: Requirements in Context* | Addison-Wesley |
| **Requirements Engineering** | Rupp, C. (2009) | *Requirements-Engineering und -Management* | Hanser |
| **Low-Fidelity Wireframing** | Constantine, L. L., & Lockwood, L. A. D. (1999) | *Software for Use: A Practical Guide* | Addison-Wesley |
| **High-Fidelity Prototyping** | Rettig, M. (1994) | *Prototyping for Tiny Fingers* | CACM, 37(4), 21–27 |
| **OMG UML Specification** | OMG (2017) | *Unified Modeling Language (UML) v2.5.1* | Object Management Group |
| **Standard Usability** | ISO (2018) | *ISO 9241-11:2018 Usability Framework* | ISO Standard |
| **System Usability Scale (SUS)** | Sauro, J., & Lewis, J. R. (2016) | *Quantifying the User Experience (2nd ed.)* | Morgan Kaufmann |
| **Software Maintainability** | ISO/IEC (2023) | *ISO/IEC 25010:2023 Systems and Software Quality* | ISO/IEC |