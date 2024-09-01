### **Patricia Leondrea Diajeng Putri**
### **122450050 / RB**

## **1. Pengantar**
Visualisasi Data merupakan suatu alat untuk mengubah data abstrak menjadi bentuk fisik. Visualisasi Data digunakan karena memiliki cara yang efektif untuk menyajikan data menarik kepada manusia. Saat ini, banyak perusahaan memiliki lebih banyak data sehingga semakin banyak pula perusahaan yang menggunakan data dan analitik lanjutan untuk menginformasi keputusan strategis dan operasional. Visualisasi Data ini sangat cocok untuk memberikan gambaran secara menyeluruh tentang Big Data dan memudahkan para ilmuwan data dalam meinginterpetasikan hasil analisis data.

Perkembangan Visualisasi Data sangat mengalami kemajuan pesat di berbagai bidang seperti pada komunitas grafik komputer yang menggunakan D3, komunitas visualisasi yang menggunakan tableu, ataupun komunitas basis data. Visualisasi data pun banyak digunakan dalam berbagai aplikasi yang berkaitan dengan basis data, seperti Excel, Google Sheets, dan lainnya.

### **Pipeline Visualisasi Data**
Pipeline Visualisasi Data umumnya bersifat iteratif yang terdiri dari beberapa langkah seperti import data, persiapan data, manipulasi data, mapping, serta rendering. Berdasarkan pipeline ini, terdapat tiga arah utama yang membuat Visualisasi Data lebih efisien dan efektif, yaitu
1. Spesifikasi Visualisasi : menyediakan berbagai cara bagi pengguna untuk menentukan apa yang mereka inginkan
2. Pendekatan Efisien untuk Visualisasi Data : memproses pembuatan visualisasi data harus efisien dan dapat diskalakan, terutama untuk komponen "Data Manipulation" dan "Mapping"
3. Rekomendasi Visualisasi data : memandu pengguna untuk memberikan rekomendasi visualisasi dari berbagai sudut pandang.

### **Survey Terkait**
Pada umumnya, survey tentang Visualisasi Data berfokus pada topik tertentuk, seperti visualisasi grafis, visualisasi data terkait, visualisasi ontologi, visualisasi data berdimensi tinggi, dan visualisasi data temporal. Survei ini mengkaji teknik visualisasi dari perspektif yang berbeda, yaitu
1. Spesifikasi Visualisasi : mengkaji klasifikasi, sumber data, media presentasi, dan bahasa visualisasi.
2. Pendekatan Efisien untuk Visualisasi Data : membahas integrasi basis data, visualisasi data, dan analisis data sehingga pengguna dapat bekerja dalam satu sistem, namun tanpa diskusi khusus tentang efisiensi.
3. Rekomendasi Visualisasi Data : membahas bagaimana berbagai sistem secara otomatis merekomendasikan visualisasi yang informatif untuk pengguna.

## **2. Spesifikasi Visualisasi Data**
### **2.1 Spesifikasi Visualisasi Data**
Secara umum, bahasa visualisasi data terdiri dari tiga bagian, yaitu:
1. Data : meliputi catatan data yang perlu divisualisasikan dan transformasi seperti pengelompokan, pengelompokan bin, penyaringan, dan pengurutan.
2. Tanda (Isyarat Visual) : termasuk jenis (misalnya, batang, garis, titik), ukuran (lebar, tinggi visualisasi), legenda, dan properti lain seperti lebar dan warna batang.
3. Pemetaan : menghubungkan data dengan tanda yang sesuai.

### **2.2 Kategorisasi Bahasa Visualisasi Data**
Bahasa visualisasi data dapat dikategorikan berdasarkan tingkat ekspresivitasnya, yaitu :
1. Bahasa Tingkat Rendah (lebih ekspresif namun lebih kompleks) : mengharuskan untuk menentukan semua elemen pemetaan, misalnya Prefuse
2. Bahasa Tingkat Tinggi (lebih mudah digunakan karena menyediakan default yang masuk akal dan lebih banyak batasan) : mencakup rincian konstruksi visualisasi, seperti fungsi pemetaan dan properti tanda, misalnya ggplot2.

### **2.3 Operasi Visual Berbasis GUI**
Alat berbasis GUI seperti Google Sheets, mengikuti prinsip "manipulasi langsung" untuk spesifikasi visualisasi, menyediakan antarmuka yang ramah pengguna untuk eksplorasi data. Meskipun demikian, alat ini memiliki keterbatasan dalam fleksibilitas untuk mengubah detail visualisasi.

