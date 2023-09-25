# V-for-Exccel-Wilayah

Rumus yang diberikan digunakan untuk mengisi kolom G secara otomatis dengan nama file yang memuat teks yang sesuai di kolom F. Ini dapat berguna jika Anda ingin mencari teks tertentu di file-file teks yang ada dalam folder Document.

Rumus tersebut akan mencari teks yang sama dengan nilai di kolom F di setiap file teks dalam folder Document. Jika teks ditemukan dalam salah satu file, maka nama file tersebut akan ditampilkan di kolom G. Jika tidak ada file yang memuat teks yang sesuai, kolom G akan tetap kosong.

# Folder Document

Folder ini berisi beberapa file teks dengan konten yang berbeda.

## Daftar File

- [Rantepao.txt](./Rantepao.txt): File teks dengan konten:

Rantepao
Karassik
Pasele


- [Tallunglipu.txt](./Tallunglipu.txt): File teks dengan konten:

Darra'
Tallunglipu
Tagari


- [Sa'dan.txt](./Sa'dan.txt): File teks dengan konten:

Balusu
Pangli
Palawa'


## Mengisi Kolom G Otomatis

Untuk mengisi kolom G secara otomatis dengan nama file yang memuat teks yang sesuai di kolom F, Anda dapat menggunakan rumus di bawah ini:

=IF(ISNUMBER(SEARCH(F1, INDIRECT("'Folder Document/""&F1&"".txt'!A1"))), F1, "")

Rumus ini akan mencari teks yang sama dengan nilai di kolom F di setiap file teks dalam folder Document. Jika teks ditemukan dalam salah satu file, maka nama file tersebut akan ditampilkan di kolom G. Jika tidak ada file yang memuat teks yang sesuai, kolom G akan tetap kosong.

Pastikan untuk mengganti 'Folder Document' dengan lokasi folder yang sesuai di komputer Anda sebelum menggunakan rumus ini.

Harap dicatat bahwa rumus ini hanya akan mencari file di folder Document dan hanya akan menampilkan nama file yang memuat teks yang sesuai. Jika ada lebih dari satu file yang memuat teks yang sama, hanya nama file pertama yang akan ditampilkan di kolom G.

Anda dapat menyalin teks di atas dan menyimpannya sebagai file Readme.md di dalam folder Document Anda. Pastikan untuk mengganti tautan file txt dengan tautan yang sesuai jika diperlukan.

Terima kasih atas pengingatannya, dan maaf atas ketidaktepatan sebelumnya.

Silakan gunakan teks di atas dan simpan sebagai file Readme.md di dalam folder Document Anda. Pastikan untuk mengganti tautan file txt dengan tautan yang sesuai jika diperlukan.
