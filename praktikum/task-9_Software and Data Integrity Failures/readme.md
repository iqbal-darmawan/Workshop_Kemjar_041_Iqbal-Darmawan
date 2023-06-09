<h3 align="center">
    <b>Kemanan Jaringan</b><br>
    Software and Data Integrity Failures
</h3>
<br>
<p align="center">
  <img src="./Aspose.Words.6d1d5ac3-0cfd-44b5-8758-1c6198b4bb74.001.png" alt="Size Limit CLI" width="300">
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

**Software and Data Integrity Failures** 

**Deskripsi** 

Software and data integrity failures dan data terkait dengan kode dan infrastruktur yang tidak melindungi  dari  pelanggaran  integritas.  Contohnya  adalah  saat  aplikasi  bergantung  pada plugin, pustaka, atau modul dari sumber, repositori, dan jaringan pengiriman konten (CDN) yang tidak tepercaya. Pipeline CI/CD yang tidak aman dapat menimbulkan potensi akses tidak sah, kode berbahaya, atau penyusupan sistem. Terakhir, banyak aplikasi sekarang menyertakan fungsionalitas pembaruan otomatis, di mana pembaruan diunduh tanpa verifikasi integritas yang  memadai  dan  diterapkan  ke  aplikasi  tepercaya  sebelumnya.  Penyerang  berpotensi mengunggah  pembaruan  mereka  sendiri  untuk  didistribusikan  dan  dijalankan  di  semua instalasi. Contoh lain adalah di mana objek atau data dikodekan atau diserialkan ke dalam struktur yang dapat dilihat dan dimodifikasi oleh penyerang yang rentan terhadap deserialisasi yang tidak aman. 

Gagalnya  Menjaga  Integritas  Data  dan  Perangkat  Lunak  disebabkan  oleh  kode  dan infrastruktur  yang  tidak  mencegah  terjadinya  pelanggaran  integritas.  Contohnya  sebuah objek/data  yang  telah  di  enkoding/diserialisasi  di  dalam  struktur  yang  dapat  dilihat  dan dimodifikasi oleh penyerang yang rentan terhadap deserialisasi yang tidak aman. 

**Percobaan** 

Pada percobaan ini akan menunjukan mengunduh kode tanpa pemeriksaan integritas. 

1. **Buka Aplikasi Juice Shop.** 

![](Aspose.Words.6d1d5ac3-0cfd-44b5-8758-1c6198b4bb74.003.jpeg)

2. **Tambahkan /ftp pada link juiceshop.** 

![](Aspose.Words.6d1d5ac3-0cfd-44b5-8758-1c6198b4bb74.004.jpeg)

3. **Klik package.json.bak** 

![](Aspose.Words.6d1d5ac3-0cfd-44b5-8758-1c6198b4bb74.005.jpeg)

4. **Buka Burpsuite kemudian Menu Decoder, masukkan %00** 

![](Aspose.Words.6d1d5ac3-0cfd-44b5-8758-1c6198b4bb74.006.jpeg)

5. **Lakukan Encode as URL** 

![](Aspose.Words.6d1d5ac3-0cfd-44b5-8758-1c6198b4bb74.007.png) ![](Aspose.Words.6d1d5ac3-0cfd-44b5-8758-1c6198b4bb74.008.png)

6. **Copy hasil encode pada URL package.json.bak** 

![](Aspose.Words.6d1d5ac3-0cfd-44b5-8758-1c6198b4bb74.009.png)

7. **Kode telah dapat diunduh**  

![](Aspose.Words.6d1d5ac3-0cfd-44b5-8758-1c6198b4bb74.010.jpeg)

![](Aspose.Words.6d1d5ac3-0cfd-44b5-8758-1c6198b4bb74.011.jpeg)
