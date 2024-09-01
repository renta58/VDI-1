MEMBUAT SEBUAH VISUALISASI DATA LEBIH EFISIEN DAN EFEKTIF: SEBUAH SURVEI
1.      VISUALISASI DATA
Visualisasi data,yang mengubah data abstrak menjadi bentuk fisik (misalnya panjang,posisi,bentuk,warna dan lainnya) merupakan cara yang dapat digunakan untuk menyajikan data  yang menarik bagi manusia  agar lebih berorientasi secara visual. Visualisasi data sangat baik untuk memberikan gambaran umum yang baik tentang data yang besar sehingga memudahkan interpretasi hasil analitik bagi seorang ilmuwan data.
Alur visualisasi data;
Import data-->data preparation-->data manipulation-->mapping-->rendering
1.      Data impor,menyimpan,mengambil data yang diperlukan dari sumber data yang diinginkan
2.      Data preparation, untuk menyiapkan data yang diimpor untuk divisualisasi,misalnya dengan menormalkan nilai,mengoreksi entri yang salah,dan menginterpolasi nilai yang hilang
3.      Data manipulation,yaitu memilih data yang akan disosialisasikan(alias memfilter dari komunitas visualisasi) dan mungkin dengan operasi umum lainnya seperti menggabungkan atau mengelompokkan.
4.      Mapping,adalah memetakan data yang diperoleh dari proses diatas ke primitif geometris(misalnya,titik dan garis),bersama dengan atributnya(misalnya warna,posisi,dan ukuran)
5.      Rendering,adalah mengubah data geometris di atas menjadi representasi visual
Berdasarkan alur kerja, maka terdapat tiga tahap yang membuat visualisasi data lebih efisien dan efektif:
1.)    Visualization Specifications,spesifikasi visualisasi menyediakan berbagai cara bagi pengguna untuk menentukan yang mereka inginkan karena 2 alasan berikut:
Self completenes,penting bagi pembaca untuk mengetahui bagaimana pembuatan visualisasi data.
Language design perspective: mengacu pada proses pemetaan informasi yang berbeda ke elemen visual dan manipulasi data untuk pemilihan bahasa basis data dan bahasa visualisasi
 
2.)    Efficient Approaches for Data Visualization
Agar dapat melibatkan pengguna secara efektif dalam alur kerja iteratif,proses pembuatan visualisasi data harus efisien dan dapat  diskalakan khususnya dengan dua komponen yaitu manipulasi data dan pemetaan
3.)    Rekomendasi visualisasi data
Sistem visualisasi dapat memandu pengguna dengan cerdas  dengan menggunakan rekomendasi agar memberikan spesifikasi yang ambigu dan sistem  akan secara otomatis menyelesaikan visualisasi dan memberikan rekomendasi. Untuk pendekatan yang efisien,maka akan mempertimbangkan cara mengintegrasikan basis data,visualisasi data dan analisis data untuk fokus membangun visualisasi data secara efisien.
 
2.      SPESIFIKASI VISUALISASI DATA
1.Spesifikasi visualisasi data
Secara umum visualisasi data terdiri dari tiga bahan: data,tanda atau isyarat visual), dan pemetaan
-        Data: data perlu divisualisasikan seperti filter,sortie dan digunakan untuk merekam data yang ditentukan.
-        Tanda
Jenis:representasi visual untuk catatan data seperti batang,garis atau titik
Ukuran :lebar,tinggi visualisasi
Legenda: informasi legenda
Properti lainnya seperti lebar dan warna batang
-        Pemetaan: memetakan data ke tanda yang sesuai
2.Kategorisasi bahasa visualisasi data
Kategori bahasa visualisasi data didasarkan pada ekspresi vitasnya, yaitu semakin rendah level suatu data bahasa,maka semakin ekspresif bahasa tersebut. Dimensi lain untuk memahami berbagai level bahasa spesifikasi visualisasi adalah melalui aksebilitasnya(atau mudah digunakan): semakin tinggi level suatu bahasa,semakin mudah digunakan . spesifikasi visualisasi data diklasifikasikan menjadi empat jenis/; bahasa tingkat rendah,bahasa tingkat tinggi,alat berbasis GUI, dan bahasa yang kurang spesifikasi. Semakin tinggi tingkat spesifikasi visualisasi data,semakin mudah digunakan dan semakin kurang ekspresif.
3.  	Operasi visualisasi berbasis GUI
Dibanding dengan menggunakan bahasa visualisasi seperti yang telah dibahas sebelumnya,cara yang lebih mudah untuk memberikan spesifikasi adalah  dengan mengikuti “prinsip manipulasi langsung”. Daftar alat berbasis GUI  seperti Excel,Google sheets,Microsoft dan lain-lain.
 
