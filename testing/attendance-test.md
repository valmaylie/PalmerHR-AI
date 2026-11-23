# Pengujian Attendance Agent

## Tujuan
Merekap data kehadiran dan menandai catatan yang perlu diverifikasi.

## Prompt
```text
Baca dan ikuti skill attendance-recap.
Analisis examples/data_karyawan_fiktif.csv.
Rekap kehadiran per karyawan dan unit, identifikasi data kosong,
duplikat, format tidak valid, dan anomali jam.
Jangan mengubah file sumber.
```

## Hasil contoh yang dilaporkan
- Total catatan: 5.
- Total karyawan: 3.
- Hadir: 4.
- Izin: 1.
- EMP003 pada unit Kantor ditandai karena jam masuk dan pulang kosong; perlu konfirmasi apakah kondisi tersebut sesuai status izin.
- Tidak ditemukan duplikat pada data contoh.
- Keterlambatan/lembur tidak dihitung karena jadwal dan toleransi tidak disediakan.

## Kriteria evaluasi
- [x] Pengelompokan per unit.
- [x] Rekap jumlah hadir dan izin.
- [x] Penandaan data kosong.
- [x] Tidak mengarang jadwal/toleransi.
- [x] Tidak mengubah file sumber (sesuai keluaran yang dilaporkan).
