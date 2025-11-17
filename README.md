Tentu, berikut adalah konversi Laporan Misi 1 Anda ke dalam format Markdown, lengkap dengan semua bagian, daftar, tabel, dan sitasi sesuai dengan dokumen yang Anda berikan.

---

# [cite_start]Tugas Besar Pergudangan Data - Misi 1 [cite: 1]

## [cite_start]UNIT: Sarana dan Prasarana [cite: 2]

### [cite_start]Nama Kelompok: [cite: 3]
* [cite_start]EFI DEFIYATI (123450005) [cite: 4]
* [cite_start]MUHAMMAD AQIL RAMADHAN (123450066) [cite: 5]
* [cite_start]TOBIAS DAVID MANOGARI (122450091) [cite: 6]
* [cite_start]CINDY LAURA MANIK (123450112) [cite: 7]

---

## [cite_start]MISI 1: DESAIN KONSEPTUAL DAN LOGIKAL [cite: 8]

### [cite_start]Step 1: Analisis Kebutuhan Bisnis (Business Requirements Analysis) [cite: 9]

#### [cite_start]1. Identifikasi Stakeholders [cite: 10]

[cite_start]**1.1 Pengguna Utama Data Mart** [cite: 11]
* [cite_start]Kepala Unit Sarana dan Prasarana [cite: 12]
* [cite_start]Kepala Bagian Umum [cite: 13]
* [cite_start]Staf Administrasi Sarpras [cite: 14]
* [cite_start]Unit Perencanaan dan Penganggaran [cite: 15]
* [cite_start]Unit Akademik dan Prodi (pengguna ruang kelas/lab) [cite: 16]
* [cite_start]Dosen (pemakai ruang kuliah/praktikum) [cite: 17]
* [cite_start]Unit Laboratorium dan Studio [cite: 17]

[cite_start]**1.2 Pengambil Keputusan (Decision Makers)** [cite: 18]
* [cite_start]Kepala Biro Umum dan Perlengkapan [cite: 19]
* [cite_start]Kepala Unit Sarana dan Prasarana [cite: 20]
* [cite_start]Unit Perencanaan dan Pengembangan [cite: 21]

#### [cite_start]2. Analisis Proses Bisnis [cite: 22]

[cite_start]**2.1 Proses Bisnis** [cite: 23]
1.  [cite_start]**Manajemen Ruang** [cite: 24]
    * a. [cite_start]Pendataan ruang, kapasitas, dan tipe ruang [cite: 25]
    * b. [cite_start]Penjadwalan penggunaan ruang [cite: 26]
    * c. [cite_start]Pemeriksaan kecukupan kapasitas dengan jumlah mahasiswa [cite: 27]
2.  [cite_start]**Inventaris Barang** [cite: 28]
    * a. [cite_start]Pendataan barang per ruangan [cite: 29]
    * b. [cite_start]Mutasi barang antar ruangan [cite: 30]
    * c. [cite_start]Pemeriksaan kondisi barang (baik, rusak ringan, rusak berat) [cite: 31]
4.  [cite_start]**Pemeliharaan dan Perbaikan** [cite: 32]
    * a. [cite_start]Perawatan fasilitas secara rutin [cite: 34]
    * b. [cite_start]Penanganan kerusakan ringan [cite: 35]
    * c. [cite_start]Pencatatan seluruh aktivitas pemeliharaan [cite: 36]
5.  [cite_start]**Pengajuan Kebutuhan Fasilitas** [cite: 37]
    * a. [cite_start]Penerimaan permintaan fasilitas dari unit/prodi [cite: 38]
    * b. [cite_start]Klasifikasi kebutuhan berdasarkan tingkat prioritas [cite: 39]
    * c. [cite_start]Dokumentasi kebutuhan dan status usulan [cite: 40]
4.  [cite_start]**Monitoring Utilisasi Ruang dan Fasilitas** [cite: 41]
    * a. [cite_start]Melihat tingkat pemakaian ruang kelas [cite: 42]
    * b. [cite_start]Memantau ketersediaan laboratorium [cite: 43]
    * c. [cite_start]Melihat pola penggunaan fasilitas yang sering digunakan [cite: 44]

[cite_start]**2.2 Key Performance Indicators (KPI)** [cite: 45]
[cite_start]*2.2.1 KPI Tingkat Institusi* [cite: 46]
* [cite_start]Persentase ketersediaan ruang kelas [cite: 47]
* [cite_start]Tingkat kelayakan fasilitas kampus [cite: 48]
* [cite_start]Tingkat pemanfaatan ruang (room utilization rate) [cite: 49]

