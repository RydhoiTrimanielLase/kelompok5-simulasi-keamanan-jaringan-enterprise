# 🔐 Simulasi Keamanan Jaringan Enterprise
### Project Based Learning — Jaringan Komputer dan Komunikasi Data
**Teknik Informatika · Universitas Maritim Raja Ali Haji · T.A 2025/2026**

---

## 👥 Kelompok 5

| No | Nama | NIM |
|----|------|-----|
| 1 | Nurpaisyah | 2401020063 |
| 2 | Syhara Suheti | 2401020067 |
| 3 | Septia Dwi Ananta | 2401020074 |
| 4 | Gelia Rahma | 2401020092 |
| 5 | Rydhoi Trimaniel Lase | 2401020061 |

---

## 📋 Deskripsi Proyek

Proyek ini mensimulasikan **keamanan jaringan enterprise** pada perusahaan fiktif **PT. Nusantara Teknologi** menggunakan GNS3 dan Virtual Machine. Jaringan dibagi menjadi beberapa segmen berdasarkan divisi perusahaan, dengan penerapan ACL, Firewall, dan kebijakan akses antar segmen untuk membatasi komunikasi sesuai kebutuhan keamanan.

---

## 🏗️ Topologi Jaringan

| Perangkat | Keterangan |
|-----------|-----------|
| 1 Router | Core routing |
| 1 Firewall | ACL & policy enforcement |
| 5 Switch | Per segmen divisi |
| 5 Linux PC | IT Admin (×5) |
| 30 Windows Client | Keuangan (×10), HRD (×10), Operasional (×15) — representasi |
| 3 Ubuntu Server | Web Server, DB Server, File Server |

![Topologi Jaringan](https://raw.githubusercontent.com/RydhoiTrimanielLase/kelompok5-simulasi-keamanan-jaringan-enterprise/main/topologi.jpeg)

📎 **[Lihat/edit file topologi (.drawio)](https://github.com/RydhoiTrimanielLase/kelompok5-simulasi-keamanan-jaringan-enterprise/blob/main/topologi.drawio)**

---

## 🌐 IP Plan & Subnetting

Network induk: `192.168.10.0/24`

| Segmen | Subnet | Range IP | Host Tersedia |
|--------|--------|----------|---------------|
| IT Admin | 192.168.10.0/27 | .1 – .30 | 30 |
| Keuangan | 192.168.10.32/28 | .33 – .46 | 14 |
| Server Farm | 192.168.10.64/29 | .65 – .70 | 6 |
| HRD | 192.168.10.80/28 | .81 – .94 | 14 |
| Operasional | 192.168.10.96/28 | .97 – .110 | 14 |

---

## 🔒 Kebijakan Akses (ACL)

| Divisi | Hak Akses |
|--------|-----------|
| IT Admin | Akses ke **semua** segmen |
| Keuangan | Hanya ke **Server Farm** |
| HRD | Hanya ke **Server Farm** |
| Operasional | Hanya ke **Web Server** |

---

## 🧰 Tools & Teknologi

![GNS3](https://img.shields.io/badge/GNS3-Simulator-blue)
![Ubuntu](https://img.shields.io/badge/Ubuntu-Server-orange)
![Windows](https://img.shields.io/badge/Windows-Client-blue)

- **GNS3** — simulasi router dan switch
- **Ubuntu Server** — Linux Server (Web, DB, File)
- **Windows Client** — end device divisi
- **Draw.io** — diagram topologi
- **ACL & Firewall** — kebijakan keamanan jaringan

---

## 📁 Struktur Repository

```
kelompok5-simulasi-keamanan-jaringan-enterprise/
│
├── README.md
│
├── Progress-1/
│   ├── proposal.pdf          ← Proposal & analisis kebutuhan
│   ├── topologi.png          ← Gambar topologi jaringan
│   └── topologi.drawio       ← File Draw.io (editable)
│
├── Progress-2/               ← (akan diisi)
├── Progress-3/               ← (akan diisi)
└── Final/                    ← (akan diisi)
```

---

## 📅 Jadwal Progress

| Tahap | Deadline | Status |
|-------|----------|--------|
| Progress 1 | 13 Juni 2026, 21.00 WIB | 🟡 In Progress |
| Progress 2 | 20 Juni 2026, 21.00 WIB | ⬜ Belum |
| Progress 3 | 27 Juni 2026, 21.00 WIB | ⬜ Belum |
| Final | 01 & 03 Juli 2026 | ⬜ Belum |

---

## 📌 Kompetensi yang Dipelajari

- Access Control List (ACL)
- Firewall & kebijakan keamanan
- Segmentasi jaringan
- Subnetting (VLSM)
- Konfigurasi GNS3 + VM

---

> **Mata Kuliah:** Jaringan Komputer dan Komunikasi Data  
> **Program Studi:** Teknik Informatika — UMRAH  
> **Tahun Akademik:** 2025/2026
