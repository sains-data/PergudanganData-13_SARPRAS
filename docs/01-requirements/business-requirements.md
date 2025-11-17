
---

# Tugas Besar Pergudangan Data - Misi 1

## UNIT: Sarana dan Prasarana

**Nama Kelompok:**
* EFI DEFIYATI (123450005)
* MUHAMMAD AQIL RAMADHAN (123450066)
* TOBIAS DAVID MANOGARI (122450091)
* CINDY LAURA MANIK (123450112)

---

## MISI 1: DESAIN KONSEPTUAL DAN LOGIKAL

### Step 1: Analisis Kebutuhan Bisnis (Business Requirements Analysis)

**1. Identifikasi Stakeholders**

**1.1 Pengguna Utama Data Mart**
* Kepala Unit Sarana dan Prasarana
* Kepala Bagian Umum
* Staf Administrasi Sarpras
* Unit Perencanaan dan Penganggaran
* Unit Akademik dan Prodi (pengguna ruang kelas/lab)
* Dosen (pemakai ruang kuliah/praktikum)
* Unit Laboratorium dan Studio

**1.2 Pengambil Keputusan (Decision Makers)**
* Kepala Biro Umum dan Perlengkapan
* Kepala Unit Sarana dan Prasarana
* Unit Perencanaan dan Pengembangan

**2. Analisis Proses Bisnis**

**2.1 Proses Bisnis**

**Manajemen Ruang**
* a. Pendataan ruang, kapasitas, dan tipe ruang
* b. Penjadwalan penggunaan ruang
* c. Pemeriksaan kecukupan kapasitas dengan jumlah mahasiswa

**Inventaris Barang**
* a. Pendataan barang per ruangan
* b. Mutasi barang antar ruangan
* c. Pemeriksaan kondisi barang (baik, rusak ringan, rusak berat)

**Pemeliharaan dan Perbaikan**
* a. Perawatan fasilitas secara rutin
* b. Penanganan kerusakan ringan
* c. Pencatatan seluruh aktivitas pemeliharaan

**Pengajuan Kebutuhan Fasilitas**
* a. Penerimaan permintaan fasilitas dari unit/prodi
* b. Klasifikasi kebutuhan berdasarkan tingkat prioritas
* c. Dokumentasi kebutuhan dan status usulan

**Monitoring Utilisasi Ruang dan Fasilitas**
* a. Melihat tingkat pemakaian ruang kelas
* b. Memantau ketersediaan laboratorium
* c. Melihat pola penggunaan fasilitas yang sering digunakan

**2.2 Key Performance Indicators (KPI)**

**2.2.1 KPI Tingkat Institusi**
* Persentase ketersediaan ruang kelas
* Tingkat kelayakan fasilitas kampus
* Tingkat pemanfaatan ruang (room utilization rate)

**2.2.2 KPI Tingkat Unit / Program Studi**
* Rata-rata penggunaan ruang praktikum
* Kesesuaian kapasitas ruang dengan jumlah mahasiswa
* Persentase penyelesaian laporan kerusakan

**2.2.3 KPI Operasional Sarpras**
* Waktu respon penanganan perbaikan
* Jumlah fasilitas rusak per bulan
* Jumlah permintaan fasilitas baru per unit
* Jumlah barang yang mengalami mutasi

**2.3 Kebutuhan Analitik**

**2.3.1 Pertanyaan Analitik yang Akan Dijawab**
* Ruangan mana yang paling sering digunakan?
* Bagaimana tren kondisi barang dari bulan ke bulan?
* Apakah kapasitas ruang sudah sesuai dengan jumlah mahasiswa?
* Berapa banyak laporan perbaikan yang diselesaikan tepat waktu?
* Barang apa saja yang paling sering mengalami kerusakan?

