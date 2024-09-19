# TUGAS 5 PRAKTIKUM SISTEM OPERASI

**1. Lihat daftar secara lengkap pada direktori aktif, belokkan tampilan standard output ke file baru.**

Untuk melihat daftar direktori aktif, gunakan perintah $ ls, sedangkan untuk membelokkan tampilan standard output ke file baru, gunakan ">"

![Screenshot 2024-09-19 111917](https://github.com/user-attachments/assets/22e1a8f2-5eda-4bc8-92ba-43d30c6fc7f2)

**2. Lihat daftar secara lengkap pada direktori /etc/passwd, belokkan tampilan standard output ke file baru tanpa menghapus file baru sebelumnya.**

Untuk melihat daftar lengkap dari direktori /etc/passwd, gunakan perntah $ ls, sedangkan untuk membelokkan tampilan standard output ke file baru
tanpa menghapus file baru sebelumnya, gunakan ">>"

![Screenshot 2024-09-19 112158](https://github.com/user-attachments/assets/9024ddda-a082-4e6b-9dc6-e8dbdb28241d)

**3. Urutkan file baru dengan cara membelokkan standard input.**

Untuk mengurutkan file, gunakan perintah $ sort, sedangkan untuk membelokkan standard input, gunakan "<"

![Screenshot 2024-09-19 112421](https://github.com/user-attachments/assets/77d1b7aa-7c26-43f7-a2f2-57d15f9299cd)

**4. Urutkan file baru dengan cara membelokkan standard input dan standard output ke file baru.urut.**

Untuk mengurutkan file, gunakan perintah $ sort, sedangkan untuk membelokkan standard input, gunakan "<", sedangkan untuk membelokkan standard output ke file, gunakan ">".
Pembelokan standart input dan standart output dapat dikombinasikan asalkan tidak boleh menggunakan nama file yang sama sebagai standart input dan output.

![Screenshot 2024-09-19 112653](https://github.com/user-attachments/assets/4098190f-1bf7-48af-95d6-b75168d85d26)

**5. Buatlah direktori latihan6 sebanyak 2 kali dan belokkan standard error ke file rmdirerror.txt.**

Gunakan perintah $ mkdir untuk membuat direktori baru. Saat membuat direktori yang sama sebanyak dua kali, akan muncul pesan error. 
Pesan error itu kemudian dibelokkan ke file dengan menggunakan "2>".

![Screenshot 2024-09-19 113044](https://github.com/user-attachments/assets/a31be1be-003b-4cad-af78-1341f60b1f45)

**6. Urutkan kalimat berikut dengan menggunakan notasi here document :**

**sort <<@@@**

**Jakarta**

**Bandung**

**Surabaya**

**Padang**

**Palembang**

**Lampung**

**@@@**

Pertama, buat notasi here document yang akan dibelokkan ke sebuah file kemudian isi document tersebut. Setelah diisi dan diakhiri, isi dokumen akan tersimpan ke file yang dibelokkan. 
File tersebut kemudian diurutkan menggunakan perintah $ sort. 

![Screenshot 2024-09-19 113318](https://github.com/user-attachments/assets/d0ab27de-20db-4974-9f67-40b2e7e16776)

**7. Hitung jumlah baris, kata, dan karakter dari file baru.urut dengan menggunakan filter dan tambahkan data tersebut ke file baru.**

Untuk mendapatkan jumlah baris, kata, dan karakter (secara berurutan) dari sebuah file, gunakan perintah wc yang dipipakan dengan perintah cat. 
Hasilnya kemudian bisa ditambahkan ke file menggunakan ">>"

![Screenshot 2024-09-19 113542](https://github.com/user-attachments/assets/00cf823d-bf82-4930-8b8a-d5bb5cae12fa)

**8. Gunakan perintah di bawah ini dan perhatikan hasilnya:**

**cat /etc/passwd | sort | pr -n | grep tty03**

Menampilkan isi /etc/passwd, mengurutkannya, menomori barisnya, dan mencari baris yang mengandung tty03.

**find /etc –print | head**

Menampilkan 10 baris pertama dari daftar file dan direktori di dalam /etc.

**head /etc/passwd | tail -5 | sort**

Menampilkan 5 baris terakhir dari 10 baris pertama file /etc/passwd, kemudian mengurutkannya.

![Screenshot 2024-09-19 113847](https://github.com/user-attachments/assets/378da178-5adb-4686-9465-585416148e27)

**9. Gunakan perintah berikut dan perhatikan hasilnya:**

**who | cat | cat | sort | pr | head | cat | tail**

Menampilkan pengguna yang sedang login (who), mengurutkan hasilnya, memformat output, menampilkan baris pertama dan terakhir dari hasil tersebut.

![Screenshot 2024-09-19 114049](https://github.com/user-attachments/assets/d7fc6f84-4793-4371-b991-088cebc92f6d)

