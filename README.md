# KELOMPOK-5
SISTER

Titik kunci yang mewakili tingkat konsistensi data:
1. Konsistensi Kuat (Strong Consistency): Pada titik ini, sistem terdistribusi menjamin bahwa setiap akses baca akan selalu melihat versi data yang sama, tidak peduli di mana akses tersebut dilakukan. Konsistensi kuat menghilangkan semua kemungkinan inkonsistensi data, tetapi seringkali mengorbankan kinerja dan skalabilitas.
2. Konsistensi Terbatas (Limited Consistency): Konsistensi terbatas mengizinkan beberapa bentuk keterlambatan atau inkonsistensi sementara dalam data antar node dalam sistem terdistribusi. Namun, batasan ini harus terdefinisi dengan jelas dan dapat diterima oleh aplikasi yang menggunakan data tersebut.
3. Konsistensi Eventual (Eventual Consistency): Ini adalah titik di mana sistem terdistribusi mengizinkan inkonsistensi data sementara antar node, tetapi pada akhirnya, semua node akan konvergen ke versi data yang sama. Konsistensi ini sering digunakan dalam sistem yang sangat terdistribusi untuk meningkatkan kinerja dan toleransi terhadap partisi jaringan.
4. Konsistensi Lemah (Weak Consistency): Pada titik ini, sistem terdistribusi hanya memberikan sedikit atau tanpa jaminan konsistensi antar node. Data dapat divergensi dan terlihat berbeda di beberapa node pada waktu yang sama. Konsistensi lemah sering digunakan dalam sistem yang sangat terdistribusi yang fokus pada kinerja maksimum.


Konsistensi Data adalah hal yang mengacu pada tingkat keseragaman atau kekonsistenan data di seluruh komponen atau node yang terdapat dalam suatu sistem yang tersebar secara geografis atau logis. Dalam sistem terdistribusi, data dapat disimpan dan diakses dari berbagai lokasi yang berbeda, dan masalah konsistensi muncul ketika dua atau lebih operasi terjadi pada data yang sama dalam waktu yang bersamaan atau hampir bersama. Oleh karena itu, konsistensi data menjadi kritikal dalam memastikan bahwa informasi yang disimpan dan diambil dari sistem tersebut adalah akurat, dapat diandalkan, dan sesuai dengan harapan. Ada beberapa model konsistensi data yang digunakan dalam sistem terdistribusi:

  a. Strong Consistency (Konsistensi Kuat): Dalam model ini, setiap operasi baca akan mengembalikan hasil yang sama seperti hasil operasi tulis yang sebelumnya. Ini berarti       setiap pembaruan data akan terlihat seketika oleh semua entitas dalam sistem, dan tidak ada inkonsistensi antara baca dan tulis.
  b. Eventual Consistency (Konsistensi Akhir): Model konsistensi ini mengizinkan adanya keterlambatan dalam penyebaran pembaruan data ke seluruh sistem. Dengan kata lain,        jika tidak ada pembaruan data lebih lanjut, semua node akan akhirnya mencapai keadaan konsisten setelah suatu waktu. Ini sering digunakan dalam sistem yang harus             menjaga kinerja tinggi.
  c. Causal Consistency (Konsistensi Sebab-Akibat): Dalam model ini, operasi-operasi yang memiliki hubungan sebab-akibat harus diterapkan secara konsisten. Jika operasi A        mempengaruhi operasi B, maka operasi A harus terlihat sebelum operasi B di semua node.
  d. Session Consistency (Konsistensi Sesuai Sesi): Konsistensi ini berkaitan dengan konsistensi dalam konteks sesi pengguna. Selama sesi pengguna tertentu, pengguna akan        melihat operasi mereka sendiri dalam urutan yang konsisten, tetapi tidak perlu konsisten dengan operasi pengguna lain.
  e. Read Your Writes (Baca Tulisan Anda): Dalam model ini, pengguna akan selalu melihat hasil tulisan mereka sendiri saat mereka membaca data. Meskipun operasi-operasi          pengguna lain mungkin belum terlihat, operasi pengguna sendiri harus terlihat.

