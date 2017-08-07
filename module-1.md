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

buka terminal kalian dan jalankan perintah di bawah

1. Buat Akun pada github.com karena kita akan menggunakan github sebagai sarana pembelajaraan kita nanti

- Cloning repo ini dengan perintah `git clone github.com/evo3cx/learn-basic`

- maka folder learn-basic akan terdownload di komputer kalian, masuk ke dalam folder dengan perintah `cd learn-basic`

- buat branch atas nama kalian dengan perintah `git checkhout -b {nama-kalian}`. ini akan menjalankan git untuk membuat branch baru dengan nama kalian. kita menggunakan branch sebagai version control code kalian.

- check jika branch sudah terbuat dengan benar `git branch`, ini akan memunculkan list dari branch
  baca lebih lengkap soal branch [disini](https://git-scm.com/book/en/v1/Git-Branching-What-a-Branch-Is).

- buat folder dengan nama kalian di dalam learn-basic `mkdir {nama-kalian}`

- pindah ke folder dengan nama kalian dengan perintah `cd {nama-kalian}`

- jika sudah lalu initial npm dengan perintah `npm install`

- lalu jalankan perintah ini di terminal `echo "##learn basic " >> first.md`

- lalu jalankan perintah ini
    `git add first.md &&
    git push -u {nama-kalian}`

-  lalu refresh halaman ini, ini adalah lagkah pertama kalian untuk dalam menggunakan git dan github


### Diskusi

jika kalian mengalami masalah dalam mengerjakaan tugas atau ada beberapa catatan saya yang keliru silahkan buat [issue](https://github.com/evo3cx/learn-basic/issues) dan masukan masalah kalian.
