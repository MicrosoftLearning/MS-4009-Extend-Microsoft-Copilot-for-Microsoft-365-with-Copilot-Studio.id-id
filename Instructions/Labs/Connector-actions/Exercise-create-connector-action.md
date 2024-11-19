# Latihan: Membuat tindakan konektor

Dalam latihan ini, Anda akan:

- Membuat tindakan konektor di Copilot Studio
- Menguji tindakan konektor di Microsoft Teams
- Menyimpan dan menerbitkan tindakan konektor

## Tugas 1: Membuat tindakan konektor di Copilot Studio

Dalam tugas ini, Anda akan mengonfigurasi tindakan konektor untuk konektor MSN Cuaca.

1. Buka [Copilot Studio](https://copilotstudio.microsoft.com) dan masuk dengan akun kerja atau sekolah Anda, jika diminta. Lewati pesan selamat datang apa pun.

    **Catatan:** Pertama kali Anda membuka Copilot Studio, tampilan yang muncul dapat berupa antarmuka obrolan untuk membuat copilot pertama Anda. Jika ini terjadi, pilih **...** menu di kanan atas (di sebelah tombol **Buat**) lalu pilih **Batalkan pembuatan copilot** untuk keluar dari antarmuka obrolan dan menampilkan halaman beranda Copilot Studio.
1. Pilih **Pustaka** di navigasi kiri. Di sini, Anda dapat melihat daftar tindakan dan konektor yang sudah ada dan membuat yang baru.
1. Pilih **Tambahkan item** di bagian atas.  Menu mencantumkan 2 opsi untuk memperluas Copilot untuk Microsoft 365.
:::image type="content" source="../Media/extend copilot options.png" alt-text="Window mencantumkan 2 opsi untuk memperluas Copilot: membuat copilot atau membuat tindakan.":::
2. Pilih **Tindakan baru**.
3. Pilih **Konektor** untuk membuka wizard untuk tindakan konektor.
4. Pilih **MSN Cuaca** sebagai konektor.
5. **Tinjau ulang** deskripsi.

    > [!IMPORTANT]
    > Deskripsi ini sangat penting karena Copilot akan menggunakan ini untuk mencocokkan pesan pengguna dengan plugin Anda. Jika Anda tidak memiliki deskripsi yang baik, Copilot mungkin tidak memicu tindakan konektor Anda.

1. Pilih **Selanjutnya**.
1. Pilih tindakan **Dapatkan cuaca saat ini** .
1. **Tinjau** deskripsi tindakan.

    > [!IMPORTANT]
    > Tinjau deskripsi tindakan di layar berikut. Deskripsi tindakan ini sangat penting karena Copilot akan menggunakan ini untuk mencocokkan pesan pengguna dengan tindakan Anda. Jika Anda tidak memiliki deskripsi tindakan yang baik, Copilot mungkin memicu tindakan yang salah.

1. Pilih **Selanjutnya**.
1. **Tinjau** deskripsi semua input dan output.

    > [!IMPORTANT]
    > Tinjau deskripsi input dan output di layar berikut. Deskripsi input dan output ini sangat penting karena Copilot akan menggunakan ini untuk memicu konektor (input) dan untuk menulis respons (output) yang baik kepada Anda. Jika Anda tidak memiliki deskripsi input dan output yang baik, Copilot mungkin tidak memicu konektor dengan benar atau tidak akan mengirim kembali respons yang baik.

1. Pilih **Selanjutnya**.
1. Selanjutnya, Anda akan melihat layar tempat Anda dapat menambahkan lebih banyak tindakan jika mau, tetapi dalam hal ini kita akan melewati ini dan memilih **Berikutnya**.

## Tugas 2: Menguji tindakan konektor di Microsoft Teams

Dalam tugas ini, Anda akan menguji tindakan konektor yang Dikonfigurasi di tugas 1 di Microsoft 365 Copilot di Microsoft Teams.

![Bagian tinjau, uji, dan terbitkan tindakan Anda pada wizard tindakan konektor.](../Media/connect-test.png)

1. Pilih koneksi yang sudah ada jika Anda memilikinya, atau pilih **Koneksi baru** untuk membuat koneksi baru untuk konektor MSN Cuaca.
1. Pada menu **Koneksi baru** , pilih **Buat**.
1. Di bawah **Koneksi yang dipilih**, Anda sekarang dapat memilih koneksi baru Anda dari menu dropdown.
1. Pilih tombol **Tindakan uji**.

    > [!NOTE]
    > Ini akan memicu proses di mana tindakan konektor Anda akan disebarkan ke Microsoft Teams sehingga Anda dapat mengujinya.

1. Pilih **Uji** untuk membuka halaman Pengujian.

    > [!NOTE]
    > Ini akan membuka tab browser baru dan akan mencoba meluncurkan Microsoft Teams.

1. Jangan ragu untuk memilih **Batal** di pop-up tempat ia mencoba meluncurkan Microsoft Teams.
1. Pilih **Gunakan aplikasi web sebagai gantinya**.

    > [!NOTE]
    > Ini akan membuka Microsoft 365 Copilot di Microsoft Teams.

1. Dari area tulis pesan di Copilot di Teams, pilih ikon **plugin ** di samping ikon kirim.
1. Temukan plugin **Test-MSN Weather** dan pilih tombol untuk mengaktifkannya.

    > [!NOTE]
    > Ini akan menampilkan pesan berikut.

    ![Pesan menampilkan bahwa plugin Test-MSN Cuaca aktif.](../Media/test-msn-weather.png)


1.  Kirim pesan berikut ke Microsoft 365 Copilot, mengisi nilai untuk lokasi dan unit yang Anda inginkan.

    ```text
    What is the current weather in <your location> in <celsius/fahrenheit> according to MSN Weather?
    ```

1. Jika semua berjalan dengan baik, Copilot harus merespons dengan pesan menggunakan plugin.  

   ![Cuplikan layar yang memperlihatkan contoh pesan kesalahan. Plugin merespons dengan cuaca saat ini di Utrecht, Belanda di celsius.](../Media/msn-weather-result.png)

   **Catatan:** Copilot dapat meminta izin kepada Anda sebelum menggunakan plugin.  Pilih **Selalu izinkan** untuk mengaktifkan Copilot untuk menggunakan plugin.

   :::image type="content" source="../Media/test-msn-weather-allow.png" alt-text="Cuplikan layar Copilot meminta izin untuk menggunakan plugin.":::

## Tugas 3: Menyimpan dan menerbitkan tindakan konektor

Dalam tugas ini, Anda akan menyimpan tindakan konektor dan menerbitkannya.

Mari kita ambil di mana kita tinggalkan di Copilot Studio.

1. Pilih **Berikutnya** di wizard dan tindakan konektor akan diterbitkan.

    > [!NOTE]
    > Di layar berikutnya, Anda akan dapat masuk ke layar detail atau menyimpan dan menutup. Seperti yang ditunjukkan dalam pesan, mungkin perlu beberapa menit agar tindakan muncul dalam pengalaman salinan.

      ![Cuplikan layar terbitkan di wizard tindakan konektor.](../Media/connector-action-finished.png)
   
1. Pilih **Simpan dan Tutup**.

Anda sekarang telah mengonfigurasi dan menerbitkan tindakan konektor Anda.
