# Bridging Global Infrastructure to Address Local Challenge with HPC
Studi kasus sesi **Bridging Global Infrastructure to Address Local Challenge with HPC** (Asst. Prof. Dr. Worawan Diaz C.) - *Informatics Practitioner Lecture Series, Informatika Unib*.

**Tema:** deteksi dan atribusi penyebab deforestasi di Provinsi Bengkulu. Data **sintetis** (untuk pembelajaran).

**Tujuan:** Menunjukkan bagaimana komputasi paralel/HPC mempercepat pemrosesan banyak tile citra satelit untuk masalah lokal (pemantauan hutan).

## Hasil singkat
Dijalankan pada **1 core** (sandbox), sehingga tidak ada speedup:

| Worker | Waktu (detik) | Speedup | Efisiensi |
|---|---|---|---|
| 1 | 3.55 | 1.0x | 1.0 |
| 2 | 3.857 | 0.92x | 0.46 |
| 4 | 4.25 | 0.84x | 0.21 |

**Jalankan ulang di mesin multi-core** untuk hasil yang bermakna.

## Struktur
```
src/parallel_benchmark.py   # benchmark paralel
src/config.py
reports/  docs/
```

## Menjalankan
```bash
pip install -r requirements.txt
python -m src.parallel_benchmark
```

## Laporan
Lihat [`docs/studi_kasus.md`](docs/studi_kasus.md).

## Repo lain dalam rangkaian studi kasus ini
- `01-data-analysis-and-ai`
- `03-gis-spatial-analysis`
- `04-machine-learning-intro`
- `05-hci-data-visualization`
- `06-deforestation-drivers-satellite-ai`
