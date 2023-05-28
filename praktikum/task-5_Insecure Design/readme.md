<h3 align="center">
    <b>Kemanan Jaringan</b><br>
    Insecure Design
</h3>
<br>
<p align="center">
  <img src="./Aspose.Words.45c16fce-2283-43c6-835a-c9b39e2c83b4.001.jpeg" alt="Size Limit CLI" width="300">
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

**A. Privacy Policy Inspection**

pada challange ini kita diperintahkan untuk melakukan inspeksi pada halaman privacy policy untuk mendapatkan informasi penting dari web OWASP Juice Shop ini.

1. Masuk kehalaman privacy policy dengan melakukan klik account pada bagian navbar lalu klik privacy & security dan selanjutnya kita klik privacy policy.

![Screenshot](Aspose.Words.45c16fce-2283-43c6-835a-c9b39e2c83b4.002.png)

1. Selanjutnya akan muncul halaman privacy policy seperti berikut

![Screenshot](Aspose.Words.45c16fce-2283-43c6-835a-c9b39e2c83b4.003.png)

1. Pada halaman ini ketika kita melakukan hover pada bagian alamat domain kita, muncul warna kuning dan merah seperti pada gambar ini.

![Screenshot](Aspose.Words.45c16fce-2283-43c6-835a-c9b39e2c83b4.004.png)

1. Tidak hanya itu saja ternyata, masih ada kalimat kalimat lainnya yang ketika dihover muncul warna serperti itu, berikut ini adalah list kalimatnya
   1. [http://127.0.0.1](http://127.0.0.1/)
   1. we may also
   1. instruct you
   1. to refuse all
   1. reasonably necessary
   1. responsibility
1. Kita gabungkan semua kalimat tersebut menjadi sebuah enpoint url <http://127.0.0.1:3000/We/may/also/instruct/you/to/refuse/all/reasonably/necessary/responsibility> dan akan muncul halaman website seperti gambar berikut

![Screenshot](Aspose.Words.45c16fce-2283-43c6-835a-c9b39e2c83b4.005.png)

dari halaman ini kita dapat melihat informasi penting seperti framework yang digunakan beserta dengan versi nya, kita juga dapat melihat directory structure nya juga. Oleh karena itu challange ini termasuk Insecure Design karena melanggar "CWE-209 Generation of Error Message Containing Sensitive Information"

