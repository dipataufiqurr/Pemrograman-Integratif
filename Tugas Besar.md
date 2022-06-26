# - Pemograman Integratif -
**Difa Taufiqurrahman   1202199005**

---
# Step 1 Install Laravel
### Install PHP
•	Download php di website https://windows.php.net/download#php-8.1. Kemudian pilih file zip 29,24 MB

![1](https://user-images.githubusercontent.com/92538741/173117724-30155a21-605d-4ec6-94ca-9074eb9e5b1d.png)


• Ekstrak file php, kemudian copy di lokasi “ C:\Program Files “. Cari file bernama "php.ini-development", buat salinan dan ubah nama file salinan menjadi “php.ini”. buka menggunakan text editor, dan jadikan seperti pada gambar, kemudian simpan.

![2](https://user-images.githubusercontent.com/92538741/173117952-020d408c-fd5a-4dea-a422-52a099d83908.png)
![3](https://user-images.githubusercontent.com/92538741/173117955-a628dd06-6973-43e7-85e8-22be957e0f62.png)

•	Buka `Edit The System Environment Variables`, klik `Environment Variables`

![4](https://user-images.githubusercontent.com/92538741/173118140-f92b8daf-f3e3-4bac-8b03-6b1f87991531.png)


•	Pilih variabel path untuk menambahkan alamat dari file php tadi, kemudian pilih ok.

![5](https://user-images.githubusercontent.com/92538741/173118219-7abd8ecb-5a17-4099-a40e-5dddedec677f.png)
![6](https://user-images.githubusercontent.com/92538741/173118284-ec17b398-4459-4859-adda-99813627e5dc.png)

•	Buka terminal dan ketikkan `php –v`, maka akan muncul tampilan seperti digambar, yang artinya php berhasil terinstall.

![6 5](https://user-images.githubusercontent.com/92538741/173118370-3067e15e-03b3-43e1-ab3b-8c3a0e86b1c6.png)


### INSTALL COMPOSER

•	Downlaod Composer https://getcomposer.org/download/ 
• Install file composer. Jika sudah buka terminal dan ketik “composer”, maka akan muncul tampilan seperti digambar, yang mana composer sudah terinstall.

![7](https://user-images.githubusercontent.com/92538741/173118721-15acd647-675f-427a-9b6b-c58a511d22f8.png)

### INSTALL LARAVEL VIA COMPOSER 

•	Buat folder baru di komputer untuk menginstall laravel. Kemudian buka terminal lalu masuk ke folder yang telah di buat
•	Buat project untuk install laravel dengan command `composer create-project laravel/laravel nama_project`

![8](https://user-images.githubusercontent.com/92538741/173119250-69549479-24b7-4899-aebe-713fade80848.png)

•	Masuk  terlebih dahulu ke folder project yang sudah dibuat dengan command `cd nama_project/` Dan jalankan project dengan command `php artisan serve`

![9](https://user-images.githubusercontent.com/92538741/173119647-6e3116c4-1de3-4a16-8c8f-3912381d53e4.png)

•	Buka laravel di browser sesuai dengan server yang ada di gambar

![9 5](https://user-images.githubusercontent.com/92538741/173119675-8b60e84a-58f3-434f-978b-540a466cf736.png)

![10](https://user-images.githubusercontent.com/92538741/173119860-9fef7860-0483-47fc-a318-13ee89276065.png)

---
# Step 2 - Menambahkan RSS
---

• Edit DB_DATABASE di .env sesuai dengan nama database yang sudah dibuat

![image](https://user-images.githubusercontent.com/92538741/175817980-45c346fa-d293-474b-bc13-14f2ac54b51a.png)

![image](https://user-images.githubusercontent.com/92538741/175817973-0cd94ac8-2784-4cf0-a508-ad1a461825cc.png)


• Buat migrations dengan 2 table rss dan news dengan comand seperti dibawah

![image](https://user-images.githubusercontent.com/92538741/175818043-03e3c01c-5378-4943-b292-8b2b2495b666.png)

• Tambahkan kolom name dan url pada tabel rss, seperti pada gambar dibawah

![image](https://user-images.githubusercontent.com/92538741/175818468-513529c4-b50c-4ff9-b79a-4cf6bf41b98a.png)

• Tambahkan kolom title, img_url, description, source_url,  dan rss_id pada tabel news, seperti pada gambar dibawah

![image](https://user-images.githubusercontent.com/92538741/175818512-227a795c-aa8f-4298-8b29-80a0eec8b1a6.png)

• Untuk menjalankan migrasi yang dibuat jalankan perintah diterminal seperti dibawah, lalu cek database

![image](https://user-images.githubusercontent.com/92538741/175818599-77e00771-3982-4a43-a1f2-b352a8e0365c.png)

![image](https://user-images.githubusercontent.com/92538741/175818648-a02d8b9c-ab9a-4924-a211-68f7b87f1c60.png)


• Buat koneksi  model  ke database  dengan membuat seeder dan controller untuk tabel Rss dan News dengan perintah seperti gambar dibawah

![image](https://user-images.githubusercontent.com/92538741/175818706-aa0ecf68-4627-4f80-80cb-7fa076ce4611.png)

• Edit file Rss.php, RssSeeder.php serta DatabaseSeeder.php seperti pada gambar dibawah

![image](https://user-images.githubusercontent.com/92538741/175818760-ce10d5f3-5b72-4fc8-aaaf-42b7319d19fc.png)

![image](https://user-images.githubusercontent.com/92538741/175818751-5d9cebbc-b1e3-4e6d-928a-3575bff6bfc6.png)

![image](https://user-images.githubusercontent.com/92538741/175818744-34b16e1a-18b8-4641-8b40-b5fe1fc6e9aa.png)

• Kemudian cek koneksi dengan perintah, kemudian cek database

![image](https://user-images.githubusercontent.com/92538741/175818855-289b46e8-c6b4-4c6f-b02f-b0e3aa325bb8.png)

![image](https://user-images.githubusercontent.com/92538741/175818935-fc5dfee2-a60f-44b6-b183-c7f84c34c439.png)

• Jalankan comand seperti gambar dibawah

![image](https://user-images.githubusercontent.com/92538741/175818995-240a0a29-6184-44d1-a00b-d2c030197b61.png)

• Edit file News.php, web.php, NewsController.php, serta file migration News seperti pada gambar dibawah

![image](https://user-images.githubusercontent.com/92538741/175819003-c8f876df-39d7-4923-b7a2-3957e6eec6c6.png)

![image](https://user-images.githubusercontent.com/92538741/175819026-fcdccd8e-c8bb-4cd0-a32c-c9c77e8afa91.png)

![image](https://user-images.githubusercontent.com/92538741/175819260-7a4b53a5-b6a4-4c68-8321-16762e55c820.png)



• Cek local host http://127.0.0.1:8000/aggregate/1

![image](https://user-images.githubusercontent.com/92538741/175819284-f7d7eaef-9e0f-4e41-9754-c8e205b92a5b.png)

• Cek local host http://127.0.0.1:8000/aggregate/4

![image](https://user-images.githubusercontent.com/92538741/175819323-03437e2f-ea15-4b8e-a232-f3bd5f82fa80.png)

• Cek local host http://127.0.0.1:8000/aggregate/5

![image](https://user-images.githubusercontent.com/92538741/175819346-3c139d0f-7fe8-4480-9696-562b380b75e1.png)

• Database phpmyadmin

![image](https://user-images.githubusercontent.com/92538741/175819477-763466a7-8731-44e4-9122-bf9074ec39ed.png)

### Difa Taufiqurrahman | 1202199005 



