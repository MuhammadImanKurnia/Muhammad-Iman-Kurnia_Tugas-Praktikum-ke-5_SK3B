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
   
   a. Untuk mengedit file /etc/profile, kita bisa menggunakan command sudo untuk mendapatkan hak akses super user, lalu menggunakan command nano untuk mengedit file                tersebut. Caranya, kita ketik sudo nano /etc/profile
      ![Screenshot from 2024-09-19 18-57-09](https://github.com/user-attachments/assets/82d22f41-4c7e-430c-bd0a-eb3d04b20465)
      
      Lalu kita ketik echo “Profile dari /etc/profile” dibaris paling bawah
      ![Screenshot from 2024-09-19 20-09-05](https://github.com/user-attachments/assets/3c0f6b88-4ea0-4fa4-a604-8c38a00d2b12)
      Kemudian kita tekan ctrl + x, lalu tekan Y, kemudian enter untuk keluar

   b. Edit semua profile yang ada di soal, kemudian cantumkan instruksi echo, misalnya pada /home/ mahasiswa/.bash_profile :  echo “Profile dari .bash_profile”. Caranya bisa       dilihat dari gambar berikut :
   
      - untuk .bash_profile
        ![Screenshot from 2024-09-19 19-25-48](https://github.com/user-attachments/assets/c0594b7d-f3e9-4b9a-8d5d-5801093847a9)
        ![Screenshot from 2024-09-19 19-18-10](https://github.com/user-attachments/assets/39c64fa6-43ef-4b9c-9221-ca75492d73ea)

      - untuk .bash_login
        ![Screenshot from 2024-09-19 19-26-00](https://github.com/user-attachments/assets/22a36a10-d3e4-48ed-be36-18504f1613d8)
        ![Screenshot from 2024-09-19 19-24-08](https://github.com/user-attachments/assets/61b061c0-7117-49ed-b2dc-994220bfb6e7)

      - untuk .profile (cantumkan intruksi echo dibaris terakhir)
        ![Screenshot from 2024-09-19 19-26-07](https://github.com/user-attachments/assets/c450a831-ceb2-4025-b025-1bb87bfaa965)
        ![Screenshot from 2024-09-19 19-23-23](https://github.com/user-attachments/assets/0a5c436b-c1a5-4d38-ba4d-2199562a25e9)

      - untuk .bashrc (cantumkan intruksi echo dibaris terakhir)
        ![Screenshot from 2024-09-19 19-26-14](https://github.com/user-attachments/assets/49c77e50-a62f-4306-b075-8de4fc5d50ef)
        ![Screenshot from 2024-09-19 19-25-15](https://github.com/user-attachments/assets/13e11c40-ae9a-4df6-9d4b-6ea7880aa3e7)

   c. Jalankan instruksi subtitute user (su dan su -), kemudian keluar dengan perintah exit. Caranya :
      ![Screenshot from 2024-09-19 19-45-43](https://github.com/user-attachments/assets/b245d68c-f87b-4284-ab70-68c672060d01)
      ![Screenshot from 2024-09-19 19-29-57](https://github.com/user-attachments/assets/f242bad0-0a98-40a5-8cb7-695971391cd6)
      Perbedaan dari kedua utilitas tersebut adalah, utilitas su untuk mengganti user tanpa mengubah environment, sedangkan su - untuk mengganti user dengan memuat                 environment (profile) dari user tersebut



        





   


