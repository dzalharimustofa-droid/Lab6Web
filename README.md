Lab6Web — Praktikum 6: JavaScript DOM dan Event Handling

Mata Kuliah: Pemrograman Web Pertemuan: 7 Program Studi: Teknik Informatika

Tujuan Praktikum
Memahami DOM sebagai representasi dokumen HTML yang dapat diakses melalui JavaScript.
Menggunakan id, class, dan selector CSS untuk memilih elemen HTML.
Mengubah teks, atribut, kelas CSS, dan gaya elemen melalui JavaScript.
Menangani event pengguna menggunakan addEventListener().
Membuat validasi form dan menampilkan pesan sesuai kondisi input.
Mengembangkan halaman interaktif dengan minimal tiga fungsi yang berjalan benar.
Struktur File
lab6_dom_event/
├── index.html    # Struktur halaman dan elemen setiap latihan
├── style.css     # Gaya tampilan (.highlight, .teks-besar, .selesai, li)
├── script.js     # Logika DOM dan event handling (Latihan 1–6)
└── README.md     # Dokumentasi praktikum
Cara Menjalankan
Pastikan perangkat memiliki browser modern (Chrome, Firefox, Edge) dan editor kode seperti Visual Studio Code.
Unduh atau clone repository ini, lalu buka folder lab6_dom_event.
Pastikan index.html, style.css, dan script.js berada dalam satu folder.
Buka index.html di browser (klik dua kali atau gunakan ekstensi Live Server di VS Code).
Buka Developer Tools/Console (tekan F12) untuk memeriksa error dan hasil program.
Langkah Kerja
Persiapan
Membuat folder kerja lab6_dom_event.
Membuat file index.html, style.css, dan script.js.
Menghubungkan CSS dan JavaScript dari index.html. Script dimuat dengan atribut defer agar dijalankan setelah HTML selesai diparsing.
Membuka halaman di browser dan mengaktifkan Developer Tools/Console.
Latihan 1 — Mengubah teks dengan DOM

Memilih elemen judul dan pesan dengan getElementById(), lalu mengubah isinya menggunakan textContent.

Latihan 2 — Event click

Menambahkan addEventListener("click", ...) pada tombol tombolAksi. Saat diklik, paragraf menampilkan waktu tindakan menggunakan new Date().toLocaleTimeString().

Latihan 3 — Mengubah kelas dan gaya CSS

Menambahkan kelas .highlight dan .teks-besar pada style.css. Tombol tombolGaya memakai classList.toggle() untuk menambah atau menghapus kelas pada paragraf teksGaya.

Latihan 4 — Event input dan penghitung karakter

Event input pada kolom namaInput memperbarui jumlah karakter di elemen jumlahKarakter secara langsung saat pengguna mengetik, menghapus, atau menempelkan teks.

Latihan 5 — Validasi form pendaftaran

Form berisi nama, email, dan usia. Pada event submit, event.preventDefault() mencegah halaman dimuat ulang, lalu input diperiksa:

Nama tidak boleh kosong.
Email harus sesuai pola email.
Usia harus berupa bilangan bulat 17–100.

Pesan kesalahan atau pesan sukses ditampilkan pada elemen pesanForm.

Skenario pengujian:

No	Kondisi	Hasil yang diharapkan
1	Semua input kosong	"Nama wajib diisi."
2	Nama kosong	"Nama wajib diisi."
3	Email tidak valid	"Masukkan email yang valid."
4	Usia di bawah 17	"Usia harus berupa bilangan bulat 17–100."
5	Semua input valid	"Validasi berhasil. Form siap diproses."
Latihan 6 — Daftar tugas sederhana (To-do List)

Tombol "Tambah" membuat elemen li baru dengan createElement() dan menambahkannya ke daftar. Teks tugas ditampilkan dengan textContent. Tombol "Tandai selesai" pada setiap tugas memakai classList.toggle("selesai") untuk mencoret teks. Jika input kosong, muncul pesan "Tulis tugas terlebih dahulu."
![alt text](?<img width="1600" height="899" alt="WhatsApp Image 2026-11-01 at 14 36 04" src="https://github.com/user-attachments/assets/6393cc5f-6b20-4a50-8deb-90dd4c99f113" />
raw=true)
![alt text](<img width="1600" height="899" alt="WhatsApp Image 2026-11-01 at 14 36 22" src="https://github.com/user-attachments/assets/f6773dbf-ad3e-4993-87dc-ce0c276870f4" />
?raw=true)
![alt text](<img width="1600" height="899" alt="WhatsApp Image 2026-11-01 at 14 36 40" src="https://github.com/user-attachments/assets/ecd0d9b2-7986-44de-86c7-ae0d0e6972f3" />
?raw=true)
![alt text](<img width="1600" height="446" alt="WhatsApp Image 2026-11-01 at 17 37 06" src="https://github.com/user-attachments/assets/55c1d6ee-742c-417b-a1b4-e70e1a87146f" />
?raw=true)
![alt text](<img width="1600" height="544" alt="WhatsApp Image 2026-11-01 at 17 37 32" src="https://github.com/user-attachments/assets/86307d64-8546-4687-91cb-d2e78c3b933a" />
?raw=true)
![alt text](<img width="1600" height="544" alt="WhatsApp Image 2026-11-01 at 17 37 32" src="https://github.com/user-attachments/assets/ac392557-df51-48a6-8b48-b31119a94425" />
?raw=true)
![alt text](<img width="1600" height="549" alt="WhatsApp Image 2026-11-01 at 17 38 08" src="https://github.com/user-attachments/assets/6140e47d-49fd-4d59-9ae2-8b6d76c101a7" />
?raw=true)
![alt text](<img width="1600" height="848" alt="WhatsApp Image 2026-11-01 at 17 44 02" src="https://github.com/user-attachments/assets/01fafe8c-87c5-4ed9-b65c-d961f3cfbe47" />
?raw=true)