[cite_start]*2.2.2 KPI Tingkat Unit / Program Studi* [cite: 50]
* [cite_start]Rata-rata penggunaan ruang praktikum [cite: 51]
* [cite_start]Kesesuaian kapasitas ruang dengan jumlah mahasiswa [cite: 52]
* [cite_start]Persentase penyelesaian laporan kerusakan [cite: 53]

[cite_start]*2.2.3 KPI Operasional Sarpras* [cite: 54]
* [cite_start]Waktu respon penanganan perbaikan [cite: 55]
* [cite_start]Jumlah fasilitas rusak per bulan [cite: 55]
* [cite_start]Jumlah permintaan fasilitas baru per unit [cite: 56]
* [cite_start]Jumlah barang yang mengalami mutasi [cite: 56]

[cite_start]**2.3 Kebutuhan Analitik** [cite: 57]
[cite_start]*2.3.1 Pertanyaan Analitik yang Akan Dijawab* [cite: 58]
* [cite_start]Ruangan mana yang paling sering digunakan? [cite: 59]
* [cite_start]Bagaimana tren kondisi barang dari bulan ke bulan? [cite: 60]
* [cite_start]Apakah kapasitas ruang sudah sesuai dengan jumlah mahasiswa? [cite: 61]
* [cite_start]Berapa banyak laporan perbaikan yang diselesaikan tepat waktu? [cite: 62]
* [cite_start]Barang apa saja yang paling sering mengalami kerusakan? [cite: 63]

[cite_start]*2.3.2 Laporan yang Diperlukan* [cite: 64]
* [cite_start]Dashboard pemanfaatan ruang [cite: 65]
* [cite_start]Laporan kondisi fasilitas [cite: 66]
* [cite_start]Laporan perawatan dan perbaikan [cite: 67]
* [cite_start]Laporan permintaan fasilitas baru [cite: 68]
* [cite_start]Laporan mutasi barang [cite: 69]

### [cite_start]Step 2: Identifikasi Sumber Data (Data Source Identification) [cite: 70]

#### [cite_start]1. Sumber Data Utama [cite: 71]
* [cite_start]Sistem Manajemen Ruang (internal kampus) [cite: 73]
* [cite_start]Data Inventaris Sarpras (Excel/Database internal) [cite: 74]
* [cite_start]Formulir pengajuan perbaikan [cite: 75]
* [cite_start]Formulir permintaan fasilitas baru [cite: 76]
* [cite_start]Dokumen mutasi barang [cite: 77]

#### [cite_start]2. Data Source Analysis [cite: 78]

[cite_start]*Tabel 2.1* [cite: 79]

| Sumber Data | Tipe | Tabel Utama | Volume | Frekuensi Update |
| :--- | :--- | :--- | :--- | :--- |
| Sistem Ruang | SQL Server | Rooms, RoomUsage | ~10k | [cite_start]Harian | [cite: 80]
| Inventaris Barang | Excel/DB | Items, ItemStatus | ~50k | [cite_start]Mingguan | [cite: 80]
| Pengajuan Perbaikan | Form Online | RepairRequest | ~5k | [cite_start]Harian | [cite: 80]
| Permintaan Fasilitas | Form Online | FacilityRequest | ~2k | [cite_start]Mingguan | [cite: 81]
| Mutasi Barang | Excel | ItemMovement | kecil | [cite_start]Tidak tentu | [cite: 81]

[cite_start]Pada tabel 2.1 sistem data terdiri dari lima sumber utama yang digunakan untuk mendukung pengelolaan sarana dan prasarana[cite: 82]. [cite_start]Sistem Ruang menggunakan SQL Server sebagai basis data utama, dengan tabel Rooms dan RoomUsage yang menyimpan sekitar 10.000 data dan diperbarui setiap hari untuk memastikan informasi penggunaan ruangan selalu terbaru[cite: 83]. [cite_start]Selanjutnya, Inventaris Barang tersimpan dalam format Excel maupun database, mencakup tabel Items dan ItemStatus dengan volume data cukup besar, yaitu sekitar 50.000 baris, dan diperbarui setiap minggu[cite: 84]. [cite_start]Untuk Pengajuan Perbaikan, data berasal dari formulir online dan disimpan dalam tabel RepairRequest dengan jumlah sekitar 5.000 data yang diperbarui secara harian karena sifatnya yang operasional dan membutuhkan respons cepat[cite: 85]. [cite_start]Permintaan Fasilitas Baru juga dikumpulkan melalui formulir online dan dicatat dalam tabel FacilityRequest, dengan volume sekitar 2.000 data dan diperbarui mingguan[cite: 86]. [cite_start]Terakhir, Mutasi Barang dicatat melalui file Excel pada tabel ItemMovement, dengan jumlah data relatif kecil dan frekuensi yang tidak menentu, tergantung ada atau tidaknya perpindahan barang[cite: 87].

