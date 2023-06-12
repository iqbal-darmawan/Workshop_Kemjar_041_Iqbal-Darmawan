<h3 align="center">
    <b>Kemanan Jaringan</b><br>
    Data Mining
</h3>
<br>
<p align="center">
  <img src="..\task-6_Security Misconfiguration\Aspose.Words.bc219017-9ee2-4d10-8a50-ace671e64fd2.001.png" alt="Size Limit CLI" width="300">
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

**Laporan Praktikum** 

1. Bagi File menjadi 5 bagian : init.pcap, init2.pcap, init3.pcap, init4.pcap, init5.pcap 

![](Aspose.Words.94f601b4-2bfd-4f8c-a57e-5d43c5ca9b8e.002.jpeg)

2. Kemudian buka file tersebutsecara bergantian menggunakan Wireshark. Pada langkah ini kita gunakan  

file init.pcap 

![](Aspose.Words.94f601b4-2bfd-4f8c-a57e-5d43c5ca9b8e.003.jpeg)

3. Untuk proses analisa yang akan dilakukan nantinya, kita akan mengambil data dengan ip versi 4 (ipv4) dan protocol TCP, DNS saja. Untuk proses tersebut  dapat  dilakukan pada wireshark menggunakan perintah ip.version==4 && tcp || dns pada kolom display filter tepat dibawah toolbar 

![](Aspose.Words.94f601b4-2bfd-4f8c-a57e-5d43c5ca9b8e.004.jpeg)

4. Untuk mendapatkan delta time dan delta time dan delta time display, klik Edit – Preferences – Column 

![](Aspose.Words.94f601b4-2bfd-4f8c-a57e-5d43c5ca9b8e.005.jpeg)

Hasilnya 

![](Aspose.Words.94f601b4-2bfd-4f8c-a57e-5d43c5ca9b8e.006.jpeg)

5. Export file pcap tersebut keformat Comma-separated Value (.csv) dengan cara klik File – Export Packet Dissections – As CSV. Yang perlu diperhatikan yaitu pada Pacet Range, pastikan yang terpilih yaitu Displayed, karena data pada Displayed ini sudah terfilter denga nip version 4 

![](Aspose.Words.94f601b4-2bfd-4f8c-a57e-5d43c5ca9b8e.007.jpeg)

![](Aspose.Words.94f601b4-2bfd-4f8c-a57e-5d43c5ca9b8e.008.jpeg)

5. membuat workflow/project  baru. Dengan cara klik File – New – New Knime Workflow – Tulis Nama workflow dan Lokasi workflow tersebut – Klik Finish 

![](Aspose.Words.94f601b4-2bfd-4f8c-a57e-5d43c5ca9b8e.009.jpeg)

6. Tambahkan data kedalam file reader 

![](Aspose.Words.94f601b4-2bfd-4f8c-a57e-5d43c5ca9b8e.010.jpeg)

7. Gabungkan kelima data dengan menggunakan concatenate dan data reader seperti gambar dibawah 

![](Aspose.Words.94f601b4-2bfd-4f8c-a57e-5d43c5ca9b8e.011.jpeg)

8. Untuk melakukan labeling data normal kita akan menggunakan Node Missing Value. Node ini digunakan untuk mengisi data kosong. 

![](Aspose.Words.94f601b4-2bfd-4f8c-a57e-5d43c5ca9b8e.012.jpeg)

9. Untuk memastikan bahwa kolom label sudah terisi dengan value Malicious atau Normal, dapat menggunakan node Value Counter. Node ini berfungsi untuk menghitung jumlah seluruh value pada kolom terpilih. 

![](Aspose.Words.94f601b4-2bfd-4f8c-a57e-5d43c5ca9b8e.013.jpeg)

10. Export file ke dalam format .csv dengan menggunakan node CSV Writer 

![](Aspose.Words.94f601b4-2bfd-4f8c-a57e-5d43c5ca9b8e.014.jpeg)

Saya menaruh data didalam file hasil.csv 

![](Aspose.Words.94f601b4-2bfd-4f8c-a57e-5d43c5ca9b8e.015.jpeg)

11. Data Pre Processing 

Proses dimana data akan dibersihkan (cleaning) karena biasanya didalam suatu data terdapat nilai-nilai yang tidak sempurna atau bahkan terdapat nilai-nilai yang hilang atau kosong yang nantinya akan dapat mempengaruhi proses kedepannya. Pada proses ini kita membutuhkan Node-node berikut : File Reader, Column Filter, Missing Value.

![](Aspose.Words.94f601b4-2bfd-4f8c-a57e-5d43c5ca9b8e.016.jpeg)

12. Proses data transformation, pada proses ini data akan diubah ke format yang sesuai untuk proses  data  mining.  Node  yang  digunakan  pada  tahap  ini  yaitu  Normalizer.  Berikut konfigurasinya 

![](Aspose.Words.94f601b4-2bfd-4f8c-a57e-5d43c5ca9b8e.017.jpeg)

13. Data Mining  

Setelah menyelesaikan tahap data transformation, kita akan menjalankan proses Data Mining, dalam proses ini kita akan menggunakan Metode Klasifikasi Decision Tree dengan teknik Cross  Validation.  Pada  proses  ini  kita  membutuhkan  Node-node  berikut  :  X-Partitioner, Decision Tree Learner, Decision Tree Predictor, X-Aggregator Sehingga akan membentuk flow seperti ini 

![](Aspose.Words.94f601b4-2bfd-4f8c-a57e-5d43c5ca9b8e.018.jpeg)

14. Node Scorer yang didalamnya terdapat perhitungan untuk melihat seberapa baik model ini dengan menggunakan teknik confusion matrix. Berikut konfigurasinya. 

![](Aspose.Words.94f601b4-2bfd-4f8c-a57e-5d43c5ca9b8e.019.jpeg)

15. Hasil  Prediksi 

![](Aspose.Words.94f601b4-2bfd-4f8c-a57e-5d43c5ca9b8e.020.jpeg)