Visualisasi data interaktif,visualisasi data yaitu proses eksplorasi  untuk menambah/menghapus/mengubah atribut dan mengubah jenis bagan hingga mendapatkan visualisasi yang diinginkan dalam eksplorasi.
4.  	Spesifikasi yang kurang jelas
Visuaslisasi tidak akan berarti jika tidak dapat memberikan wawasan tentang data. Karena pengguna tidak benar-benar mengetahui semua aspek data yang ada sehingga diperlukan dukungan spesifikasi yang kurang spesifik  sehingga memberikan beberapa  petunjuk  dengan tipe berbasis referensi, jenis petunjuk berbasis kata kunci serta Jenis petunjuk ketiga adalah “berbasis bahasa alami” yang mempertimbangkan konteks masukan pengguna dan status sistem dalam siklus eksplorasi data, bukan petunjuk sekali jalan dalam petunjuk “berbasis kata kunci.
 
3.  	PENDEKATAN EFISIENSI UNTUK VISUALISASI DATA
 
Pendekatan ini akan membahas pendekatan yang efisien untuk visualisasi data; hal ini penting karena siklus hidup visualisasi data selalu berulang.
1.      Visualisasi data yang tepat.
Banyak sistem visualisasi data yang membaca data dari basis data. Sistem ini juga dapat memanipulasi data dengan pernyataan SQL dan kemudian menggunakan alat visualisasi untuk menampilkan visualisasi. Menginterpretasikan Sistem Visualisasi dengan DBMS. Meskipun menggunakan kueri adalah hal yang wajar,ada beberapa kekurangannya salah satu masalah utama adalah banyaknya fungsi yang diulang,sehingga menghasilkan teknik pengoptimalan  yang tidak terpadu dengan asumsi dan kinerja yang berada di server(yaitu sisi basis data) dan klien (yaitu sisi visualisasi) sehingga membuat pengembang bingung untuk memilih teknik pengoptimalan yang sesuai. Masalah utama lainnya adalah metode yang dipisahkan selit dipelihara,diperluas dan dioptimalkan untuk visualisasi interaktif,yang memerlukan penerbitan kueri terus-menerus untuk memodifikasi visualisasi. Secara intuitif, cara yang menjanjikan untuk memecahkan masalah di atas adalah dengan menggabungkan (atau mengintegrasikan) pengambilan data dan rendering secara erat untuk mempercepat proses pembuatan visualisasi. Sistem Manajemen Visualisasi Data (DBMS), adalah upaya penelitian dalam arah ini. Ini mendukung dua menyederhanakan-analisis-bahasa-alami-98655. hubungan: data dan skala,dimana hubungan data mencakup catatan data yang akan disosialisasikan dan direferensikan perbedaan pada elemen visual yang ditampilkan,skala hubungan menunjukkan pemetaan dari rentang data ke pengkodean visual rentang. Ada banyak teknik optimasi untuk visualisasi interaktif:
-        penyimpanan kolom,
-        Indeks Indeks banyak digunakan untuk meningkatkan kinerja pencarian dengan mengurangi jumlah rekaman/baris dalam tabel yang perlu diperiksa.
-        Komputasi Paralel Komputasi paralel juga telah banyak digunakan untuk pemrosesan kueri dalam sistem visualisasi data.
-        Prediksi dan Pra Pengambilan Salah satu langkah penting visualisasi data adalah eksplorasi data—pengguna terus menelusuri visualisasi yang mereka minati untuk mendapatkan gambaran tentang apa yang akan disosialisasikan
Teknologi pra pengambilan dan prediksi dikategorikan menjadi 2 jenis yaitu berdasarkan visualisasi data yang saat ini dieksplorasi atau data historis. Strategi  mengambil data berdasarkan data historis:arah,fokus dan vektor. Ada 2 tahap memprediksi data: Memprediksi fase analisis dan dilanjutkan dengan memprediksi petak data.
 
