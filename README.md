# Capstone-Project_Hacktiv8

# Proyek Analisis Menu Kafe: Menemukan Minuman Paling Diminati

Proyek ini dibuat untuk membantu calon pemilik kafe dalam mengambil keputusan strategis mengenai menu yang akan disajikan. Dengan menganalisis data penjualan dari kafe lain, kita dapat mengidentifikasi tren dan preferensi pelanggan untuk menentukan menu apa yang paling berpotensi untuk sukses.

Latar Belakang
Membuka sebuah kafe baru memerlukan perencanaan yang matang, terutama dalam menentukan menu. Menu yang tepat tidak hanya akan menarik pelanggan tetapi juga mengoptimalkan manajemen stok dan meningkatkan profitabilitas. Untuk mengurangi risiko dan keraguan, proyek ini menggunakan pendekatan berbasis data untuk mendapatkan inspirasi menu.

Tujuan Utama
Tujuan utama dari program ini adalah untuk mengidentifikasi jenis menu kopi yang paling diminati oleh pelanggan. Dengan mengetahui produk terlaris, calon pemilik kafe dapat memastikan stok untuk menu tersebut selalu tersedia, menjadikannya sebagai pilar utama dalam penawaran produk.

Tentang Dataset
Dataset ini merekam transaksi penjualan harian dari sebuah kedai kopi di Cape Town, Afrika Selatan selama bulan Maret 2024. Dataset ini dirancang untuk membantu mengeksplorasi kebiasaan pelanggan dan kinerja bisnis—sempurna untuk analisis deret waktu, visualisasi data, atau proyek analisis data yang ramah bagi pemula.

🧰 Deskripsi Kolom
- date: Tanggal transaksi (YYYY/MM/DD)
- datetime: Stempel waktu pasti dari transaksi
- cash_type: Metode pembayaran (kartu atau tunai)
- card: ID pelanggan yang dianonimkan (berbasis loyalitas kartu)
- money: Jumlah yang dibelanjakan per transaksi (dalam Rand Afrika Selatan)
- coffee_name: Jenis kopi yang dibeli

📊 Analisis yang Mungkin Dilakukan
- Tren transaksi dan penjualan berdasarkan hari dalam seminggu.
- Distribusi pendapatan berdasarkan jenis kopi.
- Preferensi metode pembayaran (kartu vs. tunai).
- Rata-rata transaksi dan penjualan harian.
- Waktu puncak dalam sehari (pagi, siang, malam).

Bagaimana Program Ini Bekerja?
Program ini dirancang dalam beberapa langkah sederhana untuk mencapai tujuannya:

1. Memuat Dataset: Program memulai dengan membaca dataset Coffe_sales.csv yang berisi riwayat transaksi penjualan dari sebuah kafe. Dataset ini mencakup informasi seperti nama produk kopi, waktu transaksi, dan metode pembayaran.

2. Analisis Data dengan Pandas: Menggunakan pustaka Pandas, program menganalisis data untuk mengidentifikasi produk mana yang paling sering terjual. Secara spesifik, program menghitung frekuensi kemunculan setiap coffee_name untuk menemukan 5 menu teratas.

3. Integrasi AI dengan IBM Granite: Hasil analisis dari Pandas (yaitu, daftar 5 menu terlaris) kemudian dijadikan input untuk model bahasa AI, IBM Granite. Model ini diakses melalui API Replicate.

4. Menghasilkan Laporan dan Wawasan: IBM Granite mengolah data tersebut dan menghasilkan dua jenis laporan:

- Laporan Bisnis dengan Rekomendasi: Sebuah laporan yang ditujukan untuk perencana bisnis, berisi ringkasan eksekutif, wawasan, dan rekomendasi strategis yang dapat ditindaklanjuti mengenai manajemen inventaris dan pemasok.

- Analisis Data Murni: Sebuah analisis ringkas dalam bentuk poin-poin yang menyoroti preferensi pelanggan berdasarkan data penjualan yang ada.

Hasil Analisis
Berdasarkan data yang diolah, program ini berhasil mengidentifikasi 5 menu kopi yang paling populer:

1. Americano with Milk
2. Latte
3. Americano
4. Cappuccino
5. Cortado

Wawasan yang dihasilkan oleh AI menunjukkan bahwa minuman berbasis espresso, terutama yang dicampur dengan susu, merupakan inti dari bisnis kafe yang dianalisis. Ini memberikan fondasi yang kuat bagi calon pemilik kafe untuk membangun menu awal mereka.

Teknologi yang Digunakan
- Python: Bahasa pemrograman utama.
- Pandas: Untuk manipulasi dan analisis data.
- LangChain: Kerangka kerja untuk mengintegrasikan model bahasa.
- Replicate: Platform untuk mengakses model AI.
- IBM Granite: Model bahasa yang digunakan untuk menghasilkan analisis dan laporan.
- Jupyter Notebook / Google Colab: Lingkungan pengembangan interaktif.

Dengan proyek ini, keraguan dalam menentukan menu dapat diatasi dengan wawasan yang didukung oleh data, untuk membantu dalam membangun bisnis kafe yang sukses.
