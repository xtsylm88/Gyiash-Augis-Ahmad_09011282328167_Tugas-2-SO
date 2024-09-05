# 1. Instalasi ubuntu VMware
![Screenshot 2024-09-05 104423](https://github.com/user-attachments/assets/4082b27c-924d-4a21-b970-f547683f64f6)
![Screenshot 2024-09-05 104528](https://github.com/user-attachments/assets/8bae2add-11ee-4d7d-b431-f4d64d7026c6)


Bentuk tampilan setelah dimasukkan kata sandi.
![Screenshot 2024-09-05 112050](https://github.com/user-attachments/assets/bb11968e-2635-4fb0-9674-72efe0ab1ea5)


# 2. Mengapa pada saat instalasi perlu dipilih “/” pada opsi Mount Point ?
Pada proses instalasi diperlukan “/” pada opsi Mount Point karena ini adalah simbol untuk 
direktori root, yaitu tempat utama di mana semua file sistem Linux disimpan. Dengan memilih 
"/" sebagai Mount Point, kita memberitahu sistem untuk menempatkan semua file penting di 
partisi ini sehingga sistem bisa berjalan dengan baik setelah instalasi selesai. Kalau tidak kita 
pilih maka sistem akan bingung untuk meletakkan dimana file tersebut dan bisa membuat 
instalasi gagal.

# 3. Berikan Penjelasan ext4, ext3, swap, ntfs, fat32, btrfs !
1. ext4 
- Penggunaan: Umumnya digunakan di sistem Linux.
- Kelebihan: Menyediakan fitur seperti journaling, yang meningkatkan keandalan 
data dengan menyimpan perubahan pada log sebelum menulis ke disk. 
Mendukung volume dan ukuran file yang sangat besar.
- Kekurangan: Meskipun stabil, tidak memiliki beberapa fitur canggih yang ada 
pada sistem file modern seperti Btrfs.
2. ext3 
- Penggunaan: Juga digunakan di sistem Linux.
- Kelebihan: Memperkenalkan fitur journaling untuk meningkatkan keandalan 
data. Lebih stabil dibandingkan ext2, tetapi tidak seefisien ext4.
- Kekurangan: Tidak mendukung ukuran file dan volume sebesar ext4 dan tidak 
secepat ext4 dalam hal kinerja.
3. swap
- Penggunaan: Berfungsi sebagai area penyimpanan tambahan untuk RAM di 
sistem Linux.
- Kelebihan: Membantu sistem untuk menjalankan aplikasi lebih besar dari 
kapasitas RAM yang tersedia dengan menyimpan data sementara di disk.
- Kekurangan: Akses ke swap lebih lambat dibandingkan RAM, sehingga kinerja 
sistem bisa terpengaruh jika terlalu bergantung pada swap.
4. ntfs (New Technology File System)
- Penggunaan: Sistem file utama untuk Windows NT dan sistem operasi yang lebih 
baru (seperti Windows 10/11).
- Kelebihan: Mendukung fitur seperti enkripsi, kompresi, dan hak akses file yang 
lebih canggih dibandingkan FAT32. Memungkinkan volume dan file yang sangat 
besar.
- Kekurangan: Kurang kompatibel dengan sistem operasi non-Windows, meskipun 
dukungan untuk baca/tulis NTFS ada di beberapa sistem Linux
5. fat32 (File Allocation Table 32)
- Penggunaan: Sistem file yang lebih tua yang digunakan di berbagai sistem 
operasi, termasuk Windows, macOS, dan Linux.
- Kelebihan: Kompatibel dengan hampir semua sistem operasi, ideal untuk 
perangkat penyimpanan portabel seperti USB flash drive.
- Kekurangan: Tidak mendukung file yang lebih besar dari 4 GB dan volume lebih 
besar dari 8 TB. Tidak memiliki fitur seperti journaling.
6. btrfs (B-tree File System)
- Penggunaan: Sistem file yang relatif baru untuk Linux, dirancang untuk 
menggantikan ext4.
- Kelebihan: Menawarkan fitur canggih seperti snapshot, pengendalian kesalahan, 
dan kompresi data. Fleksibel dan mendukung pengelolaan volume yang lebih 
kompleks.
- Kekurangan: Masih dianggap kurang stabil dibandingkan ext4 dan mungkin tidak 
selalu cocok untuk semua jenis penggunaan.