Studi Kasus menggunakan Kyrix dan Tableau
Kyrix adalah sistem visualisasi data interaktif yang dapat diskalakan. Kyrix menyediakan antarmuka spesifikasi visualisasi deklaratif di front-end dan pemrosesan visualisasi yang efektif dan dapat diskalakan di back-end, di mana pengguna memperbesar tampilan untuk melihat informasi terperinci dan memperkecil tampilan untuk melihat gambaran umum dalam visualisasi yang dapat diskalakan. TDE  adalah mesin data yang disesuaikan untuk visualisasi di Tableau 6.0. TDE mengoptimalkan mesin data terutama dalam perspektif berikut.
-        Penyimpanan dan Kompresi Berorientasi Kolom.
-        Penataan Ulang Operator
-        Pengurangan Kardinalitas
 
2.      Visualisasi data perkiraan
Berbasi AQP,yaitu cara termudah untuk menghasilkan visualisasi perkiraan dalam waktu interaktif adalah dengan memanfaatkan teknik AQP yaitu berfokus pada teknik pengambilan sampel. Sample+Seek [24] adalah sistem AQP untuk menjawab visualisasi yang dihasilkan dari query agregasi dalam kecepatan interaktif, dan hasil visualisasi berada dalam batas kesalahan yang ditentukan oleh pengguna. Pertama-tama ia menyajikan konsep presisi distribusi (misalnya, jarak antara visualisasi perkiraan dan eksak) yang dapat mewakili presisi distribusi total di seluruh kelompok agregat. Dengan demikian, pengguna dapat menentukan presisi distribusi sebagai batas kesalahan. Saat mengambil sampel, untuk kueri dengan volume data besar, ia menggunakan pengambilan sampel seragam untuk menjawab query agregasi COUNT dan mengusulkan teknik pengambilan sampel bias-ukuran untuk menjawab query agregasi SUM secara perkiraan dengan lebih sedikit predikat, dan fitur utama pengambilan sampel bias-ukuran adalah memilih baris dengan probabilitas yang proporsional dengan nilainya pada atribut agregasi. Sample+Seek mengusulkan dua teknik pengindeksan untuk mempercepat pengambilan sampel: indeks terbalik yang ditambah-ukuran untuk mengindeks dimensi kategoris untuk menjawab query agregasi; dan indeks grup frekuensi rendah untuk mendukung pertanyaan-pertanyaan dengan konjungsi satu atau lebih kendala yang sama.
 
