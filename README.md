# 🏥 SQueue-Care: Data Science & Analytics Platform

Selamat datang di repositori **data_science** untuk proyek **SQueue-Care (Smart Queue & Healthcare Access Optimizer)**. Repositori ini didedikasikan khusus untuk menyimpan seluruh alur kerja data science, mulai dari analisis data eksploratif (EDA), pengujian hipotesis (A/B Testing), hingga pengembangan dasbor operasional analitik rumah sakit berbasis Streamlit.

---

## 📁 Struktur Direktori Folder

Seluruh berkas utama analitik dikelompokkan secara terstruktur di dalam folder ini:

```text
data/
├── Analisis_Data.ipynb           # Notebook Jupyter untuk proses EDA & Data Preprocessing
├── ab_testing.py                 # Skrip Python untuk kalkulasi dan validasi statistik A/B Testing
├── app.py                        # Kode utama Dasbor Analitik Operasional Rumah Sakit (Streamlit)
├── data_dictionary.md            # Kamus data penjelas seluruh fitur/kolom dalam dataset
├── dataset_RS.csv                # Dataset operasional rumah sakit mentah (raw data)
├── dataset_RS_clean.csv          # Dataset hasil pembersihan (clean data) siap pakai
├── hasil_ab_test.png             # Visualisasi output grafik hasil pengujian A/B Testing
├── Laporan_Teknis_SQueue_Care.pdf # Dokumen komprehensif metrik evaluasi & hasil analisis proyek
├── requirements.txt              # Daftar pustaka (library) Python pendukung platform
└── README.md                     # Dokumentasi utama repositori (File ini)

📈 Cakupan Analisis Proyek
Proyek data science pada platform SQueue-Care berfokus pada optimasi layanan kesehatan melalui tiga pilar analitik utama:

1. Exploratory Data Analysis (EDA) & Preprocessing
Melakukan investigasi kualitas data operasional rumah sakit, menangani missing values, serta melakukan konversi tipe data yang tepat.

Menganalisis distribusi waktu tunggu pasien (waiting time), pola penumpukan antrean berdasarkan poliklinik, serta efisiensi utilisasi alokasi dokter.

2. Validasi Statistik (A/B Testing)
Menguji efektivitas implementasi sistem antrean pintar SQueue-Care dalam mereduksi waktu tunggu pasien di rumah sakit secara signifikan.

Output visualisasi otomatis disimpan dalam file hasil_ab_test.png sebagai acuan metrik keberhasilan performa sistem bagi manajemen fasilitas kesehatan.

3. Interactive Web Dashboard (Streamlit Cloud)
Menyediakan platform analitik interaktif real-time berbasis web untuk membantu pihak manajemen rumah sakit memantau matriks operasional harian secara taktis.

🚀 Panduan Menjalankan Dasbor Secara Lokal
Jika Anda ingin menjalankan Dasbor Analitik SQueue-Care ini di lingkungan lokal komputer Anda, ikuti langkah-langkah berikut:

1. Prasyarat
Pastikan komputer Anda sudah terpasang Python 3.9+ dan lingkungan virtual terisolasi (.venv).

2. Instalasi Pustaka Dependensi
Masuk ke terminal, arahkan ke folder proyek, dan instal seluruh pustaka yang terdaftar di requirements.txt:

Bash
pip install -r data/requirements.txt

3. Jalankan Aplikasi Streamlit
Eksekusi perintah berikut dari direktori utama proyek untuk menyalakan server lokal Streamlit:

Bash
streamlit run data/app.py

Setelah berhasil dijalankan, browser Anda akan otomatis membuka alamat http://localhost:8501.
atau bisa juga ke link public : 

🛠️ Teknologi & Pustaka yang Digunakan
Bahasa Pemrograman: Python 3.11

Manipulasi & Analisis Data: Pandas, NumPy

Visualisasi Data Dinamis: Plotly, Matplotlib, Seaborn

Framework Dasbor Web: Streamlit Cloud

Analisis Statistik: SciPy (untuk komputasi t-test / A/B Testing)