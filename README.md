# Pertemuan 13 - Debugging dan Testing

Nama: Meyliana Solihah
NIM: 2225250080
Kelas: 3B
Program Studi: S1 Pendidikan Matematika

## Deskripsi
Praktik debugging, tracing, testing, dan perbaikan bug pada program Python.

## Cara Menjalankan
python praktik/praktik_4_debugging.py

## Test Case

| ID | Input | Expected | Actual Awal | Status |
|---|---|---|---|---|
| T1 | [80, 60, 90, 70] | 75.0 | 60.0 | FAIL |
| T2 | [100, 80] | 90.0 | 36.0 | FAIL |
| T3 | 60 | Lulus | Tidak lulus | FAIL |
| T4 | 59 | Tidak lulus | Tidak lulus | PASS |
| T5 | [80, 60, 90, 70] | 90 | 0 | FAIL |

## Bug Report

**B01 - Bug rata-rata**
- Penyebab: pembagi ditetapkan 5, bukan jumlah data.
- Perbaikan: gunakan jumlah elemen dalam list.

**B02 - Bug status kelulusan**
- Penyebab: operator `>` membuat nilai 60 tidak lulus.
- Perbaikan: gunakan operator `>=`.

**B03 - Bug nilai tertinggi**
- Penyebab: operator pembanding terbalik.
- Perbaikan: gunakan `>` agar nilai tertinggi diperbarui dengan benar.
