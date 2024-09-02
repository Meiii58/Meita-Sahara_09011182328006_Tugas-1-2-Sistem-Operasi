# Cara Menginstal Linux pada Virtual Box

## Langkah-langkah:

1. *Download Virtual Box*
   
   ![Virtual Box Download](https://github.com/Meiii58/Meita-Sahara_09011182328006_Tugas-1-2-Sistem-Operasi/blob/main/Gambar1.png)

2. *Buka Virtual Box, lalu klik "New" untuk membuat mesin virtual baru. Berikan nama dan pilih ISO yang akan digunakan.*
   ![Membuat Mesin Virtual Baru](https://github.com/Meiii58/Meita-Sahara_09011182328006_Tugas-1-2-Sistem-Operasi/blob/main/Gambar2.png)

3. *Atur "Base Memory" hingga warna menjadi hijau, lalu atur "Processors" menjadi 2. Setelah itu, klik "Next".*
   ![Pengaturan Memori dan Prosesor](https://github.com/Meiii58/Meita-Sahara_09011182328006_Tugas-1-2-Sistem-Operasi/blob/main/Gambar3.png)

4. *Buat ukuran "Disk Size" menjadi 25,00 GB, lalu klik "Next".*
   ![Pengaturan Ukuran Disk](https://github.com/Meiii58/Meita-Sahara_09011182328006_Tugas-1-2-Sistem-Operasi/blob/main/Gambar4.png)

5. *Klik "Settings", lalu pilih "Display". Atur "Video Memory" menjadi 128 MB, "Monitor Count" menjadi 1, dan "Scale Factor" menjadi 100%.
   Setelah itu, klik "OK".*

   ![Pengaturan Display](https://github.com/Meiii58/Meita-Sahara_09011182328006_Tugas-1-2-Sistem-Operasi/blob/main/Gambar5.png)

7. *Setelah mengatur virtual hard disk, tampilan virtual box akan terlihat seperti ini, dan instalasi siap dilakukan.*
   ![Tampilan Akhir Konfigurasi](https://github.com/Meiii58/Meita-Sahara_09011182328006_Tugas-1-2-Sistem-Operasi/blob/main/Gambar6.png)

8. *Untuk menjalankan mesin virtual, klik tombol "START" di sebelah tombol "SETTING".*
   ![Menjalankan Mesin Virtual](https://github.com/Meiii58/Meita-Sahara_09011182328006_Tugas-1-2-Sistem-Operasi/blob/main/Gambar7.png)

9. *Setelah mesin virtual berjalan, klik "Install Linux Mint".*
   ![Memulai Instalasi Linux Mint](https://github.com/Meiii58/Meita-Sahara_09011182328006_Tugas-1-2-Sistem-Operasi/blob/main/Gambar8.jpg)

10. *Centang opsi "Pasang codec-codec multimedia", lalu klik "Lanjutkan".*
   ![Menginstal Codec Multimedia](https://github.com/Meiii58/Meita-Sahara_09011182328006_Tugas-1-2-Sistem-Operasi/blob/main/Gambar9.jpg)

11. *Pilih "Hapus disk dan pasang Linux Mint", lalu klik "Pasang sekarang".*
    ![Memilih Opsi Instalasi](https://github.com/Meiii58/Meita-Sahara_09011182328006_Tugas-1-2-Sistem-Operasi/blob/main/Gambar10.jpg)

12. *Setelah muncul tampilan konfirmasi, klik "Lanjutkan".*
    ![Konfirmasi Instalasi](https://github.com/Meiii58/Meita-Sahara_09011182328006_Tugas-1-2-Sistem-Operasi/blob/main/Gambar11.jpg)

13. *Selanjutnya, pilih lokasi yang akan dijadikan zona waktu.*
    ![Memilih Zona Waktu](https://github.com/Meiii58/Meita-Sahara_09011182328006_Tugas-1-2-Sistem-Operasi/blob/main/Gambar12.jpg)

14. *Masukkan nama pengguna dan buat sandi. Anda juga dapat memilih untuk login secara otomatis atau memerlukan sandi.*
    ![Konfigurasi Pengguna](https://github.com/Meiii58/Meita-Sahara_09011182328006_Tugas-1-2-Sistem-Operasi/blob/main/Gambar13.jpg)

15. *Tunggu hingga proses instalasi selesai.*
    ![Proses Instalasi Berjalan](https://github.com/Meiii58/Meita-Sahara_09011182328006_Tugas-1-2-Sistem-Operasi/blob/main/Gambar14.jpg)

16. *Setelah instalasi selesai, klik "Nyalakan ulang sekarang".*
    ![Selesai Instalasi](https://github.com/Meiii58/Meita-Sahara_09011182328006_Tugas-1-2-Sistem-Operasi/blob/main/Gambar15.jpg)

17. *Jika muncul tampilan seperti ini, maka instalasi Linux Mint telah selesai.*
    ![Tampilan Setelah Instalasi](https://github.com/Meiii58/Meita-Sahara_09011182328006_Tugas-1-2-Sistem-Operasi/blob/main/Gambar16.jpg)

## Analisis Gambar

![Partisi Root](https://github.com/Meiii58/Meita-Sahara_09011182328006_Tugas-1-2-Sistem-Operasi/blob/main/Gambar17.png)

Saat instalasi, perlu memilih "/" pada opsi "Mount Point" karena tanda "/" adalah tanda root dari partisi. Partisi root merupakan partisi tertinggi di Linux, yang hampir sama dengan drive C: di Windows. Memilih "/" sebagai Mount Point adalah langkah penting untuk memastikan sistem operasi dapat berfungsi dengan benar dan memiliki akses ke seluruh struktur file yang diperlukan.

## Penjelasan Sistem File

a. *Ext4 (4th Extended File System)*: Dirilis secara komplit dan stabil berawal dari kernel 2.6.28 jadi apabila distro anda yang secara    default memiliki versi kernel tersebuat atau di atas nya otomatis system anda sudah support ext4 (dengan catatan sudah di include kedalam kernelnya) selain itu versi e2fsprogs harus mengunakan versi 1.41.5 atau lebih. Apabila anda masih menggunakan fs ext3 dapat mengkonversi ke ext4 dengan beberapa langkah yang tidak terlalu rumit. Keuntungan yang bisa didapat dengan mengupgrade filesystem ke ext4 dibanding ext3 adalah mempunyai pengalamatan 48-bit block yang artinya dia akan mempunyai 1EB = 1,048,576 TB ukuran maksimum filesystem dengan 16 TB untuk maksimum file size nya,Fast fsck,Journal checksumming,Defragmentation support.

b. *Ext3*: Ext3 adalah peningkatan dari sistem file Ext2. Peningkatan ini memiliki beberapa keuntungan,    diantaranya:
1.JournalingDengan menggunakan journaling, maka waktu recovery pada shutdownmendadak tidak
    akan selama pada Ext2. Namun ini menjadi kekurangan dariExt3, karena dengan adanya fitur 
    journaling, maka membutuhkan memoriyang lebih dan memperlambat operasi I/O (Input/Output).
2.Integritas dataExt3 menjamin adanya integritas data setelah terjadi kerusakan atau uncleanshut down.
   Ext3 memungkinkan kita memilih jenis dan tipe proteksi dari data.
3.KecepatanDaripada menulis data lebih dari sekali, Ext3 mempunyai throughput yanglebih besar 
   daripada Ext2 karena Ext3 memaksimalkan pergerakan head harddisk. Kita bisa memilih tiga jurnal
   mode untuk memaksimalkan kecepatan,tetapi integritas data tidak terjamin.
4.Mudah dilakukan migrasi dari sistem file Ext2 ke sistem file Ext3 tanpamelakukan format ulang.

c. *Swap*: Swap dalah opsi saat memformat drive, tetapi bukan sistem file yang sebenarnya. Ini digunakan sebagai memori virtual dan tidak memiliki struktur sistem file. Kalian tidak dapat memasang itu untuk melihat isinya. Swap digunakan sebagai “scratch spacel” atau ruang awal oleh kernel Linux untuk menyiman sementara data yang tidak dapat ditamung dalam RAM. Ini juga digunaka untuk berhibenasi. Sementara Windows menyimpn file paging-nya sebagai file di partisi sistem utamanya, Linux hanya menyimpan partisi kosong yang terisah untuk ruang swap.

d. *NTFS (New Technology File System)*: NTFS di kenalkan pertama pada Windows NT dan merupakan file systemyang benar benar berbeda di banding teknologi FAT. NTFS menawarkan securityyang jauh lebih baik, kompresi file, cluster dan bahkan support enkripsi data. NTFSmerupakan file system standar untuk Windows Xp dan apabila anda melakukanupgrade Windows biasa anda akan di tanyakan apakah ingin mengupgrade ke NTFSatau tetap menggunakan FAT. Namun jika anda sudah melakukan upgrade padaWindows Xp dan tidak melakukan perubahan NTFS itu bukan masalah karena anda bisa mengkonversinya ke NTFS kapanpun. 

  Namun ingat bahwa apabila anda sudah menggunakan NTFS akan munculmasalah jika ingin downgrade ke FAT tanpa kehilangan data.Umumnya NTFS tidak kompatibel dengan Operating System lain yang terinstall di komputer yang sama(Double OS) bahkan juga tidak terdeteksi apabila anda melakukan startup-bootmenggunakan floopy. Untuk itu sangat disarankan kepada anda untuk menyediakan partisi yang kecil saja yang menggunakan file system FAT di awal partisi. Partisi inidapat anda gunakan untuk menyimpan Recovery Tool apabila mendapat masalah.

e. *FAT32 (File Allocation Table 32)*: FAT32 mulai di kenal pada sistim Windows 95 SP2, dan merupakan pengembangan lebih dari FAT16. FAT32 menawarkan kemampuan menampung jumlat cluster yang lebih besar dalam partisi. Selain itu juga mengembangkan kemampuan harddisk menjadi lebih baik dibanding FAT16. Namun FAT32 memiliki kelemahan yang tidak di miliki FAT16 yaitu terbatasnya Operating System yang bisa mengenal FAT32.
     Tidak seperti FAT16 yang bisa di kenal oleh hampir semua system operasi, namun itu bukan masalah apabila anda menjalankan FAT32 di Windows XP karena Windows XP tidak peduli file sistim apa yang di gunakan pada partisi.

f. *BTRFS (B-Tree File System)*: Kadang singkatan ini juga diucapkan BuTteR FS atau BeTteR FS merupakan sebuah file system di bawah lisensi General Public License (GPL). Chris Mason, Direktur Linux Kernel Engineering di Oracle, merupakan “bapak” dari BTRFS yang pertama kali memulai pembuatan file system yang salah satu fiturnya adalah memaintain checksum dari seluruh file data dan metadata ini. File system sendiri adalah sebuah mekanisme penyimpanan dan pengaturan file atau data pada sebuah komputer.
      B-Tree File System ini membuat Linux dapat lebih “mengatur” storage atau tempat penyimpanan yang ada. “Mengatur” dalam hal ini bukan berarti hanya mengatur dalam hal pengalamatan saja, namun juga dapat melakukan administrasi dan pengelolaan tempat penyimpanan tersebut dengan interface yang lebih bersih sehingga pengguna dapat melihat apa yang sedang dipakai dan dikerjakan dan juga membuatnya menjadi lebih “terpercaya”.