**2.3.2 Laporan yang Diperlukan**
* Dashboard pemanfaatan ruang
* Laporan kondisi fasilitas
* Laporan perawatan dan perbaikan
* Laporan permintaan fasilitas baru
* Laporan mutasi barang

---



### Step 3: Desain Konseptual - ERD

**1. Entitas Utama**
* Room (RoomID, RoomCode, NamaRuang, Kapasitas, TipeRuang, Gedung)
* RoomUsage (UsageID, RoomID, Tanggal, JamMulai, JamSelesai, DigunakanOleh)
* Item (ItemID, NamaItem, JenisItem, Kondisi, RoomID)
* RepairRequest (RepairID, ItemID, TglPengajuan, Status, TglSelesai)
* FacilityRequest (ReqID, Unit, TglPermintaan, Jenis Permintaan, Prioritas, Status)
* ItemMovement (MovementID, ItemID, DariRuangan, KeRuangan, TglMutasi)

**2. Definisi Relationships**
* Room 1-N RoomUsage
* Room 1-N Item
* Item 1-N RepairRequest
* Item 1-N ItemMovement
* FacilityRequest berdiri sendiri (tidak wajib terhubung dengan ruang/barang)

**3. Gambar ERD**
*(Representasi tekstual dari Gambar 3.1)*

**3.1 Deskripsi setiap entitas dan relationship**
Pada gambar 3.1 diagram menggambarkan hubungan antar tabel dalam sistem manajemen fasilitas yang mengatur ruangan, barang, serta aktivitas yang berkaitan dengannya. Tabel rooms berisi informasi dasar mengenai setiap ruangan, seperti kode, nama, kapasitas, tipe ruangan, dan gedung tempat ruangan berada. Setiap ruangan dapat memiliki banyak barang, yang datanya disimpan dalam tabel items. Tabel ini mencatat nama barang, jenis, kondisi, serta ruangan tempat barang tersebut berada. Barang yang tersimpan di ruangan dapat mengalami perpindahan, dan riwayatnya dicatat dalam tabel item_movements, yang menunjukkan barang apa yang dipindahkan, berasal dari ruangan mana, dipindahkan ke ruangan mana, serta tanggal mutasinya. Selain itu, barang juga dapat diajukan untuk perbaikan; proses tersebut direkam dalam tabel repair_requests, yang memuat tanggal pengajuan, status perbaikan, tanggal selesai, dan barang yang mengalami kerusakan. Di sisi lain, penggunaan ruangan dicatat dalam tabel room_usages, yang berisi informasi mengenai tanggal pemakaian, jam mulai, jam selesai, serta siapa pengguna ruangan tersebut. Setiap catatan pemakaian terhubung ke satu ruangan dalam tabel rooms. Terakhir, terdapat tabel facility_requests yang berdiri sendiri dan digunakan untuk menampung permintaan fasilitas dari unit pengaju, seperti jenis permintaan, prioritas, tanggal permintaan, dan statusnya.

**3.2 Dokumen asumsi dan business rules**

**3.2.1 Dokumen asumsi**
1.  Setiap ruangan memiliki informasi lengkap seperti kode ruangan, nama ruangan, kapasitas, tipe ruangan, dan gedung yang bersifat tetap kecuali ada perubahan dari pihak pengelola fasilitas.
2.  Setiap barang (item) pasti berada dalam satu ruangan tertentu, sehingga roomId pada tabel items selalu valid.
3.  Setiap barang hanya memiliki satu kondisi pada satu waktu, misalnya "Baik", "Rusak Ringan", atau "Rusak Berat".
4.  Setiap perbaikan barang (repair_requests) yang tercatat pasti dilakukan terhadap barang yang sudah terdaftar di tabel items.
5.  Setiap mutasi barang (item_movements) diasumsikan dicatat pada tanggal terjadinya perpindahan (tglMutasi).
6.  Data penggunaan ruangan (room_usages) dianggap akurat, sehingga waktu mulai dan waktu selesai sudah sesuai kenyataan.
7.  Setiap penggunaan ruangan hanya untuk satu kegiatan pada satu waktu, sehingga tidak ada dua kegiatan berbeda yang menggunakan ruangan sama di jam yang sama.
8.  Permintaan fasilitas (facility_requests) diajukan oleh unit resmi dan dicatat pada tanggal pengajuan yang valid.
9.  Semua tanggal dan waktu yang dicatat telah mengikuti format standar sistem, misalnya YYYY-MM-DD untuk tanggal.
10. ERD menggambarkan sistem operasional, sehingga setiap tabel menyimpan catatan aktual kegiatan, bukan data historis analisis.

