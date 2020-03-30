LANGKAH-LANGKAH MENJALANKAN DOCKER PADA WINDOWS
1.	Unduh file instalasi Docker melalui halaman download Docker
2.	Instal Docker menggunakan executable file yang sudah diunduh.
3.	Setelah selesai proses instalasi, buka cmd lalu ketikan docker -v untuk mengecek apakah aplikasinya sudah ada atau belum.
4.	Untuk mempermudah proses konfigurasi pertama gunakan Docker Quick Start Terminal 
5.	Tunggu sampai proses selesai lalu akan muncul gambar atau lambang docker dan kita bisa menulis
6.	Untuk percobaan pertama, tuliskan docker run hello-world pada Quick Start Terminal dan akan berjalan.
7.	 Selanjutnya untuk membuat docker image kita harus membuat folder terlebih dahulu dengan mengetikkan perintah “mkdir docker”
8.	Selanjutmya masuk kedalam folder docker yang tadi kita buat ketikan perintah “cd docker”
9.	Kemudian jika belum memiliki aplikasi web ASP.NET Core maka bisa diunduh source code dengan perintah “git clone https://github.com/rezafaisal/HelloASPNETCore.git”
10.	Kemudian untuk pindah ke folder aplikasi ketikan perintah “cd HelloASPNETCore/HelloWorld.ASPNETCore/src/HelloWorld.ASNETCore/”

MEMBUAT DOCKERFILE
Dengan perintah “touch Dockerfile”. Kemudian tambahkan baris pada file Dockerfile
Keterangan dari baris diatas yaitu”
1.	FROM bertujuan menentukan lokasi image ASP.NET yang akan digunakan.
2.	COPY bertujuan untuk menentukan lokasi konten dari folder yang sedang aktif ke folder/app.
3.	WORKDIR bertujuan menentukan direktori yang akan digunakan.
4.	RUN bertujuan untuk perintah, pada baris diatas artinya dijalankan perintah dnu restore.
5.	EXPOSE bertujuan menentukan menentukan port yang akan digunakan oleh aplikasi.
6.	ENTRYPOINT bertujuan cara untuk menjalankan aplikasi, pada baris diatas aplikasi dijalankan dengan perintah dnx.

MENJALANKAN CONTAINER
Untuk menjalankan container yang telah dibuat dalam bentuk docker image gunakan perintah docker run -it nginx /bin/bash lalu enter kemudian docker ps.