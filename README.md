# latihan1
#   # PENGGUNAAN GIT 


### APA ITU GIT 
* Git adalah salah satu sistem pengontrol versi (Version ControlSystem) pada proyek perangkat lunak yang diciptakan oleh Linus Torvalds.
* Pengontrol versi bertugas mencatat setiap perubahan pada fileproyek yang dikerjakan oleh banyak orang maupun sendiri.
* Git dikenal juga dengan distributed revision control (VCS terdistribusi),artinya penyimpanan database Git tidak hanya berada dalam satutempat saja.


### INSTALASI GI
* Download *Git*, buka website resminya Git `(git-scm.com)`.
* Kemudian unduh Git sesuai dengan arsitektur komputer kita. Kalau menggunakan 64bit, unduh yang 64bit. Begitu juga kalau menggunakan 32bit.
* Selamat, Git sudah terinstal di Windows. Untuk mencobanya,silahkan buka *CMD* atau *PowerShell*, kemudian ketik perintah

``git --version``

![Screenshot 2020-10-18 141255](https://user-images.githubusercontent.com/72906441/96361435-d810cb80-114f-11eb-947a-060390174a7a.png)


### Menambahkan Global Config
* Pada saat pertama kali menggunakan git, perlu dilakukan konfigurasi ``user.name dan user.email``
* konfigurasi ini bisa dilakukan untuk global repostiry atau individual repository.

* apabila belum dilakukan konfigurasi, akan mengakibatkan terjadi kegagalan saat menjalankan perintah `git commit`

* Config Global Repository

`$ git config --global user.name “nama_user"`

`$ git config --global user.email “nama_user”`

![Screenshot 2020-10-18 141332](https://user-images.githubusercontent.com/72906441/96361567-05aa4480-1151-11eb-93a8-cad1f572bac9.png)

### Perintah Dasar Git

* `git init`, perintah untuk membuat repository local
* `git add`, perintah untuk menambahkan file baru, atau perubahan pada file pada staging sebelum proses commit.
* `git commit`, perintah untuk menyimpan perubahan kedalam database git.
* `git push -u origin master`, perintah untuk mengirim perubahan pada repository local menuju server repository.
* `git clone [url]`, perintah untuk membuat working directory yang diambil dari repositry sever.
* `git remote add origin [url]`, perintah untuk menambahkan remote server/reopsitory server pada local repositry ``(working directory)``
* `git pull`, perintah untuk mengambil/mendownload perubahan terbaru dari server repository ke local repository


### Membuat Reposiory Local

* Buka direktory aktif, misal: *d:\labs_pemrograman1* (buka menggunakan Windows Explorer)
* klik kanan pada direktory aktif tersebut, dan pilih menu *Git Bash*, sehingga muncul git bash commad
* Buat direktory project praktikum pertama dengan nama *latihan1*
``$ mkdir latihan1
$ cd latihan1``
* Sehingga terbentuk satu direktori baru dibawahnya, selanjutnya masuk kedalam direktori tersebut dengan perintah *cd* ``(change directory)``
* direktory aktif menjadi: **d:\labs_pemrograman1\latihan1


![Screenshot 2020-10-18 145520](https://user-images.githubusercontent.com/72906441/96361989-55d6d600-1154-11eb-97fa-c1ef65d1d057.png)

### Membuat Reposiory Local

* Jalankan perintah *git init*, untuk membuat repository local.
`$ git init`
* Repository baru berhasil di inisialisasi, dengan terbentuknya satu direktori hidden dengan nama .*git*
* Pada direktori tersebut, semua perubahan pada `working directory` akan disimpan.


![Screenshot 2020-10-18 145554](https://user-images.githubusercontent.com/72906441/96362066-e8777500-1154-11eb-9759-c5ea58aae306.png)

### Menambahkan File baru pada repository

* Untuk membuat file dapat menggunakan text editor, lalu menyimpan filenya pada direktori aktif (repository)
* disini kita akan coba buat satu file bernama README.md (text file)
`$ echo “# Latihan 1” >> README.md`
* File *README.md* berhasil dibuat.


![Screenshot 2020-10-18 145705](https://user-images.githubusercontent.com/72906441/96362129-56bc3780-1155-11eb-9fdb-5e4774f8f7be.png)


### Menambahkan File baru pada repository

* Untuk menambahkan file yang baru saja dibuat tersebut gunakan perintah git add.
`$ git add README.md`
* File *README.md* berhasil ditambahkan.


![Screenshot 2020-10-18 145747](https://user-images.githubusercontent.com/72906441/96362233-05f90e80-1156-11eb-99e1-f34d491360f0.png)