**3.2.2 Business rules**

**A. Aturan Barang dan Mutasi (Items & Item Movements)**
1.  Setiap item harus memiliki roomId yang valid, artinya barang tidak boleh tercatat tanpa ruangan.
2.  Item hanya dapat dipindahkan melalui proses mutasi yang dicatat di tabel item_movements.
3.  Pada saat mutasi terjadi, kondisi barang tetap merujuk pada kondisi terbaru yang tercatat pada tabel items.
4.  Setiap mutasi harus mencatat ruangan asal dan ruangan tujuan, keduanya harus berupa ruangan yang terdaftar.

**B. Aturan Perbaikan Barang (Repair Requests)**
1.  Setiap pengajuan perbaikan harus memiliki itemId yang valid, menunjukkan barang tersebut memang ada di sistem.
2.  Status perbaikan harus mengikuti daftar status standar, seperti: Pending, Diproses, atau Selesai.
3.  Tanggal selesai hanya boleh diisi jika status sudah "Selesai".
4.  Barang yang sedang diperbaiki tetap terikat pada ruangan terakhirnya, kecuali dilakukan mutasi setelah perbaikan.

**C. Aturan Penggunaan Ruangan (Room Usages)**
1.  Setiap penggunaan ruangan harus mengacu pada ruangan yang ada di tabel rooms.
2.  Jam mulai harus lebih awal dari pada jam selesai, dan tidak boleh sama.
3.  Ruangan tidak boleh digunakan oleh dua pihak berbeda dalam waktu yang bertumpuk.
4.  Setiap pemakaian ruangan harus mencantumkan pihak pengguna melalui field digunakanOleh.

**D. Aturan Permintaan Fasilitas (Facility Requests)**
1.  Setiap permintaan fasilitas harus mencantumkan unit dan jenis permintaan, keduanya wajib diisi.
2.  Prioritas harus mengikuti format standar, misalnya: Low, Medium, atau High.
3.  Status permintaan harus mengikuti aturan, seperti: Pending, Diproses, atau Selesai.
4.  Tanggal permintaan tidak boleh kosong, dan menjadi acuan proses pelayanan fasilitas.

**E. Aturan Integritas Relasi**
1.  Semua foreign key harus memiliki referensi yang valid, seperti itemId→ items.id dan roomId→ rooms.id.
2.  Data tidak boleh dihapus jika masih menjadi referensi oleh tabel lain (misalnya barang yang punya riwayat perbaikan tidak bisa dihapus begitu saja).
3.  Tabel items menjadi pusat referensi bagi mutasi dan perbaikan, sehingga setiap perubahan harus konsisten.
4.  Setiap catatan harus mengikuti format tipe data yang ditentukan (misalnya time, date, string, int).

---

### Step 4: Desain Logikal - Dimensional Model (Star Schema)

**1. Tabel Fakta**
* a. **Fact_RoomUsage**
    * RoomUsageKey
    * DateKey
    * RoomKey
    * UnitKey
    * DurationMinutes
    * JenisSesi
* b. **Fact_Repair**
    * RepairKey
    * DateKey
    * ItemKey
    * Status
    * LamaPenyelesaian (hari)
