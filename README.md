# belajar-github
1. Pentingnya Penggunaan Command Line (CLI)
Meskipun banyak aplikasi GUI (seperti GitHub Desktop atau GitKraken), Command Line tetap menjadi standar industri karena beberapa alasan:

    -Kecepatan dan Efisiensi: Setelah hafal perintahnya, mengetik jauh lebih cepat daripada menavigasi menu klik-kanan.

    -Akses ke Fitur Lengkap: Beberapa perintah Git tingkat lanjut (seperti bisect atau reflog) seringkali tidak tersedia secara penuh di aplikasi GUI.

    -Otomatisasi (Scripting): CLI memungkinkan Anda membuat skrip untuk mengotomatiskan tugas-tugas repetitif.

    -Universal: CLI bekerja sama di hampir semua sistem operasi (Windows, macOS, Linux) dan lingkungan server (SSH).

2. Langkah-Langkah Push Repository
Push digunakan untuk mengirim perubahan dari repositori lokal Anda ke repositori jarak jauh (remote) seperti GitHub atau GitLab.

Fungsi: Memperbarui kode di server agar bisa diakses oleh anggota tim lain atau sebagai cadangan.

    -git add .
    Menambahkan semua perubahan file ke area persiapan (staging area).

    -git commit -m "Pesan commit kamu"
    Merekam perubahan ke dalam riwayat repositori dengan pesan penjelasan.

    -git push origin <nama_branch>
    Mengirim commit tersebut ke server remote (biasanya branch main atau master).

<img src="/asset/Screenshot 2026-04-27 122040.png">

3. Langkah-Langkah Clone Repository
Clone digunakan untuk menyalin repositori yang sudah ada di server ke komputer lokal Anda untuk pertama kalinya.

Fungsi: Mengunduh seluruh proyek beserta riwayat versinya agar Anda bisa mulai mengerjakannya secara lokal.

    1.Buka terminal dan arahkan ke folder tempat Anda ingin menyimpan proyek.

    2.Dapatkan URL repositori (contoh: https://github.com/user/proyek.git).

    3.Jalankan perintah:
    git clone <URL_repositori>

    4.Masuk ke folder proyek:
    cd <nama_folder_proyek>

<img src="/asset/Screenshot 2026-04-27 121708.png">
<img src="/asset/Screenshot 2026-04-27 121914.png">

4. Langkah-Langkah Pull dan Push Repository
Dalam lingkungan tim, Anda tidak bisa langsung melakukan push jika ada perubahan baru di server yang belum ada di komputer Anda. Anda harus melakukan sinkronisasi terlebih dahulu.

Fungsi: Memastikan kode lokal Anda selaras dengan kode terbaru dari tim sebelum menambahkan perubahan baru (menghindari conflict).

Alur Kerja (Workflow):
    1.git pull origin <nama_branch>
    Mengambil perubahan terbaru dari server dan langsung menggabungkannya (merge) ke kode lokal Anda.

    2.Lakukan Perubahan Kode
    Edit file, perbaiki bug, atau tambah fitur di editor Anda.

    3.git add . 
    Siapkan perubahan yang telah selesai.

    4.git commit -m "Update fitur X"
    Beri label pada perubahan tersebut.

    5.git push origin <nama_branch>
    Kirim kembali hasil kerja Anda ke server.

<img src="/asset/Screenshot 2026-04-27 121759.png">