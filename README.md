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

    a. Untuk membuat script p1.sh, p2.sh, dan p3.sh, kita bisa menggunakan command nano, kemudian isi dengan command yang sudah ada di soal. Caranya bisa dilihat dari              gambar berikut :

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

    

    
    

      




    



        





   


