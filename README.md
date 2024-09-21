# Muhammad-Iman-Kurnia_Tugas-Praktikum-ke-5_SK3B
Tugas Praktikum ke 5

Nama  : Muhammad Iman Kurnia

NIM   : 09011282328044

Kelas : SK3B

1. Eksekusi seluruh profile yang ada :
   
   a. Edit file profile /etc/profile dan tampilkan pesan sebagai berikut :

       echo “Profile dari /etc/profile”

   b. Asumsi nama anda stD02001, maka edit semua profile yang ada yaitu :

       /home/stD02001/.bash_profile

       /home/. stD02001/.bash_login
  
       /home/mahasiswa/.profile

       /home/mahasiswa/.bashrc

      Ganti nama /home/mahasiswa dengan nama anda sendiri. Pada setiap file tersebut, cantumkan instruksi echo, misalnya pada /home/ mahasiswa/.bash_profile :

       echo “Profile dari .bash_profile”

      Lakukan hal yang sama untuk file lainnya, sesuaikan tampilan dengan nama file yang bersangkutan.

  c. Jalankan instruksi subtitute user, kemudian keluar dengan perintah exit sebagai berikut:

      $ su mahasiswa

      $ exit
     
     kemudian gunakan opsi – sebagai berikut :

      $ su – mahasiswa

      $ exit

     Jelaskan perbedaan kedua utilitas tersebut

   Jawab :
   
   a. Untuk mengedit file /etc/profile, kita bisa menggunakan command sudo untuk mendapatkan hak akses super user, lalu menggunakan command nano untuk mengedit file               tersebut. Caranya, kita ketik sudo nano /etc/profile
      ![Screenshot from 2024-09-19 18-57-09](https://github.com/user-attachments/assets/82d22f41-4c7e-430c-bd0a-eb3d04b20465)
      Lalu kita tambahkan echo “Profile dari /etc/profile”
      ![Screenshot from 2024-09-20 22-34-20](https://github.com/user-attachments/assets/2d0ea8a7-1553-46d1-8614-a9d2730592c2)
      Kemudian kita tekan ctrl + x, lalu tekan Y, kemudian enter untuk keluar

   b. Edit semua profile yang ada di soal, kemudian cantumkan instruksi echo, misalnya pada /home/nama user/.bash_profile :  echo “Profile dari .bash_profile”. Caranya            bisa dilihat dari gambar berikut :
   
      - untuk .bash_profile
   ![Screenshot from 2024-09-19 19-25-48](https://github.com/user-attachments/assets/c0594b7d-f3e9-4b9a-8d5d-5801093847a9)
   ![Screenshot from 2024-09-19 19-18-10](https://github.com/user-attachments/assets/39c64fa6-43ef-4b9c-9221-ca75492d73ea)

      - untuk .bash_login
   ![Screenshot from 2024-09-19 19-26-00](https://github.com/user-attachments/assets/22a36a10-d3e4-48ed-be36-18504f1613d8)
   ![Screenshot from 2024-09-19 19-24-08](https://github.com/user-attachments/assets/61b061c0-7117-49ed-b2dc-994220bfb6e7)

      - untuk .profile 
   ![Screenshot from 2024-09-19 19-26-07](https://github.com/user-attachments/assets/c450a831-ceb2-4025-b025-1bb87bfaa965)
   ![Screenshot from 2024-09-20 22-37-10](https://github.com/user-attachments/assets/74784d14-79cb-473d-93ba-b7b33234c1d5)

      - untuk .bashrc 
   ![Screenshot from 2024-09-19 19-26-14](https://github.com/user-attachments/assets/49c77e50-a62f-4306-b075-8de4fc5d50ef)
   ![Screenshot from 2024-09-20 22-36-58](https://github.com/user-attachments/assets/27d7dffa-5855-496f-9a0a-4b642bf16afa)

   c. Jalankan instruksi subtitute user (su dan su -), kemudian keluar dengan perintah exit. Caranya :
      ![Screenshot from 2024-09-19 19-45-43](https://github.com/user-attachments/assets/b245d68c-f87b-4284-ab70-68c672060d01)
      ![Screenshot from 2024-09-20 22-40-42](https://github.com/user-attachments/assets/be4fc7fb-7278-4887-9921-5afef790a93d)
      ![Screenshot from 2024-09-20 22-42-45](https://github.com/user-attachments/assets/314dbcc2-3b97-4a9c-8a9e-a44320060567)
      Perbedaan dari kedua utilitas tersebut adalah, utilitas su untuk mengganti user tanpa mengubah environment, sedangkan su - untuk mengganti user dengan memuat                environment (profile) dari user tersebut

2. Prompt String (PS)
   
   a. Edit file .bash_profile, ganti prompt PS1 dengan ‘>’. Instruksi export diperlukan dengan parameter nama variable tersebut, agar perubahan variable PS1 dikenal oleh          semua shell
   
        PS1='> '
   
        export PS1
   
   b. Eksperimen hasil PS1 :

        $ PS1=“\! > “
   
        69 > PS1=”\d > “
   
        Mon Sep 23 > PS1=”\t > “
   
        10:10:20 > PS1=”Saya=\u > “
   
        Saya=mahasiswa > PS1=”\w >”
   
        ~ > PS1=\h >”

    Jawab :

    a. Untuk mengedit file .bash_profile, kita bisa menggunakan command nano. Cara nya kita ketik nano /home/nama user/.bash_profile
       ![Screenshot from 2024-09-20 14-15-58](https://github.com/user-attachments/assets/aff3f5cc-2f92-4b16-b913-82e510378366)
       Kemudian kita tambahkan PS1='> ', ini untuk mengganti command PS1 dengan '>', lalu dibawahnya kita tambahkan export PS1, agar perubahan variable PS1 dikenal oleh            semua shell
       ![Screenshot from 2024-09-20 14-15-41](https://github.com/user-attachments/assets/94ae5e17-090c-4049-996d-422f710b119c)
       Jangan lupa di save

    b. Kemudian kita jalankan beberapa command PS1 berikut :

       - PS1='\! > ' (untuk menampilkan nomor perintah)

       - PS1='\d > ' (untuk menampilkan tanggal)

       - PS1='\t > ' (untuk menampilkan waktu)

       - PS1='Saya=\u > ' (untuk menampilkan username)

       - PS1='\w >' (untuk menampilkan direktori kerja saat ini)

       - PS1='\h >' (untuk menampilkan hostname)
   ![Screenshot from 2024-09-20 14-38-28](https://github.com/user-attachments/assets/d273fa3b-15f0-4584-a26a-4044b6164ae8)

3. Logout
   
   Edit file .bash_logout, tampilkan pesan dan tahan selama 5 detik, sebelum eksekusi logout.
   
     Echo “Terima kasih atas sesi yang diberikan”
   
     Sleep 5
   
     clear

   Jawab :

   Untuk mengedit file .bash_logout, kita menggunakan command nano. Caranya kita ketik nano /home/nama user/.bash_logout
   ![Screenshot from 2024-09-20 21-21-24](https://github.com/user-attachments/assets/036745a7-bf7a-4a48-b4b6-ec61860239a9)
   Setelah itu kita tambahkan command echo "Terima kasih atas sesi yang diberikan", kemudian di bawahnya sleep 5, dan dibawahnya lagi clear
   ![Screenshot from 2024-09-20 21-21-36](https://github.com/user-attachments/assets/51034c7a-49ea-4430-a29c-af140cfcf9bb)
   command-command di atas berfungsi untuk menampilkan pesan "Terima kasih atas sesi yang diberikan", lalu menahan layar selama 5 detik agar pesan dapat terlihat sebelum       terminal menutup sesi, dan kemudian membersihkan terminal setelah pesan ditampilkan.

   Untuk melihat pesan tersebut, kita harus login dulu menggunakan command su -. Caranya kita ketik su - nama user, setelah itu kita gunakan command exit untuk logout dan      pesan pun ditampilkan
   ![Screenshot from 2024-09-20 21-22-26](https://github.com/user-attachments/assets/c648eb3c-f82d-4578-8a50-b876d5d41ec4)
   Setelah 5 detik, terminal akan dibersihkan.

4. Bash script
   
   a. Buat 3 buah script p1.sh, p2.sh, p3.sh dengan isi masing-masing :
   
      p1.sh
   
      #! /bin/bash
   
      echo “Program p1”
   
      ls –l
   
      p2.sh
   
      #! /bin/bash
   
      echo “Program p2”
   
      who
   
      p3.sh
   
      #! /bin/bash
   
      echo “Program p3”
   
      ps x
   
   b. Jalankan script tersebut sebagai berikut :

      $ ./p1.sh ; ./p3.sh ; ./p2.sh
   
      $ ./p1.sh &
   
      $ ./p1.sh & ./p2.sh & ./p3.sh &
   
      $ ( ./p1.sh ; ./p3.sh ) &

    Jawab :

    a. Untuk membuat script p1.sh, p2.sh, dan p3.sh, kita bisa menggunakan command nano, kemudian isi dengan command yang sudah ada di soal. Caranya bisa dilihat dari gambar berikut :

       - untuk p1.sh
   ![Screenshot from 2024-09-20 21-45-22](https://github.com/user-attachments/assets/299d4853-46c5-4cea-a089-55f5a6e64bcf)
   ![Screenshot from 2024-09-20 21-43-48](https://github.com/user-attachments/assets/27e928c3-5536-4e5e-ae63-e86158cb8add)

       - untuk p2.sh
   ![Screenshot from 2024-09-20 21-45-31](https://github.com/user-attachments/assets/6369f533-e78e-4084-a69d-a4422fba5280)
   ![Screenshot from 2024-09-20 21-44-23](https://github.com/user-attachments/assets/dee4337f-9a52-406d-b872-5af7b012c58a)

       - untuk p3.sh
   ![Screenshot from 2024-09-20 21-45-54](https://github.com/user-attachments/assets/6f7ed751-4cdd-455c-9c9e-eb7cc3a84f22)
   ![Screenshot from 2024-09-20 21-45-07](https://github.com/user-attachments/assets/f48ec12b-3e56-41f6-9f94-6e327d57436b)

    b. Lalu jalankan script tersebut dengan cara sebagai berikut :

        sebelum itu kita ubah dulu script menjadi executable dengan menggunakan command chmod +x. Caranya :    
   ![Screenshot from 2024-09-20 22-54-02](https://github.com/user-attachments/assets/bc52d8d5-c4d2-49ed-9c07-ace68b8625c8)

        - ./p1.sh ; ./p3.sh ; ./p2.sh (untuk menjalankan script secara berurutan)
   ![Screenshot from 2024-09-20 22-57-02](https://github.com/user-attachments/assets/c7c56aba-3185-4036-aad7-8e9148fa134f)

        - ./p1.sh & (untuk menjalankan script di background)
   ![Screenshot from 2024-09-20 23-00-04](https://github.com/user-attachments/assets/ca2c476c-faa1-4e2a-8fe3-e7ac5a12fe43)
          Pencet ctrl + c untuk keluar

        - ./p1.sh & ./p2.sh & ./p3.sh & (untuk menggabungkan foreground dan background)
   ![Screenshot from 2024-09-20 23-02-07](https://github.com/user-attachments/assets/b2982cea-4eef-41bf-9f70-5821d3bcde01)

        - ( ./p1.sh ; ./p3.sh ) & (untuk menjalankan beberapa script dalam satu block)
   ![Screenshot from 2024-09-20 23-03-31](https://github.com/user-attachments/assets/7ecd562b-f377-4aca-887e-3686e3f0f0d1)

5. Jobs
   
   a. Buat shell-script yang melakukan loop dengan nama pwaktu.sh, setiap 10 detik, kemudian menyimpan tanggal dan jam pada file hasil.
   
      #!/bin/bash
   
      while [ true ]
   
      do
   
        date >> hasil
   
        sleep 10
   
      done
   
   b. Jalankan sebagai background; kemudian jalankan satu program (utilitas find) di background sebagai berikut :
   
      $ jobs
   
      $ find / -print > files 2>/dev/null &
   
      $ jobs
   
   c. Jadikan program ke 1 sebagai foreground, tekan ^Z dan kembalikan program tersebut ke background
   
      $ fg %1
   
      $ bg
   
   d. Stop program background dengan utilitas kill
   
      $ ps x
   
      $ kill [Nomor PID]

   Jawab :

   a. Pertama-tama kita buat shell-script dengan nama pwaktu.sh, dengan menggunakan command nano
      ![Screenshot from 2024-09-21 23-25-55](https://github.com/user-attachments/assets/b5a105fd-4d37-47f1-acf2-53d3efa0e0ad)
      Kemudian isi shell-script itu dengan command seperti digambar berikut :
      ![Screenshot from 2024-09-21 20-56-54](https://github.com/user-attachments/assets/ec8bb392-f4ed-4fc8-89a4-8b821a528773)
      Command atau script pada gambar itu untuk menciptakan loop tak terhingga yang mencatat tanggal dan waktu saat ini ke dalam file bernama hasil setiap 10 detik. Output ditambahkan ke file tanpa menghapus isi        yang sudah ada, sehingga file tersebut terus diperbarui dengan waktu baru.

   b. buat shell-script diatas menjadi executable, dangan menggunakan command chmod +x pwaktu.sh
      ![image](https://github.com/user-attachments/assets/4583e879-7213-480c-8e21-0a785f002789)
      Kemudian jalankan script di background
      ![image](https://github.com/user-attachments/assets/27ec6346-7b86-4795-88fe-6a9557b79a7d)
      Lalu jalankan perintah berikut :
   
      - jobs
  
      - find / -print > files 2>/dev/null &
  
      - jobs
      ![image](https://github.com/user-attachments/assets/8e21247c-33e7-475e-a797-b65c1bd01dc5)
      Command jobs digunakan untuk melihat daftar proses yang berjalan di bakground, dan command find / -print > files 2>/dev/null & mencari semua file dan direktori mulai dari root (/), menyimpan hasilnya dalam        file bernama files, dan mengabaikan pesan kesalahan dengan mengarahkan output kesalahan ke /dev/null. Dengan penggunaan &, perintah ini dijalankan di latar belakang, memungkinkan pengguna untuk tetap              menggunakan terminal selama proses pencarian berlangsung.

   c. Lalu kita gunakan command berikut :

      - fg %1

      - bg
      ![image](https://github.com/user-attachments/assets/077cb575-1cea-4bc7-8582-091a0ca58f16)
      Command fg adalah untuk membawa proses dari background ke foreground, dimana %1, nomor 1 adalah proses dari pwaktu.sh, yang berarti command diatas membawa proses pwaktu.sh dari background ke foreground.           Lalu, untuk menghentikan prosesnya, kita bisa tekan ctrl + z. Kemudian kita menggunakan command bg, yang dimana command tersebut untuk mengembalikan proses pwaktu.sh itu ke background kembali

   d. Untuk menyetop program background, kita bisa menggunakan command kill. Tapi kita harus mencari nomor PID nya terlebih dahulu. Caranya kita bisa menggunakan command ps x
      ![image](https://github.com/user-attachments/assets/ed7634b8-74ed-469b-a534-d66e2d00128b)
      ![image](https://github.com/user-attachments/assets/7fc724fa-9877-4e80-bf8d-b4daa955e413)
      Bisa kita lihat kalau digambar menampilkan daftar proses yang sedang berjalan di back ground dan nomor PID nya (nomor PID itu yang paling kiri). Sekarang kita coba hapus salah satu proses background dari          pwaktu.sh dangan nomor PID 5688, caranya kita ketik kill 5688
      ![image](https://github.com/user-attachments/assets/8537293a-9d99-4980-9d33-40d02ce41cb5)
      Untuk melihat apakah proses tersebut sudah di kill atau si stop, kita pakai command ps x lagi saja
      ![image](https://github.com/user-attachments/assets/bba7f12e-e305-4fb5-9604-d3ede1814231)
      ![image](https://github.com/user-attachments/assets/331c8cc4-2faf-4e26-8e91-c0df0b415db6)
      Bisa kita lihat kalau ada tulisan Terminated ./pwaktu.sh, yang berarti proses nya sudah di stop

6. History
   
   a. Ganti nilai HISTSIZE dari 1000 menjadi 20
   
      $ HISTSIZE=20
   
      $ history
   
   b. Gunakan fasilitas history dengan mengedit instruksi baris ke 5 dari instruksi yang terakhir dilakukan
   
      $ !-5
   
   c. Ulangi instruksi yang terakhir. Gunakan juga ^P dan ^N untuk bernavigasi pada history bufer
   
      $ !!
   
   d. Ulangi instruksi pada history bufer nomor 150
   
      $ !150
   
   e. Ulangi instruksi dengan prefix “ls”
   
      $ !ls

   Jawab :

   a. Untuk mengganti HISTSIZE yang awalnya 1000 menjadi 20, kita bisa menggunakan command HISTSIZE=20, fungsinya adalah ketika menggunakan command history untuk melihat daftar history atau riwayat comman-              command yang kita gunakan sebelumnya, yang ditampilkan hanyalah 20 daftar saja yang awalnya 1000.
      ![image](https://github.com/user-attachments/assets/2b57ab8f-b8c8-4dfb-8cc1-287e93f3f354)

   b. Command !-5 berfungsi untuk melihat history nomor 5 dari yang paling terkhir, dan bisa kita lihat di daftar history di atas, nomor 5 dari terakhir adalah HISTSIZE=20, maka output yang ditampilkan adalah           HISTSIZE=20
      ![image](https://github.com/user-attachments/assets/835c27a5-456d-45b5-b349-4689f149517e)

   c. Command !! berfungsi untuk melihat perintah atau command yang terakhir kita pakai. Misal kita terakhir menggunakan command echo, maka ketika kita menjalankan command !!, outputnya yang ditampilkan adalah          echo
      ![image](https://github.com/user-attachments/assets/6c987fd2-8950-4889-b282-a5302bc87f5d)

   d. Untuk melihat history nomor 150, kita bisa menggunakan command !150
      ![image](https://github.com/user-attachments/assets/eaa914b9-d7f6-4777-928b-ad696d8db674)
      Bisa kita lihat di gambar diatas, ada tulisan event not found. Itu dikarenakan history nomor 150 tidak ada di dalam 20 daftar history yang sudah ditampilkan pada bagian a. Namun jika saya menggunakan nomor        yang ada didalam daftar history, misalnya nomor 599, yang dimana merupakan history dari ps x, maka itu akan mengulangi command atau instruksi dari ps x dan outputnya juga
      ![image](https://github.com/user-attachments/assets/2c417039-3260-44f6-a706-ce2fd02dd484)

   e. Untuk mengulangi instruksi dari command ls, kita bisa menggunakan command !ls
      ![image](https://github.com/user-attachments/assets/c1e94f75-023e-4e61-b8b9-8ed0fd2c3b30)
      Bisa kita lihat, lagi-lagi event not found. Sama seperti sebelumnya, itu berarti command ls tidak ada didalam 20 daftar history. Kalau begitu saya akan menggunakan command ls supaya ada didalam daftar             history
      ![image](https://github.com/user-attachments/assets/ff289c1a-bbfd-4c17-9a8f-cef217a080b6)
      Bisa kkta lihat, command ls sudah ada didalam daftar history, yaitu di nomor 613

      Nah, karena sudah ada didalam daftar, itu berarti kita bisa mengulang command ls dengan menggunakan !ls
      ![image](https://github.com/user-attachments/assets/ff26d172-a4d2-4245-9e74-92c5eebd31b1)







  






    

    
    

      




    



        





   


