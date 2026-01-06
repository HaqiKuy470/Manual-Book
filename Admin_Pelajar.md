# 📘 **MANUAL BOOK - ARSHAKA BOT **
**Versi Dokumen : 2.1**  
**Dibuat Oleh : Developer Arshaka**  

# 🎯 **BAGIAN 1: PANDUAN ADMIN**

## 1 PANDUAN ADMIN PELAJAR
**Untuk Pengurus Kelas (Ketua, Sekretaris, Bendahara)**

### A. PENGATURAN STRUKTUR (HANYA ADMIN WA/OWNER)
| Command | Fungsi | Catatan |
|---------|--------|---------|
| `.setketua @tag` | Melantik ketua | Admin WA atau Owner |
| `.cekstruktur` | Lihat struktur | Semua bisa lihat |

### B. MANAJEMEN KEUANGAN (HANYA PENGURUS)
| Command | Format | Contoh |
|---------|--------|--------|
| `.addkas` | `.addkas tipe \| nominal \| keterangan` | `.addkas masuk \| 20000 \| Iuran` |
| `.listkas` | Lihat saldo | `.listkas` |

**⚠️ Syarat:** Hanya Ketua, Bendahara, atau Owner

### C. MANAJEMEN TUGAS & JADWAL
| Command | Format | Contoh |
|---------|--------|--------|
| `.addtugas` | `.addtugas Mapel \| Tgl \| Pesan` | `.addtugas MTK \| 20-01-2026 \| PR hal.50` |
| `.deltugas [ID]` | Hapus tugas | `.deltugas TGS-ABC12` |
| `.setjadwal` | `.setjadwal Hari \| Mapel` | `.setjadwal Senin \| MTK, IPA` |
| `.tugas` | Lihat tugas aktif | `.tugas` |

**🔔 Auto-reminder:** Bot ingatkan 24 jam & 6 jam sebelum deadline

### D. ABSENSI HARIAN (SEMUA MEMBER)
| Command | Fungsi | Contoh |
|---------|--------|--------|
| `.hadir` | Absen hadir | `.hadir` |
| `.sakit [alasan]` | Absen sakit | `.sakit demam` |
| `.izin [alasan]` | Absen izin | `.izin ada acara` |
| `.cekabsen` | Lihat absen hari ini | `.cekabsen` |

---
## 1 PANDUAN ADMIN TOOLS & UTILITAS
**Untuk Semua Admin**

### A. CUACA OTOMATIS (HANYA ADMIN WA/OWNER)
| Command | Format | Contoh |
|---------|--------|--------|
| `.setcuaca [lokasi]` | Atur lokasi | `.setcuaca Jakarta` |
| `.delcuaca` | Nonaktifkan | `.delcuaca` |

**🕐 Jadwal:** Auto kirim jam 05:00 pagi

### B. PENGINGAT SHOLAT (HANYA ADMIN WA/OWNER)
| Command | Format | Contoh |
|---------|--------|--------|
| `.setsholat [kota]` | Atur lokasi | `.setsholat Jakarta` |
| `.sholat on/off` | Aktifkan/nonaktifkan | `.sholat on` |
| `.sholat status` | Cek status | `.sholat status` |
| `.jadwalsholat` | Lihat jadwal | `.jadwalsholat` |

**🛡️ Safety:** Auto-skip grup campuran, pesan sopan

### C. REMINDER & TOOLS (SEMUA MEMBER)
| Command | Format | Contoh |
|---------|--------|--------|
| `.ingatkan` | `.ingatkan waktu [pesan]` | `.ingatkan 2h Meeting` |
| `.libur` | Lihat libur nasional | `.libur` |
| `.wiki [topik]` | Cari Wikipedia | `.wiki Soekarno` |
| `.tr [teks]` | Translate EN→ID | `.tr Good morning` |

**⏰ Satuan waktu:** m=menit, j/jam=jam, d=hari, mg=minggu, bln=bulan, thn=tahun

---

## Contact Admin

| Platform | IKontak | Keterangan | Action |
| :---: | :---: | :---: | :---: |
| <img src="https://upload.wikimedia.org/wikipedia/commons/thumb/6/6b/WhatsApp.svg/1200px-WhatsApp.svg.png" width="25"> | `+62 881-0362-71708` | ⚡ **Fast Response** | [**Chat Admin**](https://wa.me/62881036271708) |
| <img src="https://upload.wikimedia.org/wikipedia/commons/thumb/6/6b/WhatsApp.svg/1200px-WhatsApp.svg.png" width="25"> | `+62 857-9228-2715` | 🐢 **Slow Response** | [**Chat Owner**](https://wa.me/6285792282715) |

**© 2026 Arshaka Bot System - Owner: Haqi**  
**Last Updated:** System sesuai dengan semua kode terbaru
