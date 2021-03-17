# Komdat-P2_7
#Anggota Kelompok
1. Alfian Arief Santoso G64180061
2. M Faishal Mumtaz G64180093
3. Ramadhan Wiradikusuma G64180096
4. Ananda Alfarishi Anwar G64180097

<h1 align="center"><img src="https://user-images.githubusercontent.com/55485843/111281788-e7009900-866f-11eb-925a-c78eaa171cf9.png"></h1>

[Sekilas Tentang](#sekilas-tentang) | [Instalasi](#instalasi) | [Konfigurasi](#konfigurasi) | [Otomatisasi](#otomatisasi) | [Cara Pemakaian](#cara-pemakaian) | [Pembahasan](#pembahasan) | [Referensi](#referensi)
:---:|:---:|:---:|:---:|:---:|:---:|:---:



# Sekilas Tentang
[`^ kembali ke atas ^`](#)
# WAGTAIL

![Capture komdat](https://user-images.githubusercontent.com/54541186/111281876-a286e600-85fa-11eb-93b1-25c2e2725d41.PNG)


Wagtail adalah CMS yang dibangun dengan Python dan framework Django.

Content Management System merupakan sistem pembuatan website siap pakai.
mempermudah proses pembuatan website tanpa harus mengenal script pemrograman secara detil, sehingga pengguna pemula pun tidak akan menemui kesulitan ketika menggunakan CMS.

**Fitur Wagtail**

Implementasi yang berkelas
StreamField memungkinkan editor untuk membuat urutan campuran tipe konten. Ini membuat serial ke satu kolom JSON dalam database dan menyediakan cara langsung untuk menghasilkan konten pada template, menggunakan representasi HTML.

Pengeditan sederhana
kita dapat membuat kontrol pengeditan untuk masing-masing blok sesederhana atau serumit yang diperlukan: blok peta Google dapat berupa bidang kode pos sederhana, atau alat pilih lokasi seret dan perbesar / perkecil.

Ekonomi konten
Setelah keluar dari pola pikir rich text area, Anda akan menemukan cara yang lebih baik untuk mengatur informasi.

# Instalasi
[`^ kembali ke atas ^`](#)

Requirement untuk installasi : 
* Python 3
* Pipenv
* Text editor (vscode)

1. Pertama kita cek versi python terlebih dahulu
   
   $ python3 --version
 
2. Jika belum terinstall python, Mulailah dengan memperbarui daftar paket dan menginstal prasyarat:

   $ sudo apt update
   
   $ sudo apt install software-properties-common
   
3. Selanjutnya, tambahkan PPA deadsnakes ke sources list Anda:

   $ sudo add-apt-repository ppa:deadsnakes/ppa
  
4. Setelah repositori diaktifkan, instal Python 3.7 dengan mengetik perintah :

   $ sudo apt install python3
   
5. Setelah itu Install pip

   $ sudo apt install python-pip
   
6. Setelah pip terinstal maka kita dapat install pipenv

   $ sudo pip install pipenv
   
**INSTALL WAGTAIL**

1. Gunakan pip untuk menginstall wagtail

   $ sudo pip install wagtail
   
2. Wagtail terdapat fitur start yang mirip dengan django-admin startproject. menjalankan wagtail di my site akan menghasilkan folder baru dengan tambahan khusus wagtail.
Karena folder mysite sudah dibuat oleh venv, jalankan wagtail start dengan argumen tambahan untuk menentukan direktori tujuan: 

   $ wagtail start mysite mysite
   
**INSTALL PROJECT DEPENDENCIES**
   
   $ cd mysite
   
   $ pip install -r requirements.txt
   

**Create Database**

Jika kita belum punya projek terbaru, maka kita bisa membuat baru dengan cara :

   $ python manage.py migrate
 
**Create an admin user**

   $ python manage.py createsuperuser
   

**Start the server**

$ python manage.py runserver

# Konfigurasi
Melakukan Port Fowarding dari Virtualbox machine ke luar VM, disini kami menggunakan Windows 10
Kami menggunakan VM Ubuntu 18.04 

Pertama yaitu kita harus install open ssh pada Ubuntu dengan cara:

   $ sudo apt-get install openssh-server
   
   $ sudo systemctl enable ssh
   
   $ sudo systemctl start ssh

Setelah itu lakukan setting pada Virtualbox, masuk ke 'Settings -> Network -> Advance -> Port Forwarding'.

Aturan port forwarding sebagai berikut.

![Screenshot (387)](https://user-images.githubusercontent.com/60084504/111414923-757a2680-8713-11eb-838e-9ca342f6cb02.png)

Setelah selesai instalasi ssh pada Ubuntu lalu sudah menjalankan ssh. Selanjutnya silahkan menuju ke CMD windows dan login ke ssh:

   $ ssh user@server-name  



# Cara Pemakaian
[`^ kembali ke atas ^`](#)

Seperti biasa hal yang dilakukan untuk menggunakan Wagtail adalah sign in
![Capture komdat 2](https://user-images.githubusercontent.com/54541186/111287766-c64d2a80-8600-11eb-8b9b-af83164035ee.PNG)

Setelah sign in maka akan masuk ke halaman utama Wagtail
![Capture komdat 3](https://user-images.githubusercontent.com/54541186/111287995-01e7f480-8601-11eb-8ab7-596cccee74c0.PNG)

Sehabis itu kalian bisa menambahkan konten yang kalian inginkan di page yang sudah kalian miliki
![Capture komdat 4](https://user-images.githubusercontent.com/54541186/111288081-17f5b500-8601-11eb-8ee8-b5e2453cd5e0.PNG)

# Pembahasan
Pada kali ini kita berhasil melakukan installasi wagtail melalui ubuntu, Wagtail sendiri adalah CMS yang dibuat oleh Django. Untuk pemakaian didalam server ubuntu tidak ada masalah,kita bisa melakukan log in dan menggunakan aplikasi sesuai dengan kegunaannya. Untuk Proses installasi kita menginstall Python3,PipenV dan Pip. Untuk Django sudah terdapat dalam wagtailnya sendiri jadi tidak perlu melakukan installasi kembali.Untuk mengakses aplikasi melewati windows kita mengalami beberapa kendala kita bisa menyambungkan ssh tapi saat di buka di windows tidak mau terkoneksi. Sekian laporan hasil tugas akhir Komunikasi Data dan Jaringan Komputer, kurang lebihnya mohon maaf terima kasih.

# Referensi
[`^ kembali ke atas ^`](#)

https://docs.wagtail.io/en/stable/getting_started/tutorial.html?_ga=2.190831918.409681746.1615739120-158193979.1615739120