* c. **Fact_FacilityRequest**
    * FacilityReqKey
    * DateKey
    * UnitKey
    * Jenis Permintaan
    * Prioritas
    * Status

**2. Tabel Dimensi**
* Dim_Room - info ruang
* Dim_Item - info barang/fasilitas
* Dim_Unit - info unit/prodi
* Dim_Date - kalender lengkap

**3. Desain Star/Snowflake Schema**
*(Representasi tekstual dari Gambar 4.1)*

Pada gambar 4.1 diagram menunjukkan struktur data berbentuk data warehouse dengan model star schema, yang digunakan untuk menganalisis aktivitas fasilitas, pemakaian ruangan, permintaan fasilitas, dan perbaikan barang. Tabel-tabel berwarna merah merupakan tabel fakta yang menyimpan catatan peristiwa atau aktivitas, sedangkan tabel berwarna lain adalah tabel dimensi yang berisi informasi detail untuk menjelaskan setiap aktivitas. Tabel Fact_Repair menyimpan data mengenai perbaikan barang, seperti barang yang diperbaiki, status, lama waktu penyelesaian, dan tanggalnya. Detail barang tersebut berasal dari tabel Dim_Item, yang berisi informasi lengkap tentang barang, termasuk jenis barang yang diambil dari Dim_ItemType, kondisi barang dari Dim_KondisiItem, serta lokasi ruangannya melalui CurrentRoomKey yang terhubung ke Dim_Room.

Untuk aktivitas penggunaan ruangan, data tersebut dicatat dalam Fact_RoomUsage, yang memuat informasi seperti tanggal penggunaan, lama penggunaan, jenis sesi, ruangan yang digunakan, dan unit yang menggunakan ruangan. Informasi ruangan diambil dari tabel Dim_Room, yang memuat nama ruangan, tipe ruangan, kapasitas, serta gedungnya. Tipe ruangan dijelaskan lebih lanjut di Dim_RoomType, sedangkan nama gedungnya berasal dari Dim_Gedung. Aktivitas lain berupa permintaan fasilitas tercatat dalam Fact_FacilityRequest, yang menyimpan data seperti tanggal permintaan, unit pengaju, jenis permintaan, prioritas, dan status. Unit pengaju diambil dari tabel Dim_Unit. Semua aktivitas yang melibatkan tanggal terhubung ke tabel Dim_Date, yang menyimpan detail waktu seperti hari, bulan, tahun, nama bulan, dan kuartal.

---

### Step 5: Data Dictionary

**1. Tabel Analisis Sumber Data**

