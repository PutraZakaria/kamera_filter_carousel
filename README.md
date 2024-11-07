# kamera_filter_carousel

## Nama: Putra Zakaria Muzaki
## Kelas: TI-3H/19
## NIM: 2241720220

### Hasil
![alt](lib/test.gif)

## Jelaskan maksud void async pada praktikum 1?
Kata kunci async memungkinkan suatu fungsi untuk menjalankan operasi asinkron tanpa memblokir jalannya aplikasi. Ini sangat berguna saat Anda perlu menunggu hasil operasi seperti pemanggilan API atau proses yang membutuhkan waktu. Future<void> main() async menunjukkan bahwa fungsi main() akan mengembalikan Future<void>, dan kita bisa menggunakan await di dalamnya untuk menunggu hasil operasi asinkron. Pada Praktikum 1, await digunakan pada availableCameras() untuk mendapatkan daftar kamera yang tersedia sebelum aplikasi berjalan. Dengan menunggu hasilnya, aplikasi dapat memastikan bahwa informasi kamera siap saat layar TakePictureScreen ditampilkan.
<br>

## Jelaskan fungsi dari anotasi @immutable dan @override ?
1. @immutable adalah anotasi yang digunakan pada kelas untuk menunjukkan bahwa objek kelas tersebut bersifat immutable atau tidak dapat diubah setelah dibuat. Ketika sebuah kelas diberi anotasi @immutable, semua properti kelas tersebut seharusnya tidak dapat diubah setelah objek dibuat. Contoh penggunaannya pada class PhotoFilterCarousel, dimana setiap instance dari kelas ini seharusnya tidak mengalami perubahan setelah diinisialisasi, sesuai dengan prinsip "immutable".
2. @override digunakan untuk menandai bahwa metode yang dideklarasikan akan menimpa atau mengimplementasi metode yang sama di kelas induknya. Pada contoh di atas, @override digunakan pada createState di class PhotoFilterCarousel, yang menimpa metode createState dari StatefulWidget. Anotasi ini membantu membuat kode lebih jelas dan mencegah kesalahan, misalnya, jika metode yang akan ditimpa tidak ada di kelas induk, Dart akan memberikan peringatan.
