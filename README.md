# Telco Customer Churn Prediction and Retention Analysis

## Latar Belakang dan Masalah Bisnis
Industri telekomunikasi menghadapi tantangan besar dalam mempertahankan pelanggan (customer retention). Berdasarkan riset, biaya untuk mengakuisisi pelanggan baru bisa 5 hingga 7 kali lebih mahal dibandingkan mempertahankan pelanggan lama. Proyek ini bertujuan untuk menganalisis data pelanggan dari sebuah perusahaan telekomunikasi fiktif (dataset IBM) untuk memahami secara mendalam apa yang membuat pelanggan berhenti berlangganan (churn) dan memprediksi siapa saja pelanggan yang berisiko churn di masa depan.

## Tujuan Proyek
- Mengidentifikasi profil dan perilaku pelanggan yang memiliki kecenderungan tinggi untuk churn.
- Menganalisis korelasi antara jenis layanan, durasi berlangganan (tenure), dan metode pembayaran terhadap tingkat churn.
- Membangun model Machine Learning (Logistic Regression & Random Forest) untuk memprediksi probabilitas churn pelanggan.
- Memberikan rekomendasi strategis yang actionable untuk menurunkan tingkat churn dan menyelamatkan potensi kerugian finansial.

## Alat dan Teknologi
- **Python (Pandas, Numpy):** Digunakan untuk manipulasi, pembersihan, dan agregasi data historis pelanggan.
- **Matplotlib & Seaborn:** Digunakan untuk Exploratory Data Analysis (EDA) dan membangun visualisasi data yang profesional.
- **Scikit-Learn:** Digunakan untuk preprocessing (encoding & scaling) serta melatih algoritma Machine Learning.
- **Jupyter Notebook:** Digunakan sebagai environment utama untuk menyajikan analisis secara interaktif (kode, narasi, dan visualisasi).

## Struktur Proyek
- `data/` : Folder berisi dataset mentah `WA_Fn-UseC_-Telco-Customer-Churn.csv` (7.043 baris × 21 kolom).
- `images/` : Kumpulan 11 visualisasi hasil EDA dan evaluasi model Machine Learning.
- `Telco_Customer_Churn_Analysis.ipynb` : Notebook utama (Jupyter) yang memuat keseluruhan analisis (End-to-End).
- `KLIK_UNTUK_BUKA_NOTEBOOK.bat` : Shortcut otomatis untuk pengguna Windows guna menjalankan notebook dengan satu klik.

## Temuan Utama (Key Insights)
1. **Titik Kritis Churn (Tenure):** Churn paling banyak terjadi pada **6 bulan pertama** berlangganan (mencapai >40%). Jika pelanggan berhasil melewati masa 2 tahun, persentase churn turun drastis di bawah 10%.
2. **Pengaruh Kontrak:** Pelanggan dengan kontrak bulanan (Month-to-month) sangat tidak loyal dengan tingkat churn hingga 42.7%. Pelanggan kontrak 2 tahun nyaris tidak ada yang churn (hanya 2.8%).
3. **Layanan Internet Fiber Optic:** Pelanggan yang menggunakan Fiber Optic memiliki churn rate tertinggi (41%). Hal ini mengindikasikan kemungkinan adanya masalah stabilitas jaringan atau harga yang dirasa terlalu mahal dibanding kualitasnya.
4. **Metode Pembayaran:** Pengguna `Electronic check` memiliki kecenderungan churn jauh lebih tinggi dibanding pengguna pembayaran otomatis (kartu kredit/transfer bank).
5. **Performa Model Machine Learning:** Model Logistic Regression dan Random Forest mampu memprediksi churn dengan nilai **ROC-AUC mencapai 0.84**, yang berarti model ini sangat handal dalam membedakan pelanggan yang akan churn dan yang tidak.

## Rekomendasi Bisnis
- **Program Loyalti 6 Bulan Pertama:** Tim Marketing wajib memberikan insentif khusus (seperti diskon atau akses premium gratis) pada 6 bulan pertama untuk mengamankan pelanggan baru dari risiko churn.
- **Transisi ke Kontrak Jangka Panjang:** Berikan promosi atau potongan harga bagi pelanggan Month-to-month yang bersedia beralih ke kontrak 1 atau 2 tahun.
- **Audit Layanan Fiber Optic:** Tim Infrastruktur dan Produk perlu segera menginvestigasi kualitas koneksi Fiber Optic karena layanan ini menjadi pendorong churn utama.
- **Insentif Auto-Pay:** Dorong pelanggan untuk beralih ke metode pembayaran otomatis (Kartu Kredit/Bank Transfer) dengan memberikan *cashback* bulanan berskala kecil, karena pengguna auto-pay terbukti jauh lebih loyal.

## Cara Penggunaan
Bagi Anda yang melihat repository ini di GitHub, Anda bisa langsung mengklik file **`Telco_Customer_Churn_Analysis.ipynb`** untuk membaca keseluruhan proses analisis beserta visualisasinya langsung di browser Anda.

Jika Anda ingin menjalankannya secara lokal di komputer (Windows):
1. Pastikan Anda telah menginstal Python dan Jupyter.
2. Clone repository ini.
3. Klik dua kali pada file `KLIK_UNTUK_BUKA_NOTEBOOK.bat`.
4. Browser akan otomatis terbuka menampilkan notebook interaktif.

---

<div align="center">

Dibuat dan dianalisis oleh **[Benaya Bagas Christianto](https://github.com/Benaya-Bagas-Christianto)**

*Berdedikasi untuk mentransformasi data kompleks menjadi insight bisnis yang strategis dan membangun solusi berbasis Machine Learning yang berdampak nyata.*

</div>