### **2.4 Spesifikasi yang Kurang Ditentukan**
Spesifikasi visualisasi yang kurang ditentukan memungkinkan sistem visualisasi untuk menafsirkan input yang tidak lengkap berdasarkan petunjuk tertentu dari pengguna, seperti:
1. Berbasis Referensi : memberikan rekomendasi visualisasi berdasarkan visualisasi referensi yang diberikan pengguna.
2. Berbasis Kata Kunci : menerima masukan kata kunci dari pengguna dan merekomendasikan visualisasi yang relevan.
3. Berbasis Bahasa Alami: menggunakan konteks masukan pengguna dan status sistem untuk menyediakan antarmuka analisis visual yang lebih intuitif.

## **3. Pendekatan Efisien untuk Visualisasi Data**
### **3.1 Visualisasi Data yang Tepat**
Pendekatan ini bertujuan menghasilkan visualisasi yang tepat secepat mungkin. Sistem visualisasi data sering membaca data dari basis data dan menggunakan alat visualisasi untuk menghasilkan visualisasi. Pendekatan umum adalah menerjemahkan kueri visualisasi ke kueri SQL yang didukung oleh sistem manajemen basis data (DBMS). Namun, pendekatan ini memiliki kelemahan karena fungsionalitas yang berulang dan sulit untuk dioptimalkan. Alternatif yang lebih baik adalah mengintegrasikan pengambilan data dan rendering untuk mempercepat proses visualisasi. Contoh sistem yang mendukung ini adalah Ermac dan DeVIL, yang menyediakan bahasa seperti SQL untuk merepresentasikan visualisasi baik statis maupun interaktif.

### **3.2 Visualisasi Data Perkiraan**
Ketika ukuran data sangat besar dan kueri kompleks, visualisasi data yang tepat mungkin tidak selalu bisa dilakukan. Dalam kasus ini, visualisasi data perkiraan yang lebih cepat tetapi kurang akurat bisa menjadi solusi. Beberapa sistem menggunakan pendekatan Query Pemrosesan Perkiraan (AQP) untuk menghasilkan visualisasi dalam waktu interaktif dengan menggunakan subset data yang representatif. Pendekatan ini memungkinkan pengguna untuk mendapatkan visualisasi awal yang perkiraannya cukup mendekati hasil sebenarnya.

### **3.3 Visualisasi Data Progresif**
Pendekatan ini secara bertahap menyempurnakan hasil visualisasi antara, memungkinkan pengguna untuk melihat perkembangan data secara bertahap. Misalnya, sistem seperti Kyrix menyediakan antarmuka spesifikasi visualisasi deklaratif di sisi depan dan pemrosesan visualisasi yang dapat diskalakan secara efektif di sisi belakang. Teknik ini memungkinkan pengguna untuk memperbesar dan memperkecil data untuk melihat lebih banyak detail atau gambaran umum.

### **Teknologi Pendukung**
Pendekatan-pendekatan ini didukung oleh berbagai teknologi seperti penyimpanan kolom, indeks, komputasi paralel, dan prediksi atau prefetching data. Penyimpanan kolom, misalnya, menawarkan kinerja yang lebih baik untuk aplikasi OLAP dengan hanya menyimpan kolom data yang relevan. Penggunaan indeks dapat mempercepat waktu eksekusi kueri dengan mengurangi jumlah catatan yang perlu diperiksa. Komputasi paralel memungkinkan eksekusi beberapa kueri secara bersamaan, mempercepat proses visualisasi.

## **4. Rekomendasi Visualisasi**
### **4.1 Rekomendasi Berdasarkan Spesifikasi**
1. Spesifikasi yang Tidak Lengkap : memerlukan spesifikasi kosong tidak memerlukan masukan pengguna, sedangkan yang memerlukan spesifikasi parsial menerima input dari pengguna mengenai elemen visualisasi yang diinginkan, misalnya Voyager.
2. Spesifikasi sebagai Referensi : memberikan rekomendasi visualisasi berdasarkan data atau visualisasi referensi yang ada, misalnya SeeDB 

### **4.2 Rekomendasi Berdasarkan Perilaku**
Menangkap perilaku pengguna untuk mengidentifikasi tugas yang dimaksud dan memberikan rekomendasi visualisasi yang berguna berdasarkan tugas tersebut, misalnya HARVEST mengamati tindakan pengguna seperti inspeksi dan penyaringan untuk menentukan pola tugas dan merekomendasikan visualisasi sesuai.

### **4.3 Rekomendasi Personal**
1. Model Linier : memberikan rekomendasi visualisasi yang dipersonalisasi, misalnya VizDeck
2. Filtering Kolaboratif : menggunakan data dari pengguna lain untuk memberikan rekomendasi berdasarkan kesamaan preferensi, misalnya VizRec 

