
Nama    : Desi Yusmalinda

Nim     : 09030182428014


1. Login sebagai studentOS dan lihat status proses, perhatikan kolom keluaran ps –au sebagai berikut :

   a) Nama proses yang bukan root yaitu desiyus+

   
   b) PID dan COMMAND dari proses yang paling banyak menggunakan CPU Semua proses menunjukkan %CPU = 100 Maka dipilih proses yang aktif (R+): PID: 748 COMMAND: ps -au

      <img width="468" alt="desi1b" src="https://github.com/user-attachments/assets/d76c4d82-4bb5-45ef-ba78-a07801f970bf" />


   c) Buyut proses dan PID dari proses tersebut Tracing dari proses ps -au:

      <img width="290" alt="desi1c" src="https://github.com/user-attachments/assets/2c59ed49-26a9-4984-bb57-ee0663cceecc" />

    Jadi, buyut prosesnya adalah: PID: 1 COMMAND: /init


   d) beberapa proses daemon

      <img width="347" alt="desi1d" src="https://github.com/user-attachments/assets/519ccacc-d02a-47ae-acd2-fc64e93863ae" />


   e) Menjalankan perintah

  -$ csh

   <img width="451" alt="desi1e csh" src="https://github.com/user-attachments/assets/ac24f62c-eeff-4a7a-bdc1-5ccd4d9ccaa7" />


  -$ who , $ bash , dan $ ls

   <img width="468" alt="desi1e who,bash,ls" src="https://github.com/user-attachments/assets/212d397e-a267-48a8-8b16-221dd507be06" />


  -$ sh

   <img width="188" alt="desi1e sh" src="https://github.com/user-attachments/assets/c7fc075f-0651-4095-9f30-a82e22e22567" />


  -$ ps

   <img width="217" alt="desi1e ps" src="https://github.com/user-attachments/assets/00c8503a-0f1d-4078-a956-8e976d404e08" />

 PID terbesar: 931 (sh) Urutan lengkap sampai ke induk utama (PPID = 1) ditelusuri dengan ps -fp [PID]



   2. Program prog.sh dengan Trap
      
      a)  Buka file prog.sh

        <img width="277" alt="desi2 a" src="https://github.com/user-attachments/assets/12c5c4a8-981c-4038-b06a-64c5991f6757" />


      b) Menulis skrip

         <img width="251" alt="desi2 b" src="https://github.com/user-attachments/assets/f7e0b33f-2c79-4492-997c-87973d67c0f6" />


      c)Ubah file agar bisa dieksekusi, jalankan program sebagai background, dan catat nomor PID dari proses tersebut

         <img width="309" alt="desi2 c" src="https://github.com/user-attachments/assets/6c20a847-bdb2-4e16-98d3-664dc6c2107e" />


      d) Mengirim sinyal satu per satu

         <img width="315" alt="desi2 d" src="https://github.com/user-attachments/assets/8a86c6e5-adbc-488e-9ffc-9b274a9ac0be" />



      3. Program myjob.sh dengan Auto-Hapus File
         
       a) Buka file myjob.sh

         <img width="345" alt="desi3 a" src="https://github.com/user-attachments/assets/0c35c31f-cc2b-4ec5-8be3-7f32950cea2f" />


      b) Mengisi skrip

         <img width="350" alt="desi3 isi kript" src="https://github.com/user-attachments/assets/b5cdc442-2f15-4f81-86ad-d1ab67bb7696" />


      c) Buat executable, jalankan dibackground, dan Cek nomor PID nya

         <img width="236" alt="desi3 c1" src="https://github.com/user-attachments/assets/e31636e9-fdd2-4ff4-8008-a71c65f633e7" />

         <img width="352" alt="desi3 c2" src="https://github.com/user-attachments/assets/7d86de0d-cf5f-4320-b3f4-0dab29da945b" />

          
      d) Hentikan proses dengan sinyal 15

         <img width="260" alt="desi3- d" src="https://github.com/user-attachments/assets/e9bc098a-6af8-44e9-9c74-c9ed6c47dce0" />


      proses dihentikan dengan kill -15 481, muncul:

         <img width="297" alt="desi3 edihapus" src="https://github.com/user-attachments/assets/d2548604-87df-4fb2-856b-ee699d0ab5c2" />

        File berkas dan hasil otomatis terhapus Fungsi trap berjalan sukses.