#### [cite_start]3. Data Profiling [cite: 88]
* [cite_start]Periksa NULL pada RoomCode, ConditionStatus [cite: 89]
* [cite_start]Pastikan kapasitas ruang adalah angka positif [cite: 90]
* [cite_start]Cek duplikasi pada ItemID dan RoomUsageID [cite: 90]
* [cite_start]Konsistensi tanggal pemeliharaan [cite: 90]
* [cite_start]Validasi relasi: item.room_id→ rooms.room_id [cite: 91]

### [cite_start]Step 3: Desain Konseptual - ERD [cite: 92]

#### [cite_start]1. Entitas Utama [cite: 93]
* [cite_start]Room (RoomID, RoomCode, NamaRuang, Kapasitas, TipeRuang, Gedung) [cite: 94]
* [cite_start]RoomUsage (UsageID, RoomID, Tanggal, JamMulai, JamSelesai, DigunakanOleh) [cite: 95, 96, 100]
* [cite_start]Item (ItemID, Namaltem, JenisItem, Kondisi, RoomID) [cite: 98]
* [cite_start]RepairRequest (RepairID, ItemID, TglPengajuan, Status, TglSelesai) [cite: 99]
* [cite_start]FacilityRequest (ReqID, Unit, TglPermintaan, Jenis Permintaan, Prioritas, Status) [cite: 101]
* [cite_start]ItemMovement (MovementID, ItemID, DariRuangan, KeRuangan, TglMutasi) [cite: 101]

#### [cite_start]2. Definisi Relationships [cite: 102]
* [cite_start]Room 1-N RoomUsage [cite: 103]
* [cite_start]Room 1-N Item [cite: 104]
* [cite_start]Item 1-N RepairRequest [cite: 105]
* [cite_start]Item 1-N ItemMovement [cite: 106]
* [cite_start]FacilityRequest berdiri sendiri (tidak wajib terhubung dengan ruang/barang) [cite: 107]

#### [cite_start]3. Gambar ERD [cite: 108]
*(Representasi tekstual dari Gambar 3.1)*

[cite_start]**3.1 Deskripsi setiap entitas dan relationship** [cite: 179]
[cite_start]Pada gambar 3.1 diagram menggambarkan hubungan antar tabel dalam sistem manajemen fasilitas yang mengatur ruangan, barang, serta aktivitas yang berkaitan dengannya[cite: 180]. [cite_start]Tabel rooms berisi informasi dasar mengenai setiap ruangan, seperti kode, nama, kapasitas, tipe ruangan, dan gedung tempat ruangan berada[cite: 181]. [cite_start]Setiap ruangan dapat memiliki banyak barang, yang datanya disimpan dalam tabel items[cite: 182]. [cite_start]Tabel ini mencatat nama barang, jenis, kondisi, serta ruangan tempat barang tersebut berada[cite: 183]. [cite_start]Barang yang tersimpan di ruangan dapat mengalami perpindahan, dan riwayatnya dicatat dalam tabel item_movements, yang menunjukkan barang apa yang dipindahkan, berasal dari ruangan mana, dipindahkan ke ruangan mana, serta tanggal mutasinya[cite: 184]. [cite_start]Selain itu, barang juga dapat diajukan untuk perbaikan; proses tersebut direkam dalam tabel repair_requests, yang memuat tanggal pengajuan, status perbaikan, tanggal selesai, dan barang yang mengalami kerusakan[cite: 185]. [cite_start]Di sisi lain, penggunaan ruangan dicatat dalam tabel room_usages, yang berisi informasi mengenai tanggal pemakaian, jam mulai, jam selesai, serta siapa pengguna ruangan tersebut[cite: 186]. [cite_start]Setiap catatan pemakaian terhubung ke satu ruangan dalam tabel rooms[cite: 187]. [cite_start]Terakhir, terdapat tabel facility_requests yang berdiri sendiri dan digunakan untuk menampung permintaan fasilitas dari unit pengaju, seperti jenis permintaan, prioritas, tanggal permintaan, dan statusnya[cite: 188].

