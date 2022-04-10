---
title: Membuat Blog Gratis Di Github  Bagi Pemula
description: Langkah mudah membuat blog jekyll bagi pemula dengan memanfaatkan
  hosting gratis di Github
image: memilih%20tema%20lagi.png
date: 2020-12-06T05:09:17.083Z
tags:
  - Github
  - Dasar
  - Tutorial
---

## Mari kita mulai membuat blog Jekyll.
Saya asumsikan anda sudah memiliki akun Github.

### Kenapa Memilih Github
1. Hosting di Github benar-benar gratis, cocok bagi kita yang memiliki budget paspasan hanya bermodalkan domain yang kita miliki. Bila anda tidak memiliki domain, anda masih bisa membuat blog dengan url bawaan dari github pages anda.
2. Blog yang dihosting diGithub Pages sangat cepat jika dibandingkan dengan CMS lainnya. Inilah alasan mengapa saya memindahkan semua blog saya ke Jekyll (platform blogging di Github).
3. Tidak ada database atau eksekusi back-end di halaman Github. Jadi kemungkinan situs web diretas adalah nol.
4. Memiliki sedikit kesabaran untuk memahami cara kerjanya. Banyak sekali (setidaknya dalam kasus saya), pertama kali saya kesulitan dan tutorial-tutorial yang ada semuanya dalam bahasa inggris sehingga menyulitkan bagi orang seperti saya yang bahasa inggrisnya pas-pasan.

### Langkah Pertama Mencari Theme/Tema Blog Jekyll
Sebuah tema penting untuk blog yang bagus. Jika tidak, Anda dapat menggunakan tema dasar Jekyll jika Anda ingin mendesain semuanya sendiri. Tetapi jika Anda mencari tata letak pra-desain maka Anda harus mencari Jekyll Themes. Anda akan menemukan banyak tema tetapi, yang saya sarankan untuk mengunjungi https://theme.administrasi.net dan pilih tema gratis.

![Memilih Tema]({{ "/img/memilih tema lagi.png"| absolute_url }})

Pilih Tema kemudian klik repositori

### Langkah Kedua Fork Repositori
Pertama pilih tema kemudian fork repositori tema yang anda pilih (anda sudah login di github).

![Copy Repositori]({{ "/img/fork.png"| absolute_url }})

Dengan melakukan fork terhadap repositori berarti anda menyalin seluruh repositori sebagai repositori baru di dalam akun Github Anda. Anda dapat mengganti nama repositori menjadi apa pun yang Anda suka di opsi Pengaturan

### Langkah Ketiga Periksa Branch Sumber Dipilih
Setelah menyalin repositori tema, buka pengaturan dan temukan bagian Github Pages. Di sini Anda harus memilih cabang mana yang ingin Anda gunakan sebagai sumber situs web.

![Memilih Branch]({{ "/img/memilih branch.png"| absolute_url }})

### Langkah Keempat Menambahkan Custom Domain
#### Cara Pertama
Sekarang, arahkan ke repositori dan periksa apakah ada file CNAME di dalamnya. CNAME digunakan untuk domain khusus.

Jika ada, hapus URL di dalamnya dan ubah dengan custom domain milik anda. 

Blog Anda seharusnya sudah aktif dan berjalan sekarang. Tetapi berikan waktu. Maksimal 10 menit. Jekyll membangun sebuah blog statis sementara itu.

#### Cara Kedua
Selain cara di atas anda juga bisa menambahkan custom domain yang anda miliki pada kolom seperti gambar di bawah ini. 

![Custom Domain]({{ "/img/custom domain demo.png"| absolute_url }})

Apabila kolom tersebut tidak ada silahkan anda klik pilih tema dan pilih tema apa saja, kemudian kembali ke halaman pengaturan dan isikan custom domain pada kolom tersebut. 

## Konfigurasi
Edit konfigurasi pada file <code>_config.yml</code> umumnya akan terlihat seperti ini:

```
title: Demo # Judul Blog Anda
author: Username Github Anda
email: email-anda@domain.com
description: Deskripsi Blog anda.
baseurl: /blog # isi sesuaikan dengan kebutuhan anda contohnya /blog
url: https://theme.administrasi.net # Url Blog Anda, e.g. http://example.com
twitter_username: administrasi.net # ganti username twitter anda
github_username:  administrasi.net # ganti dengan username github anda
instagram_username: administrasi.net # ganti dengan username instragram
social:
  name: Nama Anda
  links:
    - https://twitter.com/administrasi.net
    - https://www.facebook.com/administrasi.net
    - https://www.linkedin.com/in/administrasi.net
	- https://plus.google.com/+administrasi.net
 	- https://github.com/administrasi.net
   	- https://keybase.io/administrasi.net
disqus:
  shortname: administrasi.net # to enable comments replace with your_disqus_shortname
```

Setelah menyelesaikan langkah-langkah di atas silahkan cek hasilnya.