**Tabel 5.1**
| Table | Column | Data Type | PK/FK | Description | Business Rule |
| :--- | :--- | :--- | :--- | :--- | :--- |
| Dim_Room | RoomKey | INT | PK | Surrogate key ruangan | Auto-increment |
| Dim_Room | RoomTypeID | INT | FK | Jenis/tipe ruang | Harus ada di Dim_RoomType |
| Dim_Room | RoomCode | VARCHAR(20) | | Kode ruang | Unique, NOT NULL |
| Dim_Room | NamaRuang | VARCHAR(100) | | Nama ruangan | NOT NULL |
| Dim_Room | Kapasitas | INT | | Kapasitas maksimum | > 0 |
| Dim_Room | GedungID | INT | FK | Lokasi gedung | Harus ada di Dim_Gedung |
| Dim_Gedung | GedungID | INT | PK | ID gedung | Auto-increment |
| Dim_Gedung | NamaGedung | VARCHAR(100) | | Nama gedung | NOT NULL |
| Dim_RoomType | RoomTypeID | INT | PK | ID tipe ruangan | Auto-increment |
| Dim_RoomType | NamaTipeRuang | VARCHAR(50) | | Nama tipe ruang | NOT NULL |
| Dim_Item | ItemKey | INT | PK | Surrogate key item | Auto-increment |
| Dim_Item | ItemTypeID | INT | FK | Jenis item | Harus ada di Dim_ItemType |
| Dim_Item | NamaItem | VARCHAR(100) | | Nama barang | NOT NULL |
| Dim_Item | KondisiID | INT | FK | Status kondisi barang | Harus ada di Dim_KondisiItem |
| Dim_Item | CurrentRoomKey | INT | FK | Lokasi ruangan saat ini | Harus ada di Dim_Room |
| Dim_ItemType | ItemTypeID | INT | PK | ID jenis item | Auto-increment |
| Dim_ItemType | NamaJenisItem | VARCHAR(100) | | Nama kategori item | NOT NULL |
| Dim_KondisiItem | KondisiID | INT | PK | ID kondisi | Auto-increment |
| Dim_KondisiItem | Kondisi | VARCHAR(50) | | Nama kondisi barang | (Baik/Rusak/Rusak Berat) |
| Dim_Unit | UnitKey | INT | PK | Surrogate key unit | Auto-increment |
| Dim_Unit | NamaUnit | VARCHAR(100) | | Nama unit/prodi | NOT NULL |
| Dim_Date | DateKey | INT | PK | YYYYMMDD | Derived from FullDate |
| Dim_Date | FullDate | DATE | | Tanggal lengkap | Valid date |
| Dim_Date | Day | INT | | Hari | 1-31 |
| Dim_Date | Month | INT | | Bulan | 1-12 |
| Dim_Date | MonthName | VARCHAR(20) | | Nama bulan | Auto-generate |
| Dim_Date | Quarter | INT | | Kuartal | 1-4 |
| Dim_Date | Year | INT | | Tahun | 4-digit |
| Fact_RoomUsage | RoomUsageKey | INT | PK | Surrogate key | Auto-increment |
| Fact_RoomUsage | DateKey | INT | FK | Tanggal penggunaan | Harus ada di Dim_Date |
| Fact_RoomUsage | RoomKey | INT | FK | Ruang yang dipakai | Harus ada di Dim_Room |
| Fact_RoomUsage | UnitKey | INT | FK | Unit pengguna | Harus ada di Dim_Unit |
| Fact_RoomUsage | DurationMinutes | INT | | Lama penggunaan | >= 0 |
| Fact_RoomUsage | SessionType | VARCHAR(50) | | Jenis pemakaian | (Kuliah/Praktikum/Rapat) |
| Fact_Repair | RepairKey | INT | PK | Surrogate key | Auto-increment |
| Fact_Repair | ItemKey | INT | FK | Barang yang diperbaiki | Harus ada di Dim_Item |
| Fact_Repair | Status | VARCHAR(50) | | Status perbaikan | (Open/Process/Done) |
| Fact_Repair | DaysToComplete | INT | | Lama penyelesaian | |
| Fact_Repair | DateKey | INT | FK | Tanggal laporan | Harus ada di Dim_Date |
| Fact_FacilityRequest | FacilityReqKey | INT | PK | Surrogate key | Auto-increment |
| Fact_FacilityRequest | DateKey | INT | FK | Tanggal permintaan | Harus ada di Dim_Date |
| Fact_FacilityRequest | UnitKey | INT | FK | Unit pemohon | Harus ada di Dim_Unit |
| Fact_FacilityRequest | JenisPermintaan | VARCHAR(100) | | Tipe fasilitas | NOT NULL |
| Fact_FacilityRequest | Prioritas | VARCHAR(20) | | Prioritas | (Rendah/Sedang/Tinggi) |
| Fact_FacilityRequest | Status | VARCHAR(50) | | Status usulan | (Diajukan/Proses/Selesai) |
| ItemMovement | MovementID | INT | PK | Surrogate key | Auto-increment |
| ItemMovement | ItemKey | INT | FK | Barang yang dipindah | Harus ada di Dim_Item |
| ItemMovement | DariRuangan | INT | FK | Ruang asal | Harus ada di Dim_Room |
| ItemMovement | KeRuangan | INT | FK | Ruang tujuan | Harus ada di Dim_Room |
| ItemMovement | TglMutasi | DATE | | Tanggal perpindahan | Valid date |

