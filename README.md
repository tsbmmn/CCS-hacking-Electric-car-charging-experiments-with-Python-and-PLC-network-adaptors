
# CCS hacking: Electric car charging experiments with Python and PLC network adaptors

**pyPLC** adalah proyek open-source berbasis Python yang dirancang untuk memudahkan interaksi dengan Programmable Logic Controllers (PLC). Proyek ini menawarkan solusi sederhana dan efisien untuk mengendalikan dan berkomunikasi dengan PLC melalui bahasa pemrograman Python.

## Fitur Utama
- **Dukungan Beragam Model PLC**: Kompatibel dengan berbagai jenis dan model PLC.
- **Mudah Diintegrasikan**: Dapat diintegrasikan ke dalam sistem lain yang berbasis Python.
- **Sederhana dan Mudah Digunakan**: Instalasi dan penggunaan yang mudah untuk keperluan automasi.
- **Baca dan Tulis Data PLC**: Menyediakan fungsi untuk membaca dan menulis data dari/ke PLC.

## Instalasi
1. Clone repository ini:
   ```bash
   git clone https://github.com/uhi22/pyPLC.git
   ```
2. Masuk ke direktori proyek:
   ```bash
   cd pyPLC
   ```
3. Install dependensi yang diperlukan:
   ```bash
   pip install -r requirements.txt
   ```

## Contoh Penggunaan
Setelah instalasi selesai, berikut adalah contoh penggunaan pyPLC untuk menghubungkan dan berkomunikasi dengan PLC:

```python
from pyPLC import PLC

# Inisialisasi koneksi ke PLC
plc = PLC(ip_address="192.168.1.10", port=502)

# Membaca data dari PLC
data = plc.read_data(register=100, length=10)
print(data)

# Menulis data ke PLC
plc.write_data(register=100, values=[1, 2, 3])
```

## Kontribusi
Kontribusi terhadap pengembangan proyek ini sangat diterima! Jika Anda ingin berkontribusi:
1. Fork repository ini.
2. Buat branch baru untuk fitur atau perbaikan bug.
3. Buat pull request dengan deskripsi yang jelas.

## Dokumentasi
https://github.com/uhi22/pyPLC


