<h3 align=“center”>
<b>Praktikum Kemanan Jaringan</b><br>
Broken Access Control (OWASP 10 Juice Shop)
</h3>
<br>
<p align=“center”>
<img src="./Aspose.Words.6b1f4fe7-3b13-422c-a571-c9955d0372ba.001.jpeg" alt=“Size Limit CLI” width=“300”>
</p>
<br>
<p align=“center”>
Dosen Pembimbing:<br>
Ferry Astika Saputra, S.T., M.Sc.
</p>
<br>
<p align=“center”>
Disusun Oleh:<br>
Iqbal Darmawan (3122640041)
</p>
<br>
<p align=“center”>
<b>
KELAS D4 LJ IT B <br>
JURUSAN D4 LJ TEKNIK INFORMATIKA <br>
DEPARTEMEN TEKNIK INFORMATIKA DAN KOMPUTER <br>
POLITEKNIK ELEKTRONIKA NEGERI SURABAYA <br>
2023
</b>
</p>
<br>

1. Five-Star Feedback

Merubah data customer feedback melalui admin.

1. Login sebagai admin terlebih dahulu
1. Masuk ke laman /administration

![](Aspose.Words.6b1f4fe7-3b13-422c-a571-c9955d0372ba.002.png)

1. Hapus customer feedback dengan bintang 5

![](Aspose.Words.6b1f4fe7-3b13-422c-a571-c9955d0372ba.003.jpeg)

1. Forged Feedback

Merubah data nilai feed back produk dengan nilai custom

1. Pertama memasukkan feedback baru

![](Aspose.Words.6b1f4fe7-3b13-422c-a571-c9955d0372ba.004.jpeg)

1. Lalu buka aplikasi burp suite dan nyalakan intercept on ketika akan melakukan submit forged feedback dan ubah data userid dengan userid lainnya

![](Aspose.Words.6b1f4fe7-3b13-422c-a571-c9955d0372ba.005.jpeg)

![](Aspose.Words.6b1f4fe7-3b13-422c-a571-c9955d0372ba.006.jpeg)

1. Forged Review

Forged review ini akan melakukan manipulasi data review produk.

1. Pertama login terlebih dahulu
1. Lalu tambahkan review pada produk

![](Aspose.Words.6b1f4fe7-3b13-422c-a571-c9955d0372ba.007.jpeg)

1. Buka burp suite lalu check endpoint terakhir pada HTTP History dengan method PUT dan kirim ke repeater dan ubah datanya dan kirimkan lagi bodynya melalui burpsuite

![](Aspose.Words.6b1f4fe7-3b13-422c-a571-c9955d0372ba.008.jpeg)

![](Aspose.Words.6b1f4fe7-3b13-422c-a571-c9955d0372ba.009.jpeg)

1. Manipulate Basket

Pada proses ini akan memanipulasi data keranjang

1. Lakukan register akun baru
1. Jika sudah login akun baru tambahkan produk ke keranjang

![](Aspose.Words.6b1f4fe7-3b13-422c-a571-c9955d0372ba.010.jpeg)

1. Buka burp suite dan check endpoint terakhir untuk mengupdate keranjang lalu kirim ke repeater

![](Aspose.Words.6b1f4fe7-3b13-422c-a571-c9955d0372ba.011.jpeg)

1. Ubah basketid nya agar produk masuk ke keranjang user lain

![](Aspose.Words.6b1f4fe7-3b13-422c-a571-c9955d0372ba.012.jpeg)![](Aspose.Words.6b1f4fe7-3b13-422c-a571-c9955d0372ba.013.jpeg)
