# Latihan: Membuat tindakan percakapan

Dalam latihan ini, Anda akan membuat tindakan percakapan yang menyediakan informasi tentang proyek organisasi fiksi berjudul "Project ABC".

Tugas latihan:

- Membuat tindakan percakapan di Copilot Studio
- Menerbitkan tindakan percakapan ke Microsoft Copilot
- Menguji tindakan percakapan Anda di Microsoft Copilot

## Tugas 1: (Opsional) Uji pengalaman default

Untuk memulai, ajukan pertanyaan tentang proyek ABC di Microsoft 365 Copilot.

1. Buka **Microsoft Teams** dan masuk dengan akun kerja atau sekolah Anda.

1. Pilih **Obrolan** di bar samping.

1. Pilih **Copilot** di menu obrolan.

1. Dalam kotak tulis pesan, masukkan `Who should I contact for questions about Project ABC?`

1. Perhatikan bahwa Microsoft 365 Copilot saat ini tidak memiliki informasi apa pun tentang Project ABC.

## Tugas 2: Membuat tindakan percakapan baru

Pertama, konfigurasikan nama, solusi, dan skema untuk tindakan percakapan baru di Microsoft Copilot.

1. Di browser web Anda, navigasikan ke [Copilot Studio](https://copilotstudio.microsoft.com) dan masuk dengan akun kerja atau sekolah Anda, jika diminta.  Pilih **lewati** untuk melewati pesan selamat datang apa pun.

    **Catatan:** Pertama kali Anda membuka Copilot Studio, tampilan yang muncul dapat berupa antarmuka obrolan untuk membuat copilot pertama Anda. Jika ini terjadi, pilih **...** menu di kanan atas (di samping tombol **Buat** ) lalu pilih **Batalkan pembuatan copilot** lalu **biarkan** untuk meninggalkan antarmuka obrolan dan menampilkan halaman beranda Copilot Studio.
1. Pilih **Pustaka** di navigasi kiri. Di sini, Anda dapat melihat daftar tindakan dan konektor yang sudah ada dan membuat yang baru.
1. Pilih **Tambahkan item** di bagian atas.  Menu mencantumkan 2 opsi untuk memperluas Copilot untuk Microsoft 365.
:::image type="content" source="../Media/extend copilot options.png" alt-text="Window mencantumkan 2 opsi untuk memperluas Copilot: membuat copilot atau membuat tindakan.":::
1. Pilih **Tindakan baru**.

1. Pilih **Percakapan** untuk membuat tindakan percakapan.

1. Di **bidang nama** masukkan `Project ABC` dan terima solusi dan skema default.

1. Pilih **Buat** untuk melanjutkan. Tindakan percakapan baru Anda dibuat. Ini akan memakan waktu beberapa detik. Setelah selesai, Anda dijatuhkan ke kanvas penulisan untuk terus mengonfigurasi tindakan Anda.

## Tugas 3: Mengonfigurasi topik

Selanjutnya, konfigurasikan nama dan pemicu untuk topik tersebut.

1. Di panel penulisan tindakan percakapan, navigasikan ke tab **Topik** .

1. Pilih kotak teks **Nama topik** di bagian atas panel, yang secara default adalah nama `"Untitled"` dan masukkan `Project ABC info` untuk menamai topik.

1. Di simpul **Pemicu** dalam topik, pilih kotak teks di bawah teks "Jelaskan apa yang dilakukan topik" lalu masukkan `Answers questions and provides information about Project ABC, including questions about objectives, points of contact, and rollout timeline.`.

## Tugas 4: Mengirim pesan

Selanjutnya, tambahkan simpul ke topik untuk mengirim pesan tentang Project ABC.

1. Di bawah simpul Pemicu, pilih **+** ikon untuk menambahkan simpul baru.

1. Di menu yang ditampilkan, pilih **Kirim pesan**.  Simpul pesan baru dibuat.

1. Pada simpul pesan, pilih kotak teks dan masukkan `Project ABC is an initiative aimed at improving the culture and engagement within the company.  Objectives of the project include improved morale, increased employee survey results, and improved culture ratings.  For more information about Project ABC, contact Devon Torres.`.

1. Pilih **Simpan** di atas kanvas penulisan untuk menyimpan perubahan.

## Tugas 5: Menerbitkan tindakan

Selanjutnya, terbitkan tindakan untuk digunakan di Microsoft 365 Copilot.

1. Pilih **Terbitkan** di bagian atas halaman.

1. Pada halaman **Terbitkan Plugin**, pilih **Terbitkan**.

1. Pada halaman **Terbitkan konten terbaru?** , konfirmasikan bahwa plugin Info Project ABC diaktifkan dan pilih **Terbitkan**.  Mungkin butuh waktu beberapa menit.  Pemberitahuan akan ditampilkan di bagian atas jendela ketika penerbitan telah selesai.

## Tugas 6: Mengaktifkan dan menguji tindakan

Terakhir, uji tindakan di Microsoft 365 Copilot.

1. Buka **Microsoft Teams**.

1. Pilih **Obrolan** di bar samping.

1. Pilih **Copilot** di menu obrolan.

1. Pada area penulisan pesan, pilih tombol **Kelola respons Copilot**.

1. Pada menu melayang, cari **Copilot Studio** lalu pilih **Tambahkan** untuk menambahkan Copilot Studio.
 
2. Tindakan **Proyek ABC info** sekarang harus dicantumkan dalam flyout.  Konfirmasikan bahwa **Project ABC info** telah diaktifkan, lalu tutuplah flyout tersebut.

:::image type="content" source="../Media/projectABCInfo-action-enabled.png" alt-text="Cuplikan layar tindakan Info ABC Proyek yang tercantum dalam "Manage Copilot response" flyout in Teams.":::

3. Dalam kotak tulis pesan, masukkan `Who should I contact for questions about Project ABC?`

4. Perhatikan bahwa Microsoft 365 Copilot mengembalikan informasi tentang Project ABC dengan memanggil tindakan percakapan.

Anda dapat menyesuaikan atau memperluas tindakan percakapan ini dengan node tambahan.  Sebagai contoh, Anda dapat membuat node baru **Jawaban generatif**, lalu mengunggah sebuah file sehingga memperluas pengetahuan yang tersedia pada tindakan tersebut.

**Catatan:** Ingat hal-hal berikut saat menguji tindakan Anda di Copilot:
- Copilot akan selalu menulis ulang jawaban Anda dengan suaranya sendiri. Tidak dimungkinkan, dalam pratinjau ini, agar konten diteruskan tidak berubah ke pengguna akhir.
- Deskripsi tindakan percakapan Anda sangat penting untuk seberapa andal tindakan tersebut akan dipanggil. Deskripsi mengajarkan orkestrator apa yang baik dalam tindakan Anda dan jawaban apa yang dapat diberikannya. Pastikan untuk menggunakan prosa yang jelas saat menulis deskripsi, dan pertimbangkan untuk bereksperimen dengan perubahan untuk mendapatkan hasil terbaik.
- Mengikuti langkah-langkah ini secara akurat tidak menjamin bahwa Copilot akan mengembalikan hasil yang diharapkan setiap kali.  Copilot akan menentukan kapan harus memanggil plugin Anda dan cara mengembalikan hasilnya.

## (Opsional) Tantangan: Buat sendiri!

Terapkan apa yang telah Anda pelajari untuk membuat, menerbitkan, dan menguji tindakan percakapan baru untuk skenario pilihan Anda.  Tinjau langkah-langkah dalam latihan ini sesuai kebutuhan.