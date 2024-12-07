# Latihan: Membuat plugin prompt

Dalam latihan ini, Anda akan:

- Cara menulis prompt yang baik
- Cara membuat perintah di Copilot Studio
- Cara menguji prompt di penyusun prompt
- Cara menggunakan plugin prompt di Microsoft 365 Copilot

## Cara menulis prompt yang baik

Sebelumnya dalam modul ini, Anda sudah mempelajari beberapa dasar-dasar rekayasa prompt. Sumber daya yang bagus untuk mempelajari lebih lanjut tentang rekayasa prompt adalah membaca panduan rekayasa yang cepat dari tim AI Builder. Panduan rekayasa prompt dapat ditemukan [di sini](https://aka.ms/learn-ai-builder-prompting-guide).

## Elemen prompt yang baik

Panduan rekayasa prompt dari tim AI Builder memiliki serangkaian elemen hebat yang harus menjadi bagian dari permintaan Anda.

Seperti yang Anda lihat, ia memiliki elemen berikut:

- **Task**: sebuah **instruksi** yang memberitahukan kepada model Generative Pre-trained Transformer (GPT) tugas yang harus dilakukan
- **Konteks**: jelaskan **data** yang ditindaklanjuti, bersama dengan input **variabel**apa pun
- **Harapan**: sampaikan kepada GPT **tujuan** dan **harapan** atas respons tersebut
- **Output**: membantu GPT memformat **output** seperti yang Anda inginkan

![Cuplikan layar halaman bahan permintaan dari panduan rekayasa prompt AI Builder. Tugas, konteks, ekspektasi, dan output disorot sebagai bahan permintaan.](../Media/4-prompt-engineering-guide.png)

## Tugas 1: Mendesain perintah

Dalam tugas ini, Anda merancang permintaan yang membantu Anda membuat rencana pengembangan profesional berdasarkan tonggak karier.

> [!IMPORTANT]
> Saat membuat perintah, Anda tidak perlu memulai dari awal. Meskipun sangat membantu untuk mengetahui cara menulis perintah yang baik, akan sangat membantu untuk memulai dengan sesuatu yang sudah membuat Anda setengah jalan di sana.
> Ada contoh perintah yang sudah tersedia di [Galeri Solusi Contoh Adopsi Microsoft](https://aka.ms/power-prompts). Dalam latihan ini kita akan menggunakan contoh [Rencana Pengembangan Profesional Perintah](https://adoption.microsoft.com/sample-solution-gallery/sample/pnp-powerplatform-prompts-professional-development/).

Mari kita tambahkan semua bahan perintah:

- **Tugas** – Merancang rencana pengembangan profesional.
- **Konteks** – Bagi seseorang yang bertujuan untuk mencapai [tonggak] karier berikut.
- **Ekspektasi** – Rencana harus mencakup tujuan dan tujuan, sumber daya, dan alat dan garis waktu untuk aktivitas.
- **Output** – Format rencana untuk ringkas dan dapat ditindaklanjuti dan menyajikan informasi dengan cara yang mudah diikuti yang cocok untuk karyawan tingkat junior.

Bersama-sama, itu akan menjadi perintah berikut:

*Rancang rencana pengembangan profesional bagi seseorang yang bertujuan mencapai [milestones] karier berikutnya. Rencana tersebut harus mencakup sasaran dan tujuan, sumber daya, serta alat-alat dan garis waktu kegiatan. Format rencana tersebut agar ringkas dan dapat dilaksanakan serta menyajikan informasi dengan cara yang jelas, mudah dipahami, dan cocok bagi karyawan tingkat junior.*

## Tugas 2: Membuat tindakan perintah di Copilot Studio

Sekarang setelah Anda selesai menulis perintah, saatnya untuk memasukkannya di Copilot Studio.

1. Di browser web Anda, navigasikan ke [Copilot Studio](https://copilotstudio.microsoft.com) dan masuk dengan akun kerja atau sekolah Anda, jika diminta.  Pilih **lewati** untuk melewati pesan selamat datang apa pun.

    **Catatan:** Pertama kali Anda membuka Copilot Studio, tampilan yang muncul dapat berupa antarmuka obrolan untuk membuat copilot pertama Anda. Jika ini terjadi, pilih **...** menu di kanan atas (di samping tombol **Buat** ) lalu pilih **Batalkan pembuatan copilot** lalu **biarkan** untuk meninggalkan antarmuka obrolan dan menampilkan halaman beranda Copilot Studio.
1. Pilih **Pustaka** di navigasi kiri. Di sini, Anda dapat melihat daftar tindakan dan konektor yang sudah ada dan membuat yang baru.
1. Pilih **Tambahkan item** di bagian atas.  Menu mencantumkan 2 opsi untuk memperluas Copilot untuk Microsoft 365.
:::image type="content" source="../Media/extend copilot options.png" alt-text="Window mencantumkan 2 opsi untuk memperluas Copilot: membuat copilot atau membuat tindakan.":::
1. Pilih **Tindakan baru**.
1. Pada layar *Tindakan baru*, pilih **Perintah**. Ini akan membuka penyusun perintah AI Builder.
1. Pada halaman **Rincian tindakan** masukkan “Rencana Pengembangan Profesional” sebagai **nama tindakan**.
1. Masukkan **deskripsi**: “Membuat rencana pengembangan profesional yang dapat ditindaklanjuti berdasarkan pencapaian karier yang diinginkan.”
1. Pilih **Selanjutnya**.
1. Pada bagian **perintah** di halaman **Tambahkan tindakan perintah** masukkan “Rancang rencana pengembangan profesional untuk seseorang yang bertujuan mencapai [milestones] karier berikut ini. Rencana harus mencakup tujuan dan tujuan, sumber daya dan alat dan garis waktu untuk aktivitas. Format rencana untuk ringkas dan dapat ditindaklanjuti dan menyajikan informasi dengan cara yang mudah diikuti yang cocok untuk karyawan tingkat junior." sebagai **perintah**.

    > [!NOTE]
    > Perhatikan bahwa ada bilah informasi di bagian atas yang menunjukkan perintah Anda harus memiliki setidaknya satu nilai dinamis

1. Di bawah **Pengaturan perintah** di bilah samping sebelah kanan, buka bagian **Input** .
1. Pilih tombol **Tambahkan input** untuk menambahkan input.
1. Masukkan `milestones` sebagai nama input Anda.
1. Tambahkan teks berikut sebagai data sampel:

      ```text
      * Become medior in 3 years
      * Have 3 top reviews in a row
      * Become a manager in 10 years
      ```

1. Pilih **[milestones]** di bagian perintah dengan kursor Anda.
1. Pilih **Sisipkan**.
1. Pilih **tonggak pencapaian**.

      Ini akan mengubah **[tonggak pencapaian]** dalam nilai dinamis.

1. Selanjutnya, kami siap untuk menguji perintah kami!

## Tugas 3: Uji perintah di penyusun perintah

1. Pilih **Perintah uji** di bawah bagian perintah. Ini akan menguji permintaan dengan data sampel yang Anda tambahkan sebelumnya.

    > [!NOTE]
    > Tindakan ini akan mengirimkan perintah ke model AI, lalu menampilkan jawabannya di bagian respons AI. Ini memungkinkan Anda untuk melihat bagaimana LLM merespons dan melihat apakah Anda senang dengan hasilnya.

1. Saat Anda puas dengan respons AI, pilih **Simpan perintah kustom** untuk menyimpan perintah.

    Di jendela berikutnya - Anda dapat meninjau deskripsi plugin dan deskripsi input.

1. Pada halaman **Pilih parameter tindakan** ubah deskripsi input **tonggak pencapaian** menjadi:

      ```text
      The career milestones that the user wants to achieve
      ```

1. Pilih **Selanjutnya**.

1. Pilih **Terbitkan** untuk menerbitkan tindakan Anda ke Microsoft 365 Copilot.  Proses ini mungkin membutuhkan waktu beberapa menit.

## Tugas 4: Gunakan plugin perintah di Microsoft 365 Copilot

Sekarang setelah Anda membuat tindakan perintah dan mengujinya, lanjutkan ke tugas berikutnya untuk mengaksesnya di Microsoft 365 Copilot.  Mungkin perlu waktu 5 menit, atau lebih lama, agar plugin Anda muncul di Microsoft 365 Copilot.

1. Buka [Microsoft Teams](https://teams.microsoft.com).
1. Pilih tombol **Copilot** di navigasi sebelah kiri.
1. Pilih ikon **Kelola respons Copilot** di bagian bawah layar (di sebelah tempat Anda dapat mengirim pesan ke Copilot).
1. Cari **Copilot Studio** di menu flyout yang muncul dan konfirmasikan bahwa menu tersebut telah diaktifkan.  
1. Pilih **ikon karet** untuk memperluas daftar tindakan di bawah Copilot Studio.

    > [!NOTE]
    > Bisa jadi Copilot Studio tidak terlihat. Mungkin ada dua alasan untuk itu: admin Anda belum menyebarkan aplikasi terintegrasi Copilot Studio atau plugin belum diindeks - dan itu bisa berarti Anda harus menunggu sedikit lama.

2. Cari tindakan dengan nama **Paket Pengembangan Profesional** dalam daftar tindakan di bawah bagian Copilot Studio dan pilih tombol di sampingnya untuk mengaktifkannya.

    > [!NOTE]
    > Jika Anda tidak melihat Rencana Pengembangan Profesional dalam daftar plugin di bawah Copilot Studio, mungkin perlu waktu sedikit lebih lama untuk muncul. Dibutuhkan waktu sedikit lebih lama untuk muncul di Microsoft 365 Copilot.

3. Setelah mengaktifkan tindakan Rencana Pengembangan Profesional, Anda sekarang dapat menggunakannya di Copilot. **Cobalah** dengan mengirim pesan berikut ke Copilot di Teams: "Saya ingin menghasilkan Rencana Pengembangan Profesional untuk mencapai tonggak pencapaian berikut: 1 - menjadi lebih baik di pekerjaan saya sebagai pemasar dan 2 - memiliki kesempatan yang lebih baik untuk dipromosikan ke peran pemasar senior."

**Tips:** Untuk mengaktifkan mode pengembang di Copilot, masukkan `-developer on` di obrolan.  Ini memungkinkan Anda untuk mengamati kapan Copilot menggunakan plugin untuk merespons dalam obrolan.