[cite_start]**3.2 Dokumen asumsi dan business rules** [cite: 189]
[cite_start]*3.2.1 Dokumen asumsi* [cite: 190]
1.  [cite_start]Setiap ruangan memiliki informasi lengkap seperti kode ruangan, nama ruangan, kapasitas, tipe ruangan, dan gedung yang bersifat tetap kecuali ada perubahan dari pihak pengelola fasilitas[cite: 191].
2.  [cite_start]Setiap barang (item) pasti berada dalam satu ruangan tertentu, sehingga roomId pada tabel items selalu valid[cite: 192].
3.  [cite_start]Setiap barang hanya memiliki satu kondisi pada satu waktu, misalnya "Baik", "Rusak Ringan", atau "Rusak Berat"[cite: 193].
4.  [cite_start]Setiap perbaikan barang (repair_requests) yang tercatat pasti dilakukan terhadap barang yang sudah terdaftar di tabel items[cite: 194].
5.  [cite_start]Setiap mutasi barang (item_movements) diasumsikan dicatat pada tanggal terjadinya perpindahan (tglMutasi)[cite: 195].
6.  [cite_start]Data penggunaan ruangan (room_usages) dianggap akurat, sehingga waktu mulai dan waktu selesai sudah sesuai kenyataan[cite: 196].
7.  [cite_start]Setiap penggunaan ruangan hanya untuk satu kegiatan pada satu waktu, sehingga tidak ada dua kegiatan berbeda yang menggunakan ruangan sama di jam yang sama[cite: 197].
8.  [cite_start]Permintaan fasilitas (facility_requests) diajukan oleh unit resmi dan dicatat pada tanggal pengajuan yang valid[cite: 198].
9.  [cite_start]Semua tanggal dan waktu yang dicatat telah mengikuti format standar sistem, misalnya YYYY-MM-DD untuk tanggal[cite: 199].
10. [cite_start]ERD menggambarkan sistem operasional, sehingga setiap tabel menyimpan catatan aktual kegiatan, bukan data historis analisis[cite: 200].

[cite_start]*3.2.1 Business rules* [cite: 201]
[cite_start]A.  **Aturan Barang dan Mutasi (Items & Item Movements)** [cite: 202]
    1.  [cite_start]Setiap item harus memiliki roomId yang valid, artinya barang tidak boleh tercatat tanpa ruangan[cite: 203].
    2.  [cite_start]Item hanya dapat dipindahkan melalui proses mutasi yang dicatat di tabel item_movements[cite: 204].
    3.  [cite_start]Pada saat mutasi terjadi, kondisi barang tetap merujuk pada kondisi terbaru yang tercatat pada tabel items[cite: 205].
    4.  [cite_start]Setiap mutasi harus mencatat ruangan asal dan ruangan tujuan, keduanya harus berupa ruangan yang terdaftar[cite: 206].
[cite_start]B.  **Aturan Perbaikan Barang (Repair Requests)** [cite: 207]
    1.  [cite_start]Setiap pengajuan perbaikan harus memiliki itemId yang valid, menunjukkan barang tersebut memang ada di sistem[cite: 208].
    2.  [cite_start]Status perbaikan harus mengikuti daftar status standar, seperti: Pending, Diproses, atau Selesai[cite: 209].
    3.  [cite_start]Tanggal selesai hanya boleh diisi jika status sudah "Selesai"[cite: 210].
    4.  [cite_start]Barang yang sedang diperbaiki tetap terikat pada ruangan terakhirnya, kecuali dilakukan mutasi setelah perbaikan[cite: 211, 212].
[cite_start]C.  **Aturan Penggunaan Ruangan (Room Usages)** [cite: 213]
    1.  [cite_start]Setiap penggunaan ruangan harus mengacu pada ruangan yang ada di tabel rooms[cite: 214].
    2.  [cite_start]Jam mulai harus lebih awal dari pada jam selesai, dan tidak boleh sama[cite: 215].
    3.  [cite_start]Ruangan tidak boleh digunakan oleh dua pihak berbeda dalam waktu yang bertumpuk[cite: 216].
    4.  [cite_start]Setiap pemakaian ruangan harus mencantumkan pihak pengguna melalui field digunakanOleh[cite: 217].
