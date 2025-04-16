
Nama    : Desi Yusmalinda

Nim     : 09030182428014


1. Login sebagai studentOS dan lihat status proses, perhatikan kolom keluaran ps –au sebagai berikut :

   a) Nama proses yang bukan root yaitu desiyus+

   
   b) PID dan COMMAND dari proses yang paling banyak menggunakan CPU Semua proses menunjukkan %CPU = 100 Maka dipilih proses yang aktif (R+): PID: 748 COMMAND: ps -au

       <img width="468" alt="desi1b" src="https://github.com/user-attachments/assets/dd9a323e-1656-43f7-b69d-eda8f5d01de0" />


   c) Buyut proses dan PID dari proses tersebut Tracing dari proses ps -au:

        <img width="290" alt="desi1c" src="https://github.com/user-attachments/assets/05eab37f-e78f-4b7f-bacc-8fbc9138e114" />

    Jadi, buyut prosesnya adalah: PID: 1 COMMAND: /init


   d) beberapa proses daemon

        <img width="347" alt="desi1d" src="https://github.com/user-attachments/assets/9d727360-8a0f-41dc-9807-75cafc44a2e0" />


   e) Menjalankan perintah

  -$ csh

      <img width="451" alt="desi1e csh" src="https://github.com/user-attachments/assets/a451c803-e3d6-4d1d-9d5f-42ea45414029" />


  -$ who , $ bash , dan $ ls

      <img width="468" alt="desi1e who,bash,ls" src="https://github.com/user-attachments/assets/92e212d7-8226-4353-901f-cfab718707db" />


  -$ sh

      <img width="188" alt="desi1e sh" src="https://github.com/user-attachments/assets/b61e6e4f-8e18-4804-b27e-664d47ae8ebd" />


  -$ ps

      <img width="217" alt="desi1e ps" src="https://github.com/user-attachments/assets/bbdd3a8a-8da2-4a98-a1f5-439a4956f488" />

  PID terbesar: 931 (sh) Urutan lengkap sampai ke induk utama (PPID = 1) ditelusuri dengan ps -fp [PID]



   2. Program prog.sh dengan Trap
      
      a)  Buka file prog.sh

          <img width="277" alt="desi2 a" src="https://github.com/user-attachments/assets/fb64533e-81ef-4c5d-a27d-19bff4180cb5" />


      b) Menulis skrip

          <img width="251" alt="desi2 b" src="https://github.com/user-attachments/assets/80e9e655-3c99-4b1c-ab6a-1da5935b0b7f" />


      c)Ubah file agar bisa dieksekusi, jalankan program sebagai background, dan catat nomor PID dari proses tersebut

          <img width="309" alt="desi2 c" src="https://github.com/user-attachments/assets/16a63b50-cd56-4a07-83fb-e58550f31b67" />


      d) Mengirim sinyal satu per satu

          <img width="315" alt="desi2 d" src="https://github.com/user-attachments/assets/013ba8d1-d11f-4300-afde-d01ecd5a46ca" />



      3. Program myjob.sh dengan Auto-Hapus File
         
       a) Buka file myjob.sh

          <img width="345" alt="desi3 a" src="https://github.com/user-attachments/assets/617fc987-3d77-4232-b2b9-75a504165259" />


      b) Mengisi skrip

          <img width="350" alt="desi3 isi kript" src="https://github.com/user-attachments/assets/e0ae52d8-41b8-4ec0-be4d-f36721f18566" />


      c) Buat executable, jalankan dibackground, dan Cek nomor PID nya

          <img width="236" alt="desi3 c1" src="https://github.com/user-attachments/assets/b0447f49-15c7-4ce8-be04-1cf8a661a8b1" />

          <img width="352" alt="desi3 c2" src="https://github.com/user-attachments/assets/b0da34a6-50af-4ea1-9b20-c9398f06051b" />


      d) Hentikan proses dengan sinyal 15

          <img width="260" alt="desi3- d" src="https://github.com/user-attachments/assets/35cf80e2-87e5-4b53-9d96-2574a5bc21c8" />

      proses dihentikan dengan kill -15 481, muncul:

          <img width="297" alt="desi3 edihapus" src="https://github.com/user-attachments/assets/1cf8cda5-b973-4b7a-a147-7a3a13a8ee37" />
      
      File berkas dan hasil otomatis terhapus Fungsi trap berjalan sukses.
