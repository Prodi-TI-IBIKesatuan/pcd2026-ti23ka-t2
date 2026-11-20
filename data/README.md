# Data

Dataset lengkap **tidak** disimpan di repo ini. Repo hanya berisi `sample/` (≤ 20 gambar yang sudah disensor) untuk contoh dan demo.

## Ringkasan

- Tautan folder Google Drive (akses terbatas): https://drive.google.com/drive/folders/1ct6powog5_FvgYBF5gVWK0yHHsYhmgWw
- Jumlah citra: 250 pasang citra gelap–terang (total 250 citra)
- Foto sendiri per anggota: Lutfi 15, Dani 15, Guntur 15, Adi 15, Egi 15 (total 75 foto sendiri)
- Sumber data tambahan dan lisensinya: LOL Dataset (Low-Light Dataset, lisensi penelitian akademis non-komersial)
- Jumlah baris anotasi: 250 baris pada anotasi.csv
- Cara pengambilan foto (perangkat, waktu, lokasi umum): Kamera smartphone (Samsung, OPPO, & iPhone), diambil pada rentang waktu malam hari (pukul 19.00 - 23.00 WIB) di lokasi jalanan, perumahan, dan fasilitas umum

## Anotasi
Pasangan citra gelap–terang sebagai referensi (mis. dataset LOL) dan foto malam sendiri. Foto sendiri tanpa pasangan dinilai dengan metrik tanpa referensi (NIQE/BRISQUE, opsional lewat paket pyiqa).

Simpan sebagai anotasi.csv di folder Drive, satu baris per citra (atau per pasangan), dengan kolom persis seperti format_anotasi.csv. Baris contoh di berkas itu fiktif.

## Etika dan privasi

Wajah orang wajib diburamkan di data/sample. Jangan menulis NIM, nama orang lain, atau data pribadi lain di repo ini.
