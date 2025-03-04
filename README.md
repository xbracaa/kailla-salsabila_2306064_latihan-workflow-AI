Deskripsi Proyek
Jadi, saya sedang mengerjakan tugas praktikum kecerdasan buatan. Tugasnya adalah menganalisis data penjualan produk dan membuat model AI yang bisa memprediksi apakah stok barang masih cukup atau perlu ditambah (restock).

Membaca Data Penjualan
Saya punya data yang berisi tanggal transaksi, nama produk, jumlah terjual, stok tersisa, dan harga satuan.
Saya membaca data ini menggunakan pandas, supaya bisa ditampilkan dan dianalisis lebih mudah.

Mengolah Data
Saya cek apakah ada data yang kosong. Kalau ada yang kosong, nanti bisa diisi atau diabaikan.
Saya ubah format tanggal supaya lebih rapi.
Saya tambahkan dua kolom baru:
Total Penjualan → hasil dari Jumlah Terjual × Harga Satuan
Keuntungan → saya anggap harga modal setiap produk adalah Rp10.000, jadi keuntungan dihitung dari selisih harga jual dan modal.

Membuat Model AI
Saya pakai metode Decision Tree Classifier (pohon keputusan).
Model ini akan belajar dari data penjualan sebelumnya dan mencari pola.
Modelnya akan menebak apakah suatu barang perlu di-restock atau tidak. Jika stoknya kurang dari 5, maka dianggap harus di-restock.

Menguji Model
Saya coba masukkan contoh produk baru, misalnya jumlah terjual = 8 dan stok tersisa = 3.
Model akan memberikan jawaban:
  1 → produk harus di-restock.
  0 → stok masih cukup.

Menampilkan Grafik
Saya buat scatter plot untuk melihat hubungan antara jumlah terjual, stok, dan keuntungan.
Grafik ini membantu melihat pola mana produk yang cepat habis dan berapa keuntungannya.

Instruksi Cara Menjalankan Kode
Persiapan
Pastikan Python sudah terinstall.
Install pustaka yang diperlukan dengan menjalankan perintah berikut di terminal atau command prompt:
  pip install pandas scikit-learn matplotlib

Menjalankan File Notebook
Jika menggunakan Google Colab, buka Google Colab dan unggah data penjualan.

Eksekusi Kode
Tulis dan jalankan kode secara berurutan dari atas ke bawah:
  1. Baca Data – Menampilkan isi data penjualan.
  2. Proses Data – Membersihkan dan menyiapkan data untuk analisis.
  3. Latih Model AI – Melatih model Decision Tree untuk prediksi restock.
  4. Uji Model – Memprediksi apakah stok produk cukup atau perlu restock.
  5. Visualisasi Data – Menampilkan grafik hubungan stok, jumlah terjual, dan keuntungan.
  Selesai

Setelah semua kode dijalankan, model AI akan memberikan prediksi, dan hasil analisis data dapat dilihat dalam bentuk tabel serta grafik.
