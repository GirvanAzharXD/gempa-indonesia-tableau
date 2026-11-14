# Gempa Bumi di Indonesia, 2024–2026

Dashboard interaktif sebaran dan tren gempa bumi di Indonesia, magnitudo M4,5 ke atas, periode 1 Januari 2024 sampai 13 November 2026. Data dari USGS Earthquake Catalog, divisualisasikan dengan Tableau Public.

**Live dashboard:** https://public.tableau.com/app/profile/mochamad.girvan.azhar/viz/GempaBumidiIndonesia20242026/GempaBumidiIndonesia20242026

## Temuan

1. Dua lonjakan jumlah gempa terjadi setelah gempa besar: April 2026 (179 gempa, susulan Bitung M7,4) dan Agustus 2026 (266 gempa, susulan Ende M7,8).
2. Sebagian besar gempa dangkal (1.750 dari 2.280) dan bermagnitudo kecil (M4,5–4,9: 1.768).
3. Aktivitas gempa terkonsentrasi di jalur seismik: pantai barat Sumatra, selatan Jawa, Sulawesi, Maluku, dan Papua.
4. Gempa terbesar dalam periode ini adalah M7,8 Ende (14 Agustus 2026), diikuti M7,4 Bitung (1 April 2026).

## Data

- **Sumber:** USGS Earthquake Catalog (earthquake.usgs.gov), diunduh manual lewat halaman pencarian USGS.
- **Cakupan:** Indonesia, 1 Jan 2024–13 Nov 2026, magnitudo M4,5+, jendela geografis lintang -11 s/d 6 dan bujur 95 s/d 141.
- **Cleaning:** dari 3.058 baris mentah, filter place membuang baris Philippines, Timor Leste, Malaysia, dan Palau, menyisakan 2.280 gempa. Dibuat kategori magnitudo (M4,5–4,9; M5,0–5,9; M6,0–6,9; M7,0+) dan kategori kedalaman (Dangkal <70 km; Menengah 70–300 km; Dalam >=300 km), lalu agregasi bulanan (35 bulan).
- **File:**
  - `gempa_indonesia_bersih.csv` — 2.280 baris, data bersih per gempa.
  - `gempa_indonesia_bulanan.csv` — 35 baris, jumlah gempa per bulan.
- **Catatan:** November 2026 parsial (data sampai 13 Nov); 73 baris bernama laut perairan Indonesia (mis. Banda Sea) dipertahankan karena masih wilayah Indonesia.

## Tools

- Tableau Public — dashboard
- Python (pandas) — cleaning dan agregasi data

## Screenshot

<img width="1838" height="781" alt="Gempa Bumi di Indonesia, 2024–2026" src="https://github.com/user-attachments/assets/309079f8-7900-4c02-a8fe-905e2918d5ed" />


## Lisensi

MIT
