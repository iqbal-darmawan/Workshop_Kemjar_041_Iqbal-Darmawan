<h3 align="center">
    <b>Kemanan Jaringan</b><br>
    Security Misconfiguration
</h3>
<br>
<p align="center">
  <img src="./Aspose.Words.bc219017-9ee2-4d10-8a50-ace671e64fd2.001.png" alt="Size Limit CLI" width="300">
</p>
<br>
<p align="center">
    Dosen Pembimbing:<br>
    Ferry Astika Saputra, S.T., M.Sc.
</p>
<br>
<p align="center">
    Disusun Oleh:<br>
    Iqbal Darmawan (3122640041)
</p>
<br>
<p align="center">
    <b>
        KELAS D4 LJ IT B <br>
        JURUSAN D4 LJ TEKNIK INFORMATIKA <br>
        DEPARTEMEN TEKNIK INFORMATIKA DAN KOMPUTER <br> 
        POLITEKNIK ELEKTRONIKA NEGERI SURABAYA <br>
        2023
    </b>
</p>
<br>
<br>

1. **Error Handling** 

memunculkan error, tetapi error yang ditampilkan tidak secara bagus dan konsisten. 

1. Nyalakan Burp Suite terlebih dahulu 

![](Aspose.Words.bc219017-9ee2-4d10-8a50-ace671e64fd2.002.jpeg)

2. Selanjutnya buka browser dan pergi ke halaman utama website OWASP Juice Shop 

![](Aspose.Words.bc219017-9ee2-4d10-8a50-ace671e64fd2.003.jpeg)

3. Buka kembali Burp Suite maka akan muncul request baru yaitu /rest/product/search 

![](Aspose.Words.bc219017-9ee2-4d10-8a50-ace671e64fd2.004.jpeg)

4. Masukkan payload /rest/product/search tadi ke repeater lalu ubah enpointnya menjadi text random lalu klik tombol send 

![](Aspose.Words.bc219017-9ee2-4d10-8a50-ace671e64fd2.005.png)

maka yang terjadi adalah response error 500 atau internal server error yang disini terlihat terdapat error message yang begitu panjangnya dan tidak tertata 

2. **Deprecated Interface** 

Menggunakan antarmuka B2B usang yang tidak dimatikan dengan benar. 

1. Pada halaman utama, klik tombol menu di pojok kiri atas untuk memunculkan sidebar. Setelah itu klik complaint 

![](Aspose.Words.bc219017-9ee2-4d10-8a50-ace671e64fd2.006.jpeg)

2. Setelah sudah masuk ke halaman complaint, isikan form yang ada, dan masukkan file dengan format xml 

![](Aspose.Words.bc219017-9ee2-4d10-8a50-ace671e64fd2.007.jpeg)

3. Setelah itu akan muncul challange Deprecated Interface berhasil di selesaikan seperti ini 

![](Aspose.Words.bc219017-9ee2-4d10-8a50-ace671e64fd2.008.jpeg)

4. Jika kita lihat di proxy history pada burp suite, akan muncul error panjang seperti ini 

![](Aspose.Words.bc219017-9ee2-4d10-8a50-ace671e64fd2.009.jpeg)
