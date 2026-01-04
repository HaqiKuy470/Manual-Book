# Manual-Book
Manual Book Penyewaan Bot
================================================================
          📘 MANUAL BOOK ADMIN - ARSHAKA BOT SYSTEM
Versi Dokumen : 1.0
Dibuat Oleh   : Developer Arshaka
Tujuan        : Panduan Penggunaan Fitur untuk Admin Grup
================================================================

DAFTAR ISI:
1. PANDUAN MODUL PELAJAR (Untuk Ketua/Pengurus Kelas)
2. PANDUAN MODUL BISNIS (Untuk Owner Toko Online)
3. PANDUAN MODUL KOMUNITAS (Untuk Admin Grup Umum)

🎓 1. PANDUAN MODUL PELAJAR
   Fokus: Manajemen Kelas, Absensi, Tugas, dan Kas
================================================================

A. PENGATURAN STRUKTUR KELAS
   Hanya Admin WA atau Owner yang bisa melantik Ketua pertama kali.
   
   1. Melantik Ketua Kelas
      Command: .setketua @tag_member
      Contoh : .setketua @Haqi
   
   2. Melantik Kabinet (Hanya bisa dilakukan oleh Ketua Kelas)
      - Sekretaris : .setsekretaris @tag_member
      - Bendahara  : .setbendahara @tag_member

   3. Kudeta/Turun Jabatan
      - Ketua Resign  : .resign (Dilakukan oleh Ketua sendiri)
      - Voting Turun  : .voteketua (Jika 70% member setuju, ketua lengser)
      - Cek Pejabat   : .cekstruktur

B. MANAJEMEN ABSENSI
   Fitur ini mencatat kehadiran harian secara real-time.

   - Absen Hadir   : .hadir (atau .absen)
   - Absen Sakit   : .sakit [Alasan]
   - Absen Izin    : .izin [Alasan]
   - Cek Harian    : .cekabsen (Lihat siapa yang belum/sudah absen hari ini)
   - Cetak Rekap   : .rekapabsen [Bulan-Tahun] 
                     Contoh: .rekapabsen 01-2026
                     (File CSV akan dikirim ke Private Chat pengurus)

C. MANAJEMEN TUGAS & JADWAL
   Bot akan memberikan reminder otomatis jika deadline tugas < 24 jam.

   1. Tambah Tugas Baru
      Format : .addtugas Mapel | Tanggal(DD-MM-YYYY) | Pesan
      Contoh : .addtugas MTK | 20-01-2026 | Kerjakan LKS Hal 50
   
   2. Lihat & Hapus Tugas
      - Lihat List : .tugas
      - Hapus Tugas: .deltugas [ID_Tugas] (ID didapat dari list .tugas)

   3. Atur Jadwal Pelajaran
      Format : .setjadwal [Hari] | [Mapel]
      Contoh : .setjadwal Senin | Upacara, MTK, B.Indo, IPA
      Cek    : .jadwal (Otomatis menampilkan jadwal hari ini)

D. MANAJEMEN KEUANGAN (KAS)
   Hanya Bendahara, Ketua, atau Owner yang bisa akses.

   1. Input Transaksi
      Format : .addkas [Masuk/Keluar] | [Nominal] | [Keterangan]
      Contoh : .addkas Masuk | 20000 | Iuran Wajib
      Contoh : .addkas Keluar | 15000 | Beli Spidol
   
   2. Cek Saldo
      Command: .listkas (Menampilkan saldo akhir & 10 riwayat terakhir)

💼 2. PANDUAN MODUL BISNIS
   Fokus: Toko Online, Auto-Struk, dan Laporan Keuangan
================================================================

A. PERSIAPAN TOKO (BRANDING)
   Lakukan ini saat pertama kali bot masuk grup.

   1. Set Nama Toko : .settoko [Nama Toko]
   2. Set Website   : .setweb [Link Website/Instagram]
   3. Set Rekening  : .setrek [Info Bank/E-Wallet]
   4. Set QRIS      : Kirim gambar QRIS dengan caption .setqris
   5. Auto Sapaan   : .setwelcome [Kalimat Sambutan]
                      .welcome on (Untuk mengaktifkan fitur sambutan)

B. MANAJEMEN PRODUK (MENU)
   1. Tambah Menu
      Format : .addmenu [Nama Produk] | [Harga]
      Contoh : .addmenu Diamond ML 86 | 20000
   
   2. Lihat Menu (Tampilan Pembeli)
      Command: .listmenu

C. TRANSAKSI & STRUK
   Bot otomatis membuat struk gambar HD (High Definition).

   1. Cara Pembeli Order
      Format : .order [Nomor_Menu]
      Contoh : .order 1, 3 (Memesan menu no 1 dan no 3)
   
   2. Buat Struk Manual (Custom)
      Gunakan ini jika item tidak ada di menu.
      Format : .struk [Item] [Harga] | [Total] | [Metode] | [Nama Pembeli]
      Contoh : .struk Nasi Goreng 15000 | 15000 | TUNAI | Budi

D. LAPORAN & KEAMANAN BISNIS
   1. Cek Omzet
      Command: .laporan (Bot akan mengirim total pendapatan ke Private Chat)
   
   2. Proteksi Grup Jualan
      - Anti Link   : .antilink on (Kirim link grup lain = Hapus pesan)
      - Anti Virtex : .antivirtex on (Kirim teks panjang = Kick)

👥 3. PANDUAN MODUL KOMUNITAS
   Fokus: Keamanan Grup, Sider (Silent Reader), dan Leveling
================================================================

A. FITUR PEMBERSIH SIDER (GHOST SIDER)
   Membersihkan anggota yang tidak aktif chat dalam kurun waktu tertentu.

   1. Aktifkan Fitur
      Command: .sider on
   
   2. Atur Batas Waktu
      Command: .siderdays [Jumlah Hari]
      Contoh : .siderdays 30 (Member diam >30 hari dianggap Sider)

   3. Eksekusi (Kick Massal)
      Command: .kicksider
      (Bot akan scan dulu. Ketik .kicksider confirm untuk menghapus member)

B. MODERASI & KEAMANAN
   1. Anti Toxic
      Command: .antitoxic on (Kick member yang berkata kasar sambil ngetag orang)
   
   2. Anti Link & Izin
      - Aktifkan : .antilink on
      - Beri Izin: .izinkan @tag_member (Member ini bebas kirim link)

C. FITUR MEMBER (INTERAKTIF)
   1. Leveling (XP)
      Setiap chat menambah XP.
      - Cek Level    : .ceklevel
      - Peringkat    : .leaderboard
   
   2. AFK (Away From Keyboard)
      Memberitahu grup jika kamu sedang sibuk.
      - Aktifkan : .afk [Alasan]
      - Matikan  : Kirim pesan apa saja di grup.

================================================================
CATATAN TAMBAHAN:
- Tanda [ ... ] artinya wajib diisi.
- Tanda | adalah pemisah, jangan dihapus.
- Pastikan Bot sudah menjadi Admin Grup agar fitur berjalan lancar.
================================================================
