# 📝 Draf Coretan 01: Diskusi Dosen Pembimbing & Jawaban Dasar Penelitian

Dokumen ini berisi rangkuman diskusi dengan Dosen Pembimbing serta jawaban terstruktur terkait pertimbangan studi kasus, penggunaan model Prototyping, dan pemetaan fitur sistem.

---

## ❓ Pertanyaan Dosen Pembimbing

1. **Kenapa Anda mengangkat Studi Kasus ini?**
2. **Seberapa jauh pemahaman Anda tentang Model Prototyping?**
3. **Kenapa pada penelitian ini harus menggunakan Model Prototyping?**
4. **Apa saja rencana fitur yang akan dibangun di dalam sistem ini?**

---

## 💡 Jawaban & Argumentasi Peneliti

### 1. Pertimbangan Pemilihan Studi Kasus
- **Minat Bidang Ilmu**: Ketertarikan kuat dalam bidang Rekayasa Perangkat Lunak (RPL) untuk menyelesaikan permasalahan dunia nyata.
- **Observasi Objek Penelitian**: Berdasarkan pengamatan awal pada Paguyuban Duta Wisata Cak & Ning Surabaya, organisasi belum memiliki sistem terintegrasi untuk mengelola manajemen internal (seperti manajemen penugasan, talent, dan pengajuan kegiatan).
- **Fragmentasi Data**: Data operasional masih tersebar di WhatsApp, Microsoft Excel, Google Sheets, dan Google Form. Hal ini memicu duplikasi data, inkonsistensi, serta menghambat efisiensi proses manajemen organisasi.

---

### 2. Pemahaman & Alur Model Prototyping
- **Fleksibilitas Metode**: Pada tahap awal, *stakeholder* menyerahkan bentuk sistem dan fitur kepada pengembang. Oleh karena itu, diperlukan pendalaman alur bisnis (*business flow*), kebijakan, serta Tugas Pokok dan Fungsi (Tupoksi) masing-masing aktor.
- **Evolusi Model Prototyping (Pressman)**:
  - **Edisi 5**: *Listen to Customer* ➔ *Build Mock-up* ➔ *Customer Test-Drive* ➔ Kembali ke *Listen to Customer*.
  - **Edisi Terbaru**: *Communication* ➔ *Quick Plan* ➔ *Modeling (Quick Design)* ➔ *Construction of Prototype* ➔ *Deployment Delivery & Feedback* ➔ Kembali ke *Communication*.
- **Penerapan dalam Literatur RPL**:
  Prototyping dapat digunakan sebagai *stand-alone process model* maupun teknik dalam konteks model pengembangan lainnya. Tahapan iteratif yang umum digunakan meliputi:
  ```text
  Requirements Gathering ➔ [Iterasi Minimal 1x] ➔ Quick Design ➔ Build Prototype ➔ Customer Evaluation ➔ Review & Update ➔ (Jika belum sesuai: kembali ke Quick Design) ➔ Customer Satisfied ➔ Development ➔ Testing ➔ Maintain
  ```
  *(Catatan: Iterasi dilakukan jika terdapat perubahan skala mayor).*

---

### 3. Alasan Penggunaan Model Prototyping pada Penelitian
- **Rujukan Teoretis (Pressman)**:
  > *"Seringkali pengguna atau pelanggan menetapkan tujuan umum tanpa merinci kebutuhan fungsi dan fitur secara detail. Di sisi lain, pengembang ragu terhadap efisiensi algoritma, adaptasi sistem operasi, atau bentuk interaksi manusia-komputer (IMK) yang tepat. Dalam kondisi tersebut, pendekatan Prototyping merupakan solusi terbaik."*
- **Siklus Keputusan Iteratif**:
  ```mermaid
  graph LR
      A["Menganalisis Kebutuhan"] --> B["Membuat Prototype"]
      B --> C{"Customer Evaluation & Review"}
      C -- "Belum Sesuai" --> A
      C -- "Sesuai" --> D["Membuat Sistem Sesuai Prototype"]
  ```

---

### 4. Pemetaan Fitur Sistem Berdasarkan Peran Pengguna (*Point of View* / PoV)

| Pengguna (Actor) | Fitur Utama (Use Cases) |
| :--- | :--- |
| **Semua Pengguna (All Users)** | • Login & Logout<br>• Ubah Profil<br>• Lihat Notifikasi |
| **Humas** | • Kelola Data Client & Sponsor<br>• Lihat Informasi Talent<br>• Kelola Pengajuan Penugasan |
| **SDM (Diklat)** | • Kelola User & Data Talent<br>• Kelola Penugasan Talent<br>• Validasi Laporan Kegiatan |
| **Talent (Cak & Ning)** | • Lihat Rating Performa & Jam Terbang<br>• Lihat Riwayat Kegiatan & Honor<br>• Konfirmasi Penugasan & Penerimaan Honor<br>• Buat Laporan Penugasan<br>• Update Profil Portofolio & Status Keaktifan |
| **Bendahara** | • Kelola Pembayaran & Rekapitulasi Honor Talent |
| **Guest (Publik)** | • Lihat Profil Organisasi & Informasi Talent<br>• Menghubungi Pihak Pengurus Cak & Ning |