# Mengirim Kode dari Git ke GitHub

## Persiapan
1. Pastikan Anda telah memiliki akun GitHub. Jika belum, buatlah akun baru di [github.com](https://github.com/).
2. Instal Git di komputer Anda jika belum terpasang.
3. Buka aplikasi Obsidian dan buat catatan baru untuk menyimpan materi ini.
## Langkah-langkah
1. *Buat Repositori GitHub Baru*: 
   - Login ke akun GitHub Anda.
   **- Klik tombol "New" untuk membuat repositori baru.**
 
     ![](asset/Pasted_image_20240730203037.png)
   **- Berikan nama repositori, pilih apakah akan bersifat publik atau privat, lalu klik "Create repository".**
        ![[Pasted_image_20240730203011.png]]
## pwd
`$ pwd` adalah perintah yang digunakan untuk "Print Working Directory" atau menampilkan direktori kerja saat ini.

Jika Anda menjalankan perintah `$ pwd` dalam terminal atau command prompt, hasilnya akan menunjukkan jalur lengkap dari direktori tempat Anda berada saat ini.

Contoh hasil dari perintah `$ pwd`:

![[asset/Pasted_image_20240731124529.PNG]]
## Git version:
   Perintah `git --version` digunakan untuk menampilkan versi Git yang terinstall pada komputer Anda.
    **Fungsi**: Perintah ini berguna untuk memeriksa versi Git yang Anda gunakan, yang dapat bermanfaat dalam mengidentifikasi dan mengatasi masalah kompatibilitas.

```cs
git --version
```

![[asset/Pasted_image_20240730205155.PNG]]
## Git init:
   - Buka terminal atau command prompt, lalu navigasi ke direktori tempat Anda menyimpan kode.
   - Jalankan perintah berikut untuk menginisialisasi Git:
     ```cs
     git init
```
![[asset/Pasted_image_20240730205613.png]]
Perintah ini digunakan untuk memulai menggunakan Git pada suatu proyek. Setelah menjalankan `git init`, direktori saat ini akan berubah menjadi repositori Git yang dapat digunakan untuk melacak perubahan pada proyek.


 
## git add.:
   - Jalankan perintah berikut untuk menambahkan file ke staging area:
    - `git add`: Perintah ini digunakan untuk menambahkan file atau perubahan ke dalam staging area.
    - `.`: Titik (dot) ini menandakan bahwa semua file di direktori saat ini dan subdirektorinya akan ditambahkan ke staging area.
```cs
       git add.
  ```

   - Perintah git add . akan menambahkan semua file baru dan perubahan ke staging area.
![[asset/Pasted_image_20240731073247.png]]

 
## GIT --LIST
git config --list 
Perintah `git config --list` digunakan untuk menampilkan semua konfigurasi Git yang telah diatur pada komputer atau repository tertentu.
FUNGSI:Perintah ini berguna untuk melihat semua pengaturan Git yang aktif, seperti username, email, remote repository, dan lainnya.

```cs
`git config --list`
```
![[asset/Pasted_image_20240730204624.png]]

## git config
 ## ***git config --global 
 - `git config`: Perintah ini digunakan untuk melihat, mengatur, dan mengelola pengaturan konfigurasi dalam Git.
- `--global`: Menandakan bahwa pengaturan ini berlaku secara global, bukan hanya untuk repositori tertentu.
- `user.name`: Menunjukkan bahwa pengaturan ini untuk nama pengguna.
- `"Indrawan666"`: Merupakan nilai yang akan ditetapkan sebagai nama pengguna global Anda dalam Git.
- - Untuk melihat pengaturan konfigurasi Git saat ini, Anda dapat menggunakan perintah `git config --list`.

```Cs
git config --global user.name "Indrawan666"
```
![[asset/Pasted_image_20240730211312.png]]

```cs
git config --global user.email "wawancaraa79@gmail.com"
```
 - `git config`: Perintah ini digunakan untuk melihat, mengatur, dan mengelola pengaturan konfigurasi dalam Git.
- `--global`: Menandakan bahwa pengaturan ini berlaku secara global, bukan hanya untuk repositori tertentu.
- `user.email`: Menunjukkan bahwa pengaturan ini untuk alamat email.
- `"wawancaraa79@gmail.com"`: Merupakan nilai yang akan ditetapkan sebagai alamat email global Anda dalam Git.
-  - Untuk melihat pengaturan konfigurasi Git saat ini, Anda dapat menggunakan perintah `git config --list`
![[Pasted image 20240730211433.png]]


## cd (direktori)

```cs
cd obsidian
```
1. - Buka terminal atau command prompt di komputer Anda.
    - Jalankan perintah "cd obsidian" untuk berpindah ke direktori "obsidian".
    - Setelah itu, Anda dapat menjalankan perintah-perintah lain di dalam direktori "obsidian".
    -![[asset/Pasted_image_20240730215258.png]]

## ls
- `   ls` - Menampilkan daftar file dan direktori di direktori saat ini.
- `ls direktori` - Menampilkan daftar file dan direktori di dalam direktori yang ditentukan.
```cs
ls
```
![[asset/Pasted_image_20240730215510.png]]

## remote add origin

remote add origin https://github.com/indrawan666/belajar-git.git
- `remote add`: Perintah ini digunakan untuk menambahkan koneksi remote ke repositori lokal.
- `origin`: Ini merupakan nama konvensi umum untuk menamai koneksi remote utama.
- `https://github.com/indrawan666/belajar-git.git`: Ini adalah URL dari repositori remote di GitHub yang ingin dihubungkan dengan repositori lokal.

 ```cs

     git remote add origin https://github.com/username/nama-repository.git
     ```


```cs
remote add origin https://github.com/indrawan666/belajar-git.git
```


## git Commit:
   - Jalankan perintah berikut untuk membuat commit dengan pesan yang jelas:
   - Perintah `git commit -m "Pesan commit"` digunakan untuk menyimpan perubahan yang telah dilakukan pada repositori Git dengan menambahkan pesan
     ```cs

     git commit -m "Pesan commit"
     ```
![[Pasted image 20240730205753.png]]
![[Pasted image 20240730221633.png]]

![[Pasted image 20240730221412.png]]




##  git push origin master
   Terakhir, jalankan perintah berikut untuk mengunggah kode Anda ke GitHub:
   ```cs
git push  origin master
```
-  push`: Berfungsi untuk mengunggah (push) perubahan dari repositori lokal ke repositori remote.
- `origin`: Nama remote repository yang telah ditambahkan sebelumnya menggunakan perintah `git remote add`.
- `master`: Nama cabang yang akan diunggah ke repositori remote.
![[asset/Pasted_image_20240730211106.png]]
 dan login sesuai akun git hub yang anda buat 
 ![[asset/Pasted_image_20240731130702.png]]

Itulah langkah-langkah dasar untuk mengirim kode dari Git ke GitHub menggunakan aplikasi Obsidian. 

## Akses Folder Proyek di Gitbash

 ### cd (direktori)

```cs
cd obsidian
```
1. - Buka terminal atau command prompt di komputer Anda.
    - Jalankan perintah "cd obsidian" untuk berpindah ke direktori "obsidian".
    - Setelah itu, Anda dapat menjalankan perintah-perintah lain di dalam direktori "obsidian".
    -![[asset/Pasted_image_20240730215258.png]]

### ls
- `   ls` - Menampilkan daftar file dan direktori di direktori saat ini.
- `ls direktori` - Menampilkan daftar file dan direktori di dalam direktori yang ditentukan.
```cs
ls
```
![[asset/Pasted_image_20240730215510.png]]

# Hubungkan Folder  Proyek Lokal
inisialisasi repository git init

hubungkan ke repository git remote 

 tampilkan status commit / koneksi file ke git hub  `git status`

tambahhkan file-file baru atau perubahan menggunkan git add .

tampilkan status commit /koneksi file ke github  `git status`








![](![[Screenshot 2024-07-31 130324.png]])








