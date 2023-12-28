# domino-playing-robot

Implementasi Robot Arm (Dobot Magician) untuk Bermain Kartu Domino

*Tujuan dari proyek ini adalah untuk mengimplementasikan robot arm (dobot magician) untuk bermain kartu domino dengan lawan pemain manusia dengan menggunakan visi komputer untuk melakukan deteksi objek (Computer Vision).*

[DoBot Magician](https://www.dobot.cc/dobot-magician/product-overview.html) adalah sebuah robot lengan serbaguna yang dirancang untuk berbagai aplikasi. Robot ini dilengkapi dengan lengan robotik yang dapat bergerak dengan presisi tinggi dalam tiga sumbu. Selain itu, Dobot Magician juga memiliki kemampuan untuk mengganti end effector, seperti gripper (penggenggam) atau pen, sesuai dengan kebutuhan aplikasi. Fitur ini memungkinkan robot ini untuk melakukan berbagai tugas seperti pemindahan dan pengambilan objek, pemrograman robot, pencetakan 3D, dan pemrosesan otomatis dengan fleksibilitas yang tinggi.

[YOLOv8](https://docs.ultralytics.com/) adalah algoritma deteksi objek yang menggunakan jaringan saraf konvolusional (CNN) untuk memprediksi bounding box dan probabilitas kelas untuk setiap objek di dalam gambar. YOLO bekerja dengan membagi gambar menjadi grid berukuran SxS. Setiap sel grid bertanggung jawab untuk memprediksi objek yang ada di dalamnya, termasuk bounding box dan probabilitas kelas. Bounding box adalah kotak persegi panjang yang mendefinisikan lokasi dan ukuran objek. Probabilitas kelas adalah nilai yang menunjukkan kemungkinan suatu sel grid berisi objek dari kelas tertentu.

Dalam hal ini memfokuskan pengoperasian DoBot Magician melalui Python dengan  menggunakan [Dobot Lab](https://www.dobot-robots.com/products/education/magician.html). Menggunakan kode Python memberikan kebebasan yang lebih besar dalam mengontrol DoBot Magician, termasuk otomatisasi dan gerakan yang sangat terkalibrasi untuk tugas yang kompleks. 

## Daftar Isi
* [Memulai](#Memulai)
* [Panduan](#Panduan)
   * [Pengaturan Kamera](#Pengaturan-Kamera)
   * [Deteksi Objek dengan YOLOv8](#Deteksi-Objek-dengan-YOLOv8)
   * [Menghubungkan Robot](#Menghubungkan-Robot)
   * [Kalibrasi Robot dengan Kamera](#Kalibrasi-Robot-dengan-Kamera)
   * [Bermain](#Bermain)
* [Kode Akhir](#Kode-Akhir)


## Memulai

Untuk berkomunikasi dengan robot, kita memerlukan aplikasi [Dobot Lab](https://www.dobot-robots.com/products/education/magician.html). Selanjutnya pastikan kita juga menginstal 
[Python](https://www.python.org/) dan [OpenCV](https://opencv.org/) dalam lingkungan Python. Untuk IDE, kita dapat memanfaatkan menu Python Lab dalam aplikasi Dobot Lab.
![alt text](./assets/dobotlab-sc.png)







