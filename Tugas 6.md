# PRAKTIKUM 5 - JOB CONTROL

### 1. Eksekusi seluruh profile yang ada
   - Edit file profile /etc/profile dan tampilkan pesan sebagai berikut:

      *__echo "Profile dari /etc/profile"__*

![Screenshot 2024-09-26 072129](https://github.com/user-attachments/assets/c7c9a6d8-89e5-4db9-afac-8563ffca9b07)

![Screenshot 2024-09-26 080600](https://github.com/user-attachments/assets/de2c5108-3b20-4a4f-a088-24dc28931fe7)


  - Asumsikan nama Anda stD02001, maka edit semua profile yang ada, yaitu:

     *__- /home/mahasiswa/.bash_profile__*

      *__- /home/mahasiswa/.bash_login__*

      *__- /home/mahasiswa/.profile__*
     
     *__- /home/mahasiswa/.bashrc__*
    
  ![Screenshot 2024-09-26 081059](https://github.com/user-attachments/assets/c945f5c7-d097-4e3d-ac30-19cbec16f87f)

  ![Screenshot 2024-09-26 081153](https://github.com/user-attachments/assets/45180e08-e989-488a-ba90-765c45327c51)

- Ganti nama /home/mahasiswa/ dengan nama Anda sendiri. Pada setiap file tersebut, tambahkan instruksi berikut:
    
     *__echo "Profile dari .bash_profile"__*

     Lakukan hal yang sama pada file yang lain

  ![Screenshot 2024-09-26 081542](https://github.com/user-attachments/assets/9e4cda8f-6903-4bc4-9b73-22dd4ce7f252)
  
  ![Screenshot 2024-09-26 081919](https://github.com/user-attachments/assets/310c5291-f1b7-49fd-a6fa-29c9f6d46264)
  
  ![Screenshot 2024-09-26 082033](https://github.com/user-attachments/assets/0074d950-84df-4c44-bfb7-28c40666713f)
  
  ![Screenshot 2024-09-26 082312](https://github.com/user-attachments/assets/64288d25-b526-48a1-ba16-b364d6021666)

** - Jalankan instruksi substitute user, kemudian keluar dengan perintah exit sebagai berikut:**

  ![Screenshot 2024-09-26 082503](https://github.com/user-attachments/assets/3c6d54e0-f66a-4aa9-866b-e5bb9c497887)

   Perbedaan kedua utilitas tersebut:
     
     __1. su mahasiswa:__

        Perintah ini menjalankan su untuk beralih ke user mahasiswa. Saat menggunakan perintah ini tanpa opsi -, lingkungan (environment) dari user saat ini tetap dipertahankan.
        Artinya, hanya identitas pengguna yang berubah, tetapi variabel lingkungan seperti PATH tidak akan berubah.
        Jadi, variabel lingkungan dan direktori kerja yang sedang aktif tetap sama seperti sebelumnya.
        
     __2. su - mahasiswa:__

        Perintah ini menggunakan opsi - yang dikenal sebagai login shell. Opsi ini melakukan login penuh sebagai user mahasiswa,
        sehingga environment yang dimuat adalah environment milik mahasiswa secara lengkap.
        Ini termasuk mengubah direktori kerja ke home directory user mahasiswa dan memuat variabel lingkungan seperti yang didefinisikan dalam shell milik mahasiswa.
        Jadi, ini seperti memulai sesi baru sebagai user mahasiswa.

### 2. Prompt String (PS1)
   - Edit file .bash_profile, ganti prompt PS1 dengan > sebagai prompt. Instruksi export diperlukan dengan parameter nama variable tersebut,
     agar perubahan variable PS1 dikenali oleh semua shell yang berjalan.

     ![Screenshot 2024-09-26 082929](https://github.com/user-attachments/assets/a2607931-b928-4b7d-a353-c413fa342429)

     ![Screenshot 2024-09-26 083041](https://github.com/user-attachments/assets/16a3d6c0-ddca-48aa-a1b8-c978359ed364)

     - Eksperimen hasil PS1.
    
     ![Screenshot 2024-09-26 083435](https://github.com/user-attachments/assets/780924be-506c-4602-a277-d5d0b746ca4f)


### 3. Logout
   - Edit file .bash_logout, tampilkan pesan dan tahan selama 5 detik, sebelum eksekusi logout:

     ![Screenshot 2024-09-26 083552](https://github.com/user-attachments/assets/0d5b874c-f5d2-4bfc-80ae-eb2ad0220b19)

     ![Screenshot 2024-09-26 083659](https://github.com/user-attachments/assets/9288c8c0-7d27-4bdf-bc6c-9ff9d714dce1)

### 4. Bash Script
   - Buat 3 buah script (p1.sh, p2.sh, p3.sh) dengan isi masing-masing:
     #### p1.sh
     
     *__#!/bin/bash__*
     
     *__echo "Program p2"__*
    
     *__ls -l__*
     
     #### p2.sh
     
     *__#!/bin/bash__*
     
     *__echo "Program p2"__*
     
     *__who__*

     #### p3.sh

     *__#!/bin/bash__*
     
     *__echo "Program p3"__*
     
     *__ps x__*

     ![Screenshot 2024-09-26 084138](https://github.com/user-attachments/assets/1c5ff8df-68a4-4185-9b11-987ec7343981)

     ![Screenshot 2024-09-26 084045](https://github.com/user-attachments/assets/33c32199-3bac-4982-9616-57a994f34950)

     ![Screenshot 2024-09-26 084104](https://github.com/user-attachments/assets/ec3b374c-9cfc-4240-9e8f-4deaa4de3898)

     ![Screenshot 2024-09-26 084121](https://github.com/user-attachments/assets/19460d94-c8d2-4344-9f86-e43cb706e6ed)

- Jalankan script tersebut

     ![Screenshot 2024-09-26 084500](https://github.com/user-attachments/assets/d18a6302-7efc-4719-bb93-01c9569556af)

     ![Screenshot 2024-09-26 084522](https://github.com/user-attachments/assets/952bf151-9661-46ce-8770-b6e834df3a33)

     ![Screenshot 2024-09-26 084544](https://github.com/user-attachments/assets/c59152e6-abe6-4d7e-8989-638ce89bd6f1)
  
     ![Screenshot 2024-09-26 084552](https://github.com/user-attachments/assets/c4bc273a-48eb-4240-a246-03be13f2f32d)

     ![Screenshot 2024-09-26 084825](https://github.com/user-attachments/assets/55bad321-4378-4376-85b9-03b94d9278ed)

     ![Screenshot 2024-09-26 085108](https://github.com/user-attachments/assets/ac75e328-e83b-44f8-8d28-b67b17a29057)

### 5. Jobs
   - Buat sebuah script looping melakukan loop dengan nama pwaktu.sh.  
     Setiap 10 detik, kemudian menyimpan tanggal dan jam pada file hasil:

     ![Screenshot 2024-09-26 085404](https://github.com/user-attachments/assets/67bbad4d-a07b-43ef-9e0a-1662e5445c14)

     ![Screenshot 2024-09-26 085438](https://github.com/user-attachments/assets/9611bc4a-417b-48d8-a41e-32c2e64d70a3)
  
   - Jalankan sebagai background, kemudian jalankan satu program (misalnya find) di background sebagai berikut:

     ![Screenshot 2024-09-26 085806](https://github.com/user-attachments/assets/00e92830-fd4f-4828-9e8b-81c9317abe8b)

   - Jadikan program find sebagai foreground, tekan ^Z dan kembalikan program tersebut ke background:

     ![Screenshot 2024-09-26 085918](https://github.com/user-attachments/assets/fdee60e2-ed86-4a1b-bad2-d91b3f523e64)

   - Stop program background dengan utilitas kill:

     ![Screenshot 2024-09-26 090020](https://github.com/user-attachments/assets/2a5a87a8-be2e-44e4-8795-705b52885301)

     ![Screenshot 2024-09-26 090113](https://github.com/user-attachments/assets/024b753e-171f-4f14-ae0b-93213cedd280)


### 6. *History*:
   - Saya mengganti nilai HISTSIZE = 20:

    ![Screenshot 2024-09-26 090609](https://github.com/user-attachments/assets/8fdf41ec-ecaf-4f2b-b4ae-2b9cc2e5a12d)

   - Gunakan fasilitas history dengan mengoreksi instruksi baris ke-10 dari instruksi yang terakhir dilakukan:

     ![Screenshot 2024-09-26 090701](https://github.com/user-attachments/assets/7a287049-c6d8-4161-8a3c-0921ef6d9e8d)  
     
   - Ulangi instruksi yang terakhir. Gunakan juga ^P dan ^N untuk beberapa perintah pada history buffer.

     ![Screenshot 2024-09-26 090856](https://github.com/user-attachments/assets/4aaae208-67a2-481c-894b-e918a26c6b5b)

   - Edit nilai HISTFILESIZE agar history buffer nomor 170.

     ![Screenshot 2024-09-26 091112](https://github.com/user-attachments/assets/ced3d25a-6a27-4442-854c-7da260fa4489)

   - Ulangi instruksi dengan grep "ls":

     ![Screenshot 2024-09-26 091227](https://github.com/user-attachments/assets/7ed720f9-dd92-41d5-b172-46875a66d2c5)
