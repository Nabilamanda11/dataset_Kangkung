# Dataset Kangkung

Dataset ini berisi data hasil pengamatan pertumbuhan tanaman kangkung (*Ipomoea aquatica*) berdasarkan parameter lingkungan, seperti tingkat kesuburan tanah, kelembapan media, pH, intensitas cahaya, kelembapan udara, dan frekuensi pemupukan. Dataset telah melalui proses normalisasi menggunakan metode Min-Max Scaling dan digunakan untuk pengembangan model Deep Learning dalam memprediksi pertumbuhan tanaman.

## File
- dataset_kangkung.csv

## Kolom
- Tinggi Tanaman
- Fertility (µS/cm)
- Moisture (%)
- pH
- Sunlight (lux)
- Humidity (%)
- Frekuensi Pemupukan

## Format
CSV

## Pra-pemrosesan Data (Data Preprocessing)

Sebelum digunakan dalam penelitian, seluruh fitur numerik pada dataset telah melalui tahap **normalisasi menggunakan metode Min-Max Scaling**, sehingga setiap nilai berada pada rentang **0–1**. Proses normalisasi dilakukan untuk menyamakan skala antar fitur dan meningkatkan performa model deep learning selama proses pelatihan.

Normalisasi dilakukan menggunakan persamaan berikut:

\[
X_{norm}=\frac{X-X_{min}}{X_{max}-X_{min}}
\]

dengan:
- \(X\) = nilai asli (raw data)
- \(X_{min}\) = nilai minimum pada fitur
- \(X_{max}\) = nilai maksimum pada fitur
- \(X_{norm}\) = nilai hasil normalisasi

Sebagai contoh, nilai **pH = 0.3333** pada dataset merupakan hasil normalisasi dan **bukan** nilai pH aktual. Hal yang sama berlaku untuk variabel lainnya seperti kelembapan media, intensitas cahaya, kesuburan tanah, dan kelembapan udara.
