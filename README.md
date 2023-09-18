# KELOMPOK-5
SISTER
Titik kunci yang mewakili tingkat konsistensi data:
1. Konsistensi Kuat (Strong Consistency): Pada titik ini, sistem terdistribusi menjamin bahwa setiap akses baca akan selalu melihat versi data yang sama, tidak peduli di mana akses tersebut dilakukan. Konsistensi kuat menghilangkan semua kemungkinan inkonsistensi data, tetapi seringkali mengorbankan kinerja dan skalabilitas.
2. Konsistensi Terbatas (Limited Consistency): Konsistensi terbatas mengizinkan beberapa bentuk keterlambatan atau inkonsistensi sementara dalam data antar node dalam sistem terdistribusi. Namun, batasan ini harus terdefinisi dengan jelas dan dapat diterima oleh aplikasi yang menggunakan data tersebut.
3. Konsistensi Eventual (Eventual Consistency): Ini adalah titik di mana sistem terdistribusi mengizinkan inkonsistensi data sementara antar node, tetapi pada akhirnya, semua node akan konvergen ke versi data yang sama. Konsistensi ini sering digunakan dalam sistem yang sangat terdistribusi untuk meningkatkan kinerja dan toleransi terhadap partisi jaringan.
4. Konsistensi Lemah (Weak Consistency): Pada titik ini, sistem terdistribusi hanya memberikan sedikit atau tanpa jaminan konsistensi antar node. Data dapat divergensi dan terlihat berbeda di beberapa node pada waktu yang sama. Konsistensi lemah sering digunakan dalam sistem yang sangat terdistribusi yang fokus pada kinerja maksimum.