[cite_start]D.  **Aturan Permintaan Fasilitas (Facility Requests)** [cite: 218]
    1.  [cite_start]Setiap permintaan fasilitas harus mencantumkan unit dan jenis permintaan, keduanya wajib diisi[cite: 219].
    2.  [cite_start]Prioritas harus mengikuti format standar, misalnya: Low, Medium, atau High[cite: 220].
    3.  [cite_start]Status permintaan harus mengikuti aturan, seperti: Pending, Diproses, atau Selesai[cite: 221].
    4.  [cite_start]Tanggal permintaan tidak boleh kosong, dan menjadi acuan proses pelayanan fasilitas[cite: 222].
[cite_start]E.  **Aturan Integritas Relasi** [cite: 223]
    1.  [cite_start]Semua foreign key harus memiliki referensi yang valid, seperti itemId→ items.id dan roomId→ rooms.id[cite: 224].
    2.  [cite_start]Data tidak boleh dihapus jika masih menjadi referensi oleh tabel lain (misalnya barang yang punya riwayat perbaikan tidak bisa dihapus begitu saja)[cite: 225].
    3.  [cite_start]Tabel items menjadi pusat referensi bagi mutasi dan perbaikan, sehingga setiap perubahan harus konsisten[cite: 226].
    4.  [cite_start]Setiap catatan harus mengikuti format tipe data yang ditentukan (misalnya time, date, string, int)[cite: 227].

### [cite_start]Step 4: Desain Logikal - Dimensional Model (Star Schema) [cite: 228]

#### [cite_start]1. Tabel Fakta [cite: 229]
a.  [cite_start]**Fact_RoomUsage** [cite: 230]
    * [cite_start]RoomUsageKey [cite: 231]
    * [cite_start]DateKey [cite: 232]
    * [cite_start]RoomKey [cite: 233]
    * [cite_start]UnitKey [cite: 234]
    * [cite_start]DurationMinutes [cite: 235]
    * [cite_start]JenisSesi [cite: 236]
b.  [cite_start]**Fact_Repair** [cite: 237]
    * [cite_start]RepairKey [cite: 238]
    * [cite_start]DateKey [cite: 239]
    * [cite_start]ItemKey [cite: 240]
    * [cite_start]Status [cite: 242]
    * [cite_start]LamaPenyelesaian (hari) [cite: 243]
c.  [cite_start]**Fact_FacilityRequest** [cite: 244]
    * [cite_start]FacilityReqKey [cite: 246]
    * [cite_start]DateKey [cite: 247]
    * [cite_start]UnitKey [cite: 248]
    * [cite_start]Jenis Permintaan [cite: 249]
    * [cite_start]Prioritas [cite: 250]
    * [cite_start]Status [cite: 251]

#### [cite_start]2. Tabel Dimensi [cite: 252]
* [cite_start]Dim_Room - info ruang [cite: 253, 254]
* [cite_start]Dim_Item - info barang/fasilitas [cite: 255, 256]
* [cite_start]Dim_Unit - info unit/prodi [cite: 257]
* [cite_start]Dim_Date - kalender lengkap [cite: 258, 259]

#### [cite_start]3. Desain Star/Snowflake Schema [cite: 260]
*(Representasi tekstual dari Gambar 4.1)*

[cite_start]Pada gambar 4.1 diagram menunjukkan struktur data berbentuk data warehouse dengan model star schema, yang digunakan untuk menganalisis aktivitas fasilitas, pemakaian ruangan, permintaan fasilitas, dan perbaikan barang[cite: 321]. [cite_start]Tabel-tabel berwarna merah merupakan tabel fakta yang menyimpan catatan peristiwa atau aktivitas, sedangkan tabel berwarna lain adalah tabel dimensi yang berisi informasi detail untuk menjelaskan setiap aktivitas[cite: 322]. [cite_start]Tabel Fact_Repair menyimpan data mengenai perbaikan barang, seperti barang yang diperbaiki, status, lama waktu penyelesaian, dan tanggalnya[cite: 323]. [cite_start]Detail barang tersebut berasal dari tabel Dim_Item, yang berisi informasi lengkap tentang barang, termasuk jenis barang yang diambil dari Dim_ItemType, kondisi barang dari Dim_Kondisiltem, serta lokasi ruangannya melalui CurrentRoomKey yang terhubung ke Dim_Room[cite: 324].