3.      Visualisasi data progresif
-        Pengelompokan Berbasis Rentang
ImMense menyediakan visualisasi resolusi yang berbeda dengan mengubah ukuran bin. Bin dengan resolusi yang sama memiliki rentang yang sama. Data multidimensi dalam imMinens dipartisi ke dalam kubus data, dan kubus dipartisi ke dalam petak dengan level yang berbeda. Pengguna dapat menjelajahi data dalam level yang berbeda dan mengubah resolusi visualisasi yang sedang dijelajahi dengan memperbesar atau memperkecil tampilan, dan kemudian, sistem akan mengubah ukuran bin agregasi yang mendasarinya sesuai dengan itu. imMense mengelompokkan data numerik dengan rentang yang sama, yang memiliki beberapa keterbatasan. Misalnya, dengan mempertimbangkan kumpulan data transkrip ujian, pengelompokan dengan rentang skor yang sama tidak berlaku jika guru ingin mengetahui 10 teratas, 10 hingga 20 teratas, 20 hingga 30 siswa teratas, dst. Selain itu, pengguna tidak dapat mengubah ukuran bin atau jumlah resolusi yang berbeda dalam imMinens.
-        Pengelompokan Berbasis Rentang dan Konten
Terdapat   dua struktur pohon untuk eksplorasi hierarkis: HATree-R (HATree berbasis Rentang) dan HATree-CHATree berbasis Konten). HATree-R mirip dengan imMinens, dan simpul daun HATree-R menunjukkan titik data dalam rentang lebar yang sama, sementara HATree-C memiliki jumlah titik data yang sama di semua simpul daun. Dengan demikian, HATree-C dapat digunakan dalam skenario transkrip ujian di atas.
 
 
4.  	REKOMENDASI VISUALISASI
Solusi gambaran umum: Sistem  rekomendasi visualisasi perlu terlebih dahulu menghitung semua visualisasi yang mungkin, lalu merekomendasikan visualisasi dengan peringkat teratas. Perlu diperhatikan bahwa ruang pencarian semua visualisasi sangatlah besar, sehingga perlu mempertimbangkan kombinasi beberapa faktor, seperti pemilihan kolom yang akan disosialisasikan, transformasi data (misalnya, grup atau bin), pemilihan penyandian visual yang tepat termasuk jenis tanda (misalnya, batang, garis, titik), dan jenis penyandian untuk bagan tanda yang dipilih (misalnya, lebar batang, posisi titik).
Memangkas Visualisasi yang Tidak Berarti: Untungnya, ada banyak sinyal (atau kendala)—baik dari pengguna atau dari kearifan tradisional—yang dapat digunakan untuk memangkas visualisasi yang “buruk” yaitu batasan yang ditentukan pengguna dan batasan yang diberikan oleh pakar.
   1.Rekomendasi berbasis spesifikasi
a. Spesifikasi tidak lengkap
Sistem rekomendasi visualisasi dengan spesifikasi kosong tidak memerlukan input pengguna, sedangkan sistem rekomendasi dengan spesifikasi parsial menerima input spesifikasi elemen visualisasi parsial pengguna untuk visualisasi yang diinginkan.
Peringkat visualisasi berbasis aturan:> Sistem rekomendasi berbasis aturan memberi peringkat kandidat visualisasi berdasarkan aturan yang telah ditentukan sebelumnya, yang biasanya merupakan metrik efektivitas persepsi manusia, diukur sebagai skor efektivitas dengan mempertimbangkan tipe data, informasi statistik, preferensi visual manusia, dll. Misalnya, diagram lingkaran yang terdiri dari banyak blok (misalnya, > 500) bukanlah visualisasi yang baik menurut persepsi manusia, karena terlalu berantakan.
 Pemeringkatan visualisasi berbasis pembelajaran mesin:> sistem  rekomendasi berbasis web pertama-tama mengumpulkan data pelatihan yang berasal dari crowdsourcing atau web, kemudian melatih model pemeringkatan yang mengambil ruang input X sebagai daftar fitur vektor, dan Y ruang keluaran yang terdiri dari nilai (atau peringkat). Model mempelajari fungsi F(·) dari pelatihan contohnya, seperti yang diberikan dua vektor input x1 dan x2, dapat tentukan mana yang lebih baik, F(x1) atau F(x2).
 b.  	spesifikasi berdasarkan referensi