### **4.4 Ringkasan**
1. Spesifikasi Kosong : untuk eksplorasi cepat data saat pengguna tidak familiar dengan visualisasi, misalnya Data2Vis.
2. Spesifikasi Parsial : memungkinkan pengguna memberikan spesifikasi sebagian untuk visualisasi yang diinginkan, misalnya DeepEye.
3. Berdasarkan Referensi : mudah dikembangkan dan cocok untuk pengguna yang jelas tentang kebutuhan mereka, misalnya Zenvisage.
4. Berdasarkan Perilaku : memberikan rekomendasi berdasarkan pola perilaku pengguna, tetapi terbatas pada pola yang telah didefinisikan.
5. Personalized : menyediakan rekomendasi khusus untuk setiap pengguna berdasarkan data historis mereka, dengan hasil yang bervariasi untuk setiap individu.

## **5. Arahan Penelitian Lain**
### **5.1 Persiapan Data untuk Visualisasi Data**
Data dunia nyata sering memerlukan persiapan yang signifikan sebelum dapat divisualisasikan secara efektif. Proses ini mencakup pembersihan data untuk mengatasi masalah seperti duplikasi, normalisasi, nilai yang hilang, dan pencilan. Dampak data kotor pada visualisasi dapat menyebabkan interpretasi yang bias.

Penelitian yang ada adalah analisis "What-if" untuk pencilan yang memungkinkan pengguna mengidentifikasi dan menghapus pencilan dari kueri agregasi dengan menemukan dan memodifikasi predikat yang menyebabkannya, menggunakan teknik analisis sensitivitas, serta Evaluasi Visualisasi dengan Data yang Hilang guna mengeksplorasi bagaimana metode imputasi yang berbeda dan teknik visualisasi mempengaruhi kualitas data yang dipersepsikan dan akurasi. Peluang penelitiannya adalah Deteksi Visualisasi Bias dan Pembersihan Data Berdasarkan Tugas.

### **5.2 Benchmarking Visualisasi Data**
Benchmarking dalam visualisasi data penting untuk evaluasi kinerja dan sistem rekomendasi. Benchmark yang efektif harus sesuai dengan tugas analisis visual, menyediakan jejak dan data yang dapat digunakan kembali, dan mempertahankan cakupan dan kualitas label yang tinggi.

Penelitian yang ada adalah VizNet yang merupakan kumpulan data berskala besar dari lebih dari 31 juta dataset dari repositori terbuka dan galeri visualisasi, menyediakan dasar untuk membandingkan teknik desain dan mengembangkan model benchmarking. Peluang penelitiannya adalah Kategorisasi Visualisasi yang menetapkan kategori konseptual untuk visualisasi (misalnya, tren vs. distribusi) merupakan tantangan dan memerlukan penelitian lebih lanjut serta Data Pelatihan untuk memberi label visualisasi untuk melatih model adalah kompleks, terutama ketika setiap visualisasi mungkin memiliki beberapa label.

### **5.3 Visualisasi Data untuk Aplikasi Terkait Basis Data**
Visualisasi data semakin integral untuk aplikasi terkait basis data, membantu dalam penemuan data, debugging, dan analisis keseluruhan.

Peluang penelitiannya adalah Visualisasi Data untuk Penemuan Data sehingga dapat meningkatkan pemahaman dan penemuan dataset relevan dari lake data besar, mengurangi kebutuhan untuk browsing yang ekstensif, serta Visualisasi Data untuk Debugging Data untuk mengatasi masalah dalam alur kerja analitik data yang disebabkan oleh input atau parameter yang salah dapat mendapat manfaat dari teknik visualisasi yang lebih baik, meskipun solusi saat ini masih dalam pengembangan.

## **6. Kesimpulan**
Visualisasi data adalah bidang yang berkembang pesat dengan banyak hasil penelitian baru dan sistem inovatif yang dikembangkan baru-baru ini. Penelitian dan praktisi dari berbagai bidang telah berkontribusi pada kesuksesan luar biasa visualisasi data, yang didorong oleh hampir semua domain dan aplikasi.

Artikel ini terutama mengulas karya-karya terbaru dalam visualisasi data dari perspektif manajemen data. Secara khusus, kami telah menggambarkan secara komprehensif mengenai spesifikasi visualisasi, metode efisien untuk visualisasi data, dan rekomendasi visualisasi. Sebagaimana telah disebutkan sebelumnya, sebagian besar sistem visualisasi data komersial unggul dalam hal kemudahan penggunaan dari segi spesifikasi visualisasi data. Namun, banyak praktisi masih mengalami masalah efisiensi dan rekomendasi dengan sistem-sistem ini. Oleh karena itu, kami juga membahas beberapa masalah terbuka yang dapat dipecahkan oleh peneliti basis data untuk memajukan bidang visualisasi data.