[cite_start]Untuk aktivitas penggunaan ruangan, data tersebut dicatat dalam Fact_RoomUsage, yang memuat informasi seperti tanggal penggunaan, lama penggunaan, jenis sesi, ruangan yang digunakan, dan unit yang menggunakan ruangan[cite: 327]. [cite_start]Informasi ruangan diambil dari tabel Dim_Room, yang memuat nama ruangan, tipe ruangan, kapasitas, serta gedungnya[cite: 328]. [cite_start]Tipe ruangan dijelaskan lebih lanjut di Dim_RoomType, sedangkan nama gedungnya berasal dari Dim_Gedung[cite: 329]. [cite_start]Aktivitas lain berupa permintaan fasilitas tercatat dalam Fact_FacilityRequest, yang menyimpan data seperti tanggal permintaan, unit pengaju, jenis permintaan, prioritas, dan status[cite: 330]. [cite_start]Unit pengaju diambil dari tabel Dim_Unit[cite: 331]. [cite_start]Semua aktivitas yang melibatkan tanggal terhubung ke tabel Dim_Date, yang menyimpan detail waktu seperti hari, bulan, tahun, nama bulan, dan kuartal[cite: 331].

### [cite_start]Step 5: Data Dictionary [cite: 332]

#### [cite_start]1. Tabel Analisis Sumber Data [cite: 333]

[cite_start]*Tabel 5.1* [cite: 334]