Pada tabel 5.1, Tabel Dim_Room digunakan untuk menyimpan informasi detail mengenai setiap ruangan yang ada di kampus. Setiap ruangan memiliki RoomKey sebagai identitas unik yang dibuat otomatis. Selain itu, ruangan dikategorikan berdasarkan RoomTypeID yang merujuk ke tabel tipe ruangan. Ruangan juga memiliki RoomCode yang wajib unik dan NamaRuang yang wajib diisi, serta Kapasitas yang menunjukkan jumlah maksimum orang yang dapat ditampung. Setiap ruangan pasti berada dalam sebuah gedung tertentu, sehingga menyertakan GedungID sebagai referensi ke tabel gedung.

Tabel Dim_Gedung berisi daftar seluruh gedung di kampus. Setiap gedung punya GedungID sebagai kunci utama dan NamaGedung sebagai penanda nama gedung tersebut. Sementara itu, tabel Dim_RoomType menyimpan informasi mengenai jenis atau kategori ruangan, seperti ruang kelas, laboratorium, atau studio, lengkap dengan RoomTypeID sebagai kunci utama dan NamaTipeRuang sebagai nama tipenya.

Tabel Dim_Item digunakan untuk mencatat semua barang inventaris yang ada, mulai dari proyektor hingga kursi dan meja. Setiap barang memiliki ItemKey sebagai kunci utama, NamaItem sebagai nama barang, serta ItemTypeID yang menghubungkannya ke tabel jenis barang. Barang juga memiliki KondisiID yang menunjukkan kondisinya (baik, rusak, atau rusak berat) dan CurrentRoomKey yang menunjukkan ruangan tempat barang berada saat ini. Informasi terkait jenis barang tersimpan di tabel Dim_ItemType, yang berisi ItemTypeID dan NamaJenisItem seperti "Elektronik" atau "Furnitur". Sementara itu, kondisi barang disimpan dalam tabel Dim_KondisiItem, yang mencakup daftar kondisi standar seperti "Baik", "Rusak", dan "Rusak Berat".

Tabel Dim_Unit mencatat daftar unit, program studi, ataupun lembaga yang menggunakan fasilitas kampus. Setiap unit memiliki UnitKey dan NamaUnit yang wajib diisi. Untuk kebutuhan tanggal, seluruh data menggunakan tabel Dim_Date sebagai referensi kalender lengkap. Tabel ini menyimpan informasi tanggal secara terstruktur, mulai dari DateKey (dalam format YYYYMMDD), FullDate, hingga atribut tanggal seperti hari, bulan, kuartal, dan tahun.

Pada bagian transaksi, tabel Fact_RoomUsage mencatat setiap kejadian penggunaan ruangan. Informasi yang tersimpan mencakup tanggal penggunaan, ruangan yang digunakan, unit yang menggunakan, durasi penggunaan dalam menit, dan jenis sesi seperti kuliah, praktikum, atau rapat. Selanjutnya, tabel Fact_Repair menyimpan catatan perbaikan barang, termasuk barang yang diperbaiki, status perbaikan (open, process, done), lama penyelesaian, dan tanggal laporan. Tabel Fact_FacilityRequest mencatat permintaan fasilitas dari berbagai unit, mencakup jenis permintaan, prioritas, status, serta unit yang mengajukan permintaan tersebut.

Terakhir, tabel ItemMovement digunakan untuk mencatat proses pemindahan barang antar-ruangan. Setiap catatan perpindahan memuat barang apa yang dipindahkan, ruangan asal dan tujuan, serta tanggal mutasinya. Tabel ini membantu melacak riwayat pergerakan barang sehingga inventaris dapat dipantau secara akurat.