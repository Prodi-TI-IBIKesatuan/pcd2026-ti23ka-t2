# Penyelarasan Warna dan Perbaikan Citra Malam Hari

Proyek kelompok **Pengolahan Citra Digital 2026** · kelas `ti23ka` · topik **T2**

[![Cek proyek](https://github.com/Prodi-TI-IBIKesatuan/pcd2026-ti23ka-t2/actions/workflows/cek-proyek.yml/badge.svg)](https://github.com/Prodi-TI-IBIKesatuan/pcd2026-ti23ka-t2/actions/workflows/cek-proyek.yml)

**Lingkup kelompok kami:** Perbaikan citra malam hari dan pencahayaan rendah pada area jalan raya, perumahan, fasilitas umum, dan lingkungan sekitar kampus.

Memperbaiki pencahayaan dan keseimbangan warna foto yang diambil dalam kondisi gelap. Anggota dan perannya ada di [ANGGOTA.yml](ANGGOTA.yml); cara kerja kelompok ada di [PANDUAN.md](PANDUAN.md).

## Notebook

| Notebook | Tahap | Isi | Buka |
| --- | --- | --- | --- |
| `01_dataset_preprocessing.ipynb` | 1 | Statistik dataset, cek anotasi, preprocessing, gambar sebelum–sesudah | [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/Prodi-TI-IBIKesatuan/pcd2026-ti23ka-t2/blob/main/notebooks/01_dataset_preprocessing.ipynb) |
| `02_metode_klasik.ipynb` | 2 | 3 metode klasik dan metriknya | [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/Prodi-TI-IBIKesatuan/pcd2026-ti23ka-t2/blob/main/notebooks/02_metode_klasik.ipynb) |
| `03_metode_modern.ipynb` | 2 | Inferensi model pralatih dan metriknya | [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/Prodi-TI-IBIKesatuan/pcd2026-ti23ka-t2/blob/main/notebooks/03_metode_modern.ipynb) |
| `04_evaluasi.ipynb` | 2 | Tabel perbandingan, uji ablasi, kasus gagal | [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/Prodi-TI-IBIKesatuan/pcd2026-ti23ka-t2/blob/main/notebooks/04_evaluasi.ipynb) |

## Dataset (Tahap 1)

- Jumlah citra: 250 pasang citra gelap–terang (total 250 citra)
- Foto sendiri: 75 citra malam (Lutfi 15, Dani 15, Guntur 15, Adi 15, Egi 15)
- Sumber data tambahan dan lisensinya: LOL Dataset (Low-Light Dataset, lisensi riset akademis non-komersial)
- Langkah preprocessing: Penyeragaman resolusi citra menjadi 512×512 piksel dengan interpolasi INTER_AREA, konversi ruang warna BGR ke LAB, serta pemisahan kanal luminans (L) dan krominans (A, B) tanpa modifikasi.

Rincian dataset, format anotasi, dan tautan Drive: [data/README.md](data/README.md). Contoh sebelum–sesudah ada di [outputs/figures/](outputs/figures/).

## Hasil (Tahap 2)

| Metode | Jenis | PSNR | SSIM |
| --- | --- | --- | --- |
| [isi: nama metode klasik 1] | klasik | [isi] | [isi] |
| [isi: nama metode klasik 2] | klasik | [isi] | [isi] |
| [isi: nama metode klasik 3] | klasik | [isi] | [isi] |
| [isi: nama model] | modern | [isi] | [isi] |

- **Uji ablasi:** [isi: parameter atau langkah yang diubah, dan pengaruhnya pada metrik]
- **Kasus gagal:** [isi: minimal 3 contoh dan penyebabnya, gambar di outputs/figures/]
- **Kesimpulan:** [isi: metode mana yang terbaik untuk lingkup kami dan mengapa]

## Demo

Aplikasi: [isi: tautan https://huggingface.co/spaces/...]

Unggah foto gelap, tampilkan hasil perbaikan berdampingan dengan aslinya. Kode aplikasi ada di [app/](app/).

## Sumber dan atribusi

Tuliskan setiap kode, model, dataset, atau bantuan AI yang dipakai beserta sumbernya. Pemakaian tanpa sumber dihitung plagiarisme.

| Yang dipakai | Sumber | Dipakai untuk |
| --- | --- | --- |
| LOL Dataset | Wei et al. (2018), BMVC / Hugging Face | Dataset benchmark low-light enhancement|
| Claude | Anthropic | Bantuan asistensi analisis dataset, preprocessing, dan validasi kode|