| Table | Column | Data Type | PK/FK | Description | Business Rule |
| :--- | :--- | :--- | :--- | :--- | :--- |
| Dim_Room | RoomKey | INT | PK | Surrogate key ruangan | [cite_start]Auto-increment | [cite: 338, 339, 340, 341, 343, 344]
| Dim_Room | RoomTypeID | INT | FK | Jenis/tipe ruang | [cite_start]Harus ada di Dim_RoomType | [cite: 345, 346, 347, 348, 349, 350]
| Dim_Room | RoomCode | VARCHAR(20) | | Kode ruang | [cite_start]Unique, NOT NULL | [cite: 351, 352, 353, 354, 355, 356]
| Dim_Room | NamaRuang | VARCHAR(100) | | Nama ruangan | [cite_start]NOT NULL | [cite: 357, 358, 361, 362, 359, 363, 360]
| Dim_Room | Kapasitas | INT | | Kapasitas maksimum | > [cite_start]0 | [cite: 364, 365, 366, 367]
| Dim_Room | GedungID | INT | FK | Lokasi gedung | [cite_start]Harus ada di Dim_Gedung | [cite: 368, 369, 370, 371, 372, 373]
| Dim_Gedung | GedungID | INT | PK | ID gedung | [cite_start]Auto-increment | [cite: 377, 378, 374, 375, 376]
| Dim_Gedung | NamaGedung | VARCHAR(100) | | Nama gedung | [cite_start]NOT NULL | [cite: 379, 380, 381, 384, 386]
| Dim_RoomType | RoomTypeID | INT | PK | ID tipe ruangan | [cite_start]Auto-increment | [cite: 383, 385, 387]
| Dim_RoomType | NamaTipeRuang | VARCHAR(50) | | Nama tipe ruang | [cite_start]NOT NULL | [cite: 392, 393, 394]
| Dim_Item | ItemKey | INT | PK | Surrogate key item | [cite_start]Auto-increment | [cite: 395, 396, 397, 398, 399]
| Dim_Item | ItemTypeID | INT | FK | Jenis item | [cite_start]Harus ada di Dim_ItemType | [cite: 400, 401, 402, 403, 404, 405]
| Dim_Item | NamaItem | VARCHAR(100) | | Nama barang | [cite_start]NOT NULL | [cite: 406, 407, 411, 412, 409, 413, 410]
| Dim_Item | KondisiID | INT | FK | Status kondisi barang | [cite_start]Harus ada di Dim_KondisiItem | [cite: 414, 415, 420, 416, 417, 418, 421, 423, 419, 422, 424]
| Dim_Item | CurrentRoomKey | INT | FK | Lokasi ruangan saat ini | [cite_start]Harus ada di Dim_Room | [cite: 425, 426, 430, 427, 428, 431, 433, 429, 432]
| Dim_ItemType | ItemTypeID | INT | PK | ID jenis item | [cite_start]Auto-increment | [cite: 434, 437, 435, 438, 436, 439, 440]
| Dim_ItemType | NamaJenisItem | VARCHAR(100) | | Nama kategori item | [cite_start]NOT NULL | [cite: 441, 442, 445, 446, 443, 447, 444]
| Dim_KondisiItem | KondisiID | INT | PK | ID kondisi | [cite_start]Auto-increment | [cite: 448, 452, 453, 449, 450, 451]
| Dim_KondisiItem | Kondisi | VARCHAR(50) | | Nama kondisi barang | (Baik/Rusak/Rusak Berat) [cite_start]| [cite: 454, 456, 455, 457, 458, 460, 459]
| Dim_Unit | UnitKey | INT | PK | Surrogate key unit | [cite_start]Auto-increment | [cite: 461, 462, 463, 464, 465, 466]
| Dim_Unit | NamaUnit | VARCHAR(100) | | Nama unit/prodi | [cite_start]NOT NULL | [cite: 467, 468, 472, 469, 470, 474, 471]
| Dim_Date | DateKey | INT | PK | YYYYMMDD | [cite_start]Derived from FullDate | [cite: 475, 476, 477, 478, 479, 481, 480, 482]
| Dim_Date | FullDate | DATE | | Tanggal lengkap | [cite_start]Valid date | [cite: 483, 484, 485, 487, 486]
| Dim_Date | Day | INT | | Hari | [cite_start]1-31 | [cite: 488]
| Dim_Date | Month | INT | | Bulan | [cite_start]1-12 | [cite: 488]
| Dim_Date | MonthName | VARCHAR(20) | | Nama bulan | [cite_start]Auto-generate | [cite: 488]
| Dim_Date | Quarter | INT | | Kuartal | [cite_start]1-4 | [cite: 488]
| Dim_Date | Year | INT | | Tahun | [cite_start]4-digit | [cite: 488]
| Fact_RoomUsage | RoomUsageKey | INT | PK | Surrogate key | [cite_start]Auto-increment | [cite: 488]
| Fact_RoomUsage | DateKey | INT | FK | Tanggal penggunaan | [cite_start]Harus ada di Dim_Date | [cite: 488]
| Fact_RoomUsage | RoomKey | INT | FK | Ruang yang dipakai | [cite_start]Harus ada di Dim_Room | [cite: 488]
| Fact_RoomUsage | UnitKey | INT | FK | Unit pengguna | [cite_start]Harus ada di Dim_Unit | [cite: 488]
| Fact_RoomUsage | DurationMinutes | INT | | Lama penggunaan | [cite_start]$\ge0$ | [cite: 488]
| Fact_RoomUsage | SessionType | VARCHAR(50) | | Jenis pemakaian | [cite_start]Kuliah/Praktikum/Rapat | [cite: 488]
| Fact_Repair | RepairKey | INT | PK | Surrogate key | [cite_start]Auto-increment | [cite: 488]
| Fact_Repair | ItemKey | INT | FK | Barang yang diperbaiki | [cite_start]Harus ada di Dim_Item | [cite: 488]
| Fact_Repair | Status | VARCHAR(50) | | Status perbaikan | [cite_start]Open/Process/Done | [cite: 488]
| Fact_Repair | DaysToComplete | INT | | Lama penyelesaian | [cite_start]| [cite: 488]
| Fact_Repair | DateKey | INT | FK | Tanggal laporan | [cite_start]Harus ada di Dim_Date | [cite: 488]
| Fact_FacilityRequest | FacilityReqKey | INT | PK | Surrogate key | [cite_start]Auto-increment | [cite: 489]
| Fact_FacilityRequest | DateKey | INT | FK | Tanggal permintaan | [cite_start]Harus ada di Dim_Date | [cite: 489]
| Fact_FacilityRequest | UnitKey | INT | FK | Unit pemohon | [cite_start]Harus ada di Dim_Unit | [cite: 489]
| Fact_FacilityRequest | JenisPermintaan | VARCHAR(100) | | Tipe fasilitas | [cite_start]NOT NULL | [cite: 489]
| Fact_FacilityRequest | Prioritas | VARCHAR(20) | | Prioritas | [cite_start]Rendah/Sedang/Tinggi | [cite: 489]
| Fact_FacilityRequest | Status | VARCHAR(50) | | Status usulan | [cite_start]Diajukan/Proses/Selesai | [cite: 489]
| ItemMovement | MovementID | INT | PK | Surrogate key | [cite_start]Auto-increment | [cite: 489]
| ItemMovement | ItemKey | INT | FK | Barang yang dipindah | [cite_start]Harus ada di Dim_Item | [cite: 489]
| ItemMovement | DariRuangan | INT | FK | Ruang asal | [cite_start]Harus ada di Dim_Room | [cite: 489]
| ItemMovement | KeRuangan | INT | FK | Ruang tujuan | [cite_start]Harus ada di Dim_Room | [cite: 489]
| ItemMovement | TglMutasi | DATE | | Tanggal perpindahan | [cite_start]Valid date | [cite: 489]