Beberapa sistem rekomendasi visualisasi merekomendasikan visualisasi berdasarkan data referensi atau visualisasi referensi. SeeDB berbasis deviasi [22] merekomendasikan visualisasi dengan penyimpangan dengan beberapa visualisasi referensi. Sebelum merekomendasikan perbaikan, pengguna harus menentukan pertanyaan yang diminati Q untuk mendapatkan data target yang disebut DQ dan juga diperlukan dataset referensi DR. Berbasis Anomali yang paling dapat membedakan anomali dalam visualisasi primer diklasifikasikan dengan beberapa metode deteksi anomali: titik normal dan titik abnormal berada dalam kelas yang berbeda, dilambangkan sebagai kolom kelas.
2.Rekomendasi Berbasis perilaku
Sistem rekomendasi berbasis perilaku menangkap perilaku pengguna saat ini sebagai masukan, kemudian menyimpulkan tugas yang diinginkan pengguna dan merekomendasikan visualisasi yang berguna berdasarkan tugas mereka. HARVEST adalah sistem rekomendasi visualisasi berbasis perilaku. HARVEST mendefinisikan 4 pola: memindai, membalik, menukar, dan drill-down. Kemudian, HARVEST dapat merekomendasikan visualisasi berdasarkan pola pengguna yang disimpulkan.
3.Rekomendasi yang dipersonalisasi
Sistem rekomendasi yang dipersonalisasi menangkap perilaku historis pengguna sebagai masukan untuk merekomendasikan visualisasi menarik yang dipersonalisasi. Teknik personalisasi berupa model linear dan penyaringan kolaboratif.
  	4.Ringkasan
Sistem rekomendasi visualisasi dengan spesifikasi kosong, seperti Draco  Data2Vis dan Rank-by-feature membantu pengguna untuk menjelajahi data dengan cepat  ketika pengguna tidak begitu familiar dengan data dan keinginan visualisasi. Sebagian besar sistem rekomendasi yang ada memerlukan spesifikasi parsial,karena mereka mengizinkan spesifikasi  pengguna  untuk visualisasi  yang diinginkan sebagai input,misalnya,kata kunci  spesifik di DeepEye. Solusi berbasis aturan ada si sesuai dengan pemahaman intuitif  seseorang terhadap visualisasi,tetapi tidak memberikan pemahaman yang lengkap  terhadap persepsi manusia,hanya berfokus pada beberapa metrik yang menarik. Mesin solusi berbasisi pembelajaran perlu mengumpulkan data pelatihan dan hasilnya memang sulit untuk diinterpretasikan,namun dapat menangkap gambaran manusia dengan baik pengetahuan kognitif  tentang efektivitas visualisasi. Dan model pembelajaran akan lebih pintar ketika banyak pelatihan data dikumpulkan.
Pengguna harus menentukan data referensi atau pola yang diinginkan dalam rekomendasi visualisasi berbasis referensi, yang mungkin sulit bagi pengguna yang tidak familiar dengan data asli dan ingin menjelajahi data dengan bantuan sistem rekomendasi. Keuntungannya adalah mudah untuk mengembangkan sistem seperti itu, dan nyaman ketika pengguna jelas tentang kebutuhan mereka, misalnya, temukan diagram garis dengan tren yang diinginkan.
Rekomendasi berbasis perilaku dapat merekomendasikan visualisasi alizations berdasarkan tugas yang disimpulkan, tetapi terbatas pada pola perilaku yang telah ditentukan sebelumnya, sehingga tidak fleksibel bagi pengguna perilaku acak.
Rekomendasi yang dipersonalisasi bekerja secara berbeda untuk pengguna yang berbeda, karena rekomendasi yang dipersonalisasi disesuaikan untuk pengguna yang berbeda berdasarkan perilaku historis mereka.



  5.     ARAH PENELITIAN LAINNYA
1.persiapan data untuk visualisasi
Persiapan data sangat diperlukan karena  data yang divisualisasikan harus dibersihkan, seperti normalisasi nilai, deduplikasi, imputasi nilai yang hilang, dan deteksi outlier.
2.Tolok ukur visualisasi data
Tolok ukur harus sesuai dengan tugas analisis visual, menyediakan jejak dan data yang dapat digunakan kembali, dan dalam hal rekomendasi, memiliki cakupan dan kualitas label yang tinggi.
3.Visualisasi data untuk aplikasi terkait  database
visualisasi data juga memainkan peran penting dalam aplikasi yang berhubungan dengan database, seperti Excel , Google Sheets , Oracle Data Visualization Desktop , IBM Db2 , Amazon Quicksight Microsoft Power BI , dan lainnya.
 
 
 
 
 
 

