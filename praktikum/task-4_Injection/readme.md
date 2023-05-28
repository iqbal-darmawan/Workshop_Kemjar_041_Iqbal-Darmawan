<h3 align="center">
    <b>Kemanan Jaringan</b><br>
    Injection
</h3>
<br>
<p align="center">
  <img src="./Aspose.Words.3a39c0a1-5640-4293-bb0c-3d1433ab8bb4.001.jpeg" alt="Size Limit CLI" width="300">
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

**A. Bender Login**

Bender login adalah login menggunakan akun email <bender@juice-sh.op> menggunakan injection

1. Masuk kehalaman login dengan melakukan klik account pada bagian navbar lalu klik login

![Screenshot](Aspose.Words.3a39c0a1-5640-4293-bb0c-3d1433ab8bb4.002.png)

1. Selanjutnya pada halaman login ini masukkan email <bender@juice-sh.op> dan dengan password diisi dengan inputan acak. Untuk melakukan injection tambahkan ' -- yang dimana maksud dari inputan tersebut adalah digunakan untuk menonaktifkan argumen query sql setelahnya atau melakukan comment jadi kita dapat menonaktifkan kondisi pengecekan passwordnya

![Screenshot](Aspose.Words.3a39c0a1-5640-4293-bb0c-3d1433ab8bb4.003.png)

1. Submit login form, maka kita akan berhasil masuk sebagai user bender

![Screenshot](Aspose.Words.3a39c0a1-5640-4293-bb0c-3d1433ab8bb4.004.png) ![Screenshot](Aspose.Words.3a39c0a1-5640-4293-bb0c-3d1433ab8bb4.005.png)

**B. Jim Login**

Sama seperti Bender login, Jim Login adalah login menggunakan akun email <jim@juice-sh.op> menggunakan injection

1. Pada web OWASP Juice Shop, pergi kehalaman customer feedback yang berada pada sidebar menu web

![Screenshot](Aspose.Words.3a39c0a1-5640-4293-bb0c-3d1433ab8bb4.002.png)

1. Selanjutnya pada halaman login ini masukkan email <jim@juice-sh.op> dan dengan password diisi dengan inputan acak. Untuk melakukan injection tambahkan ' OR '1'='1 yang dimana maksud dari inputan tersebut adalah digunakan untuk menambahkan kondisi jika 1=1 maka kondisi return pasti sama dengan true, maka login akan berhasil dilakukan

![Screenshot](Aspose.Words.3a39c0a1-5640-4293-bb0c-3d1433ab8bb4.006.png)

1. Submit login form, maka kita akan berhasil masuk sebagai user jim ![Screenshot](Aspose.Words.3a39c0a1-5640-4293-bb0c-3d1433ab8bb4.007.png)

