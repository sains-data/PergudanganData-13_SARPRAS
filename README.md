# Data Mart - Sarana dan Prasarana

## Tugas Besar Pergudangan Data - Kelompok 13
**SD25-31007-PergudanganData**

---

##
* `123450005` - EFI DEFIYATI (ETL Developer)
* `123450066` - MUHAMMAD AQIL RAMADHAN (Project Lead)
* `122450091` - TOBIAS DAVID MANOGARI (BI Developer & QA)
* `123450112` - CINDY LAURA MANIK (Database Designer)

---

## Deskripsi Proyek

Proyek data mart ini dirancang untuk menganalisis dan memantau proses bisnis di Unit Sarana dan Prasarana. Tujuannya adalah untuk menyediakan wawasan terkait utilisasi ruangan, inventaris barang, proses perbaikan, dan permintaan fasilitas untuk mendukung pengambilan keputusan oleh pemangku kepentingan seperti Kepala Unit Sarpras dan Kepala Biro Umum.

---

##  Domain Bisnis

Unit Sarana dan Prasarana, yang bertanggung jawab atas pengelolaan aset fisik kampus. Proses bisnis utama yang dianalisis meliputi:
* Manajemen Ruang (pendataan, penjadwalan, kapasitas)
* Inventaris Barang (pendataan per ruang, mutasi, pemeriksaan kondisi)
* Pemeliharaan dan Perbaikan (perawatan rutin, penanganan kerusakan)
* Pengajuan Kebutuhan Fasilitas (penerimaan permintaan, klasifikasi prioritas)
* Monitoring Utilisasi Ruang dan Fasilitas (tingkat pemakaian, ketersediaan)

---

##  Arsitektur

* **Approach:** Kimball (Desain Star/Snowflake Schema)
* **Platform:** SQL Server on Azure VM
* **ETL:** SSIS

---

##  Fitur Utama

* **Fact tables:**
    * `Fact_RoomUsage`
    * `Fact_Repair`
    * `Fact_FacilityRequest`
* **Dimension tables:**
    * `Dim_Room`
    * `Dim_Item`
    * `Dim_Unit`
    * `Dim_Date`
    * (Dan dimensi *snowflaked*: `Dim_Gedung`, `Dim_RoomType`, `Dim_ItemType`, `Dim_KondisiItem`)
* **KPIs:**
    * Tingkat pemanfaatan ruang (room utilization rate)
    * Persentase ketersediaan ruang kelas
    * Tingkat kelayakan fasilitas kampus
    * Waktu respon penanganan perbaikan
    * Persentase penyelesaian laporan kerusakan

---

##  Dokumentasi

* [Business Requirements (Misi 1)](docs/01-requirements/)
* [Design Documents (Misi 1)](docs/02-design/)
* [Laporan Analisis & Dashboard (Misi 3)](docs/03-analysis/)

---