[cite_start]Pada tabel 5.1 Tabel Dim_Room digunakan untuk menyimpan informasi detail mengenai setiap ruangan yang ada di kampus[cite: 490]. [cite_start]Setiap ruangan memiliki RoomKey sebagai identitas unik yang dibuat otomatis[cite: 491]. [cite_start]Selain itu, ruangan dikategorikan berdasarkan RoomTypeID yang merujuk ke tabel tipe ruangan[cite: 492]. [cite_start]Ruangan juga memiliki RoomCode yang wajib unik dan NamaRuang yang wajib diisi, serta Kapasitas yang menunjukkan jumlah maksimum orang yang dapat ditampung[cite: 493]. [cite_start]Setiap ruangan pasti berada dalam sebuah gedung tertentu, sehingga menyertakan GedungID sebagai referensi ke tabel gedung[cite: 494].

[cite_start]Tabel Dim_Gedung berisi daftar seluruh gedung di kampus[cite: 495]. [cite_start]Setiap gedung punya GedungID sebagai kunci utama dan NamaGedung sebagai penanda nama gedung tersebut[cite: 495]. [cite_start]Sementara itu, tabel Dim_RoomType menyimpan informasi mengenai jenis atau kategori ruangan, seperti ruang kelas, laboratorium, atau studio, lengkap dengan RoomTypeID sebagai kunci utama dan NamaTipeRuang sebagai nama tipenya[cite: 496].

[cite_start]Tabel Dim_Item digunakan untuk mencatat semua barang inventaris yang ada, mulai dari proyektor hingga kursi dan meja[cite: 497]. [cite_start]Setiap barang memiliki ItemKey sebagai kunci utama, Namaltem sebagai nama barang, serta ItemTypeID yang menghubungkannya ke tabel jenis barang[cite: 498]. [cite_start]Barang juga memiliki KondisiID yang menunjukkan kondisinya (baik, rusak, atau rusak berat) dan CurrentRoomKey yang menunjukkan ruangan tempat barang berada saat ini[cite: 499]. [cite_start]Informasi terkait jenis barang tersimpan di tabel Dim_ItemType, yang berisi ItemTypeID dan NamaJenisItem seperti "Elektronik" atau "Furnitur"[cite: 500]. [cite_start]Sementara itu, kondisi barang disimpan dalam tabel Dim_Kondisiltem, yang mencakup daftar kondisi standar seperti "Baik", "Rusak", dan "Rusak Berat"[cite: 501].

[cite_start]Tabel Dim_Unit mencatat daftar unit, program studi, ataupun lembaga yang menggunakan fasilitas kampus[cite: 502]. [cite_start]Setiap unit memiliki UnitKey dan NamaUnit yang wajib diisi[cite: 503]. [cite_start]Untuk kebutuhan tanggal, seluruh data menggunakan tabel Dim_Date sebagai referensi kalender lengkap[cite: 503]. [cite_start]Tabel ini menyimpan informasi tanggal secara terstruktur, mulai dari DateKey (dalam format YYYYMMDD), FullDate, hingga atribut tanggal seperti hari, bulan, kuartal, dan tahun[cite: 504].

[cite_start]Pada bagian transaksi, tabel Fact_RoomUsage mencatat setiap kejadian penggunaan ruangan[cite: 505]. [cite_start]Informasi yang tersimpan mencakup tanggal penggunaan, ruangan yang digunakan, unit yang menggunakan, durasi penggunaan dalam menit, dan jenis sesi seperti kuliah, praktikum, atau rapat[cite: 506]. [cite_start]Selanjutnya, tabel Fact_Repair menyimpan catatan perbaikan barang, termasuk barang yang diperbaiki, status perbaikan (open, process, done), lama penyelesaian, dan tanggal laporan[cite: 507]. [cite_start]Tabel Fact_FacilityRequest mencatat permintaan fasilitas dari berbagai unit, mencakup jenis permintaan, prioritas, status, serta unit yang mengajukan permintaan tersebut[cite: 508].

[cite_start]Terakhir, tabel ItemMovement digunakan untuk mencatat proses pemindahan barang antar-ruangan[cite: 509]. [cite_start]Setiap catatan perpindahan memuat barang apa yang dipindahkan, ruangan asal dan tujuan, serta tanggal mutasinya[cite: 510]. [cite_start]Tabel ini membantu melacak riwayat pergerakan barang sehingga inventaris dapat dipantau secara akurat[cite: 511].

### [cite_start]Step 6: GitHub Repository Setup [cite: 512]