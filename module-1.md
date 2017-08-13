## Perkenalan GIT dan GITHUB

Sebelum memulai pastikan anda sudah menginstall semua applikasi ini

1. Git  https://git-scm.com/
2. Nodejs https://nodejs.org/en/download/ (versi 6.11.2)
3. MongoDB https://www.digitalocean.com/community/tutorials/how-to-install-mongodb-on-ubuntu-16-04
4. MySQL https://www.digitalocean.com/community/tutorials/how-to-install-mysql-on-ubuntu-16-04


### Bacaan sebelum memulai
- https://try.github.io/ (try git - playground)
- http://rogerdudler.github.io/git-guide/ (GUIDE - Simple GIT)


### Intro

minggu pertama ini kita akan mengenal soal git & nodejs

- git adalah distribute version control yang bisa dikenal sebagai pengcontrol code kita di pada code base dan
- nodejs adalah javascript runtime yang di buat di atas Chrome V8 engine.  

## Tugas Minggu Pertama

minggu ini tugas awal kita adalah membuat sebuah package nodejs menggunakan npm dengan menggunakan data diri kita sebagai detail dari pacakge tersebut.

buka terminal kalian dan jalankan perintah di bawah

1. Buat Akun pada github.com karena kita akan menggunakan github sebagai sarana pembelajaraan kita nanti

- Cloning repo ini dengan perintah `git clone https://github.com/evo3cx/learn-basic.git`

- maka folder learn-basic akan terdownload di komputer kalian, masuk ke dalam folder dengan perintah `cd learn-basic`

- buat branch atas nama kalian dengan perintah `git checkhout -b {nama-kalian}`. ini akan menjalankan git untuk membuat branch baru dengan nama kalian. kita menggunakan branch sebagai version control code kalian.

  e.g:``` git checkout -b reza ```

- check jika branch sudah terbuat dengan benar `git branch`, ini akan memunculkan list dari branch
  baca lebih lengkap soal branch [disini](https://git-scm.com/book/en/v1/Git-Branching-What-a-Branch-Is).

- buat folder dengan nama kalian di dalam learn-basic `mkdir {nama-kalian}`

  e.g: ``` mkdir reza ```

- pindah ke folder dengan nama kalian dengan perintah `cd {nama-kalian}`

  e.g: ``` cd reza ```

- membuat npm package, jalankan perintah `npm init` lalu isikan form yang di minta oleh npm, setelah selesai ketik yes untuk memastikan bahwa data yang ada isi telah benar


- setelah kalian selesai berhasil membuat package baru sekarang waktunya untuk menambahkan code kalian ke repository ini.

- jalankan perintah beriku secara berurutan

    `git add .`

    `git commit -m "module-1 minggu pertama"`

    `git push origin {nama-kalian}`

  penjelasaan:
  - `git add .`

    ini akan menambahkan data yang baru kalian tambahakan ke dalam repo ini

  - `git commit -m "module-1 minggu pertama"`

    kalian memberikan pesan bahwa data yang data yang baru kalian tambahakn adalah ` "module-1 minggu pertama"`

  - `git push origin {nama-kalian}`

    `git push` adalah perintah untuk mengirimkan perubahan yang kalian buat ke server github.com, `{nama-kalian}` adalah branch yang tadi kita buat di awal.



lalu refresh halaman ini, ini adalah lagkah pertama kalian untuk dalam menggunakan git dan github


### Diskusi

jika kalian mengalami masalah dalam mengerjakaan tugas atau ada beberapa catatan saya yang keliru silahkan, tambahakan [issue](https://github.com/evo3cx/learn-basic/issues) dan masukan masalah kalian.
