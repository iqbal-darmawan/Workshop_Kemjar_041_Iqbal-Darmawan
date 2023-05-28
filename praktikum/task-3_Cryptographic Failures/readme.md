<h3 align="center">
    <b>Kemanan Jaringan</b><br>
    Cryptographic Failures
</h3>
<br>
<p align="center">
  <img src="./Aspose.Words.055ad41d-12c1-487c-8350-669dabe39605.001.jpeg" alt="Size Limit CLI" width="300">
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

**A. Nested Easter Egg**

Easter Egg merupakan pesan tersembunyi yang telah disisipkan kedalam website

1. Pergi kelaman github yang ada pada bagian sidebar menu website OWASP Juice Shop.

![Screenshot](Aspose.Words.055ad41d-12c1-487c-8350-669dabe39605.002.png) ![Screenshot](Aspose.Words.055ad41d-12c1-487c-8350-669dabe39605.003.png)

1. Selanjutnya pergi ke folder /ftp/eastere.gg maka kita akan melihat kode seperti pada gambar dibawah ini yaitu "L2d1ci9xcmlmL25lci9mYi9zaGFhbC9ndXJsL3V2cS9uYS9ybmZncmUvcnR0L2p2Z3V2YS9ndXIvcm5mZ3JlL3J0dA=="

![Screenshot](Aspose.Words.055ad41d-12c1-487c-8350-669dabe39605.004.png)

1. Selanjutnya buka website [CyberChef](https://gchq.github.io/CyberChef/)

![Screenshot](Aspose.Words.055ad41d-12c1-487c-8350-669dabe39605.005.png)

1. Masukkan operasi "From Base 64" dan "ROT 13"

![Screenshot](Aspose.Words.055ad41d-12c1-487c-8350-669dabe39605.006.png)

1. Masukkan kode yang kita dapatkan dari github kedalam input maka pada bagian output kita akan mendapatkan string seperti sebuah alamat URL website

![Screenshot](Aspose.Words.055ad41d-12c1-487c-8350-669dabe39605.007.png)

1. Kita coba masukkan URL tersebut ke web OWASP Juice Shop kita, maka akan memunculkan halaman website seperti pada gambar dibawah ini

![Screenshot](Aspose.Words.055ad41d-12c1-487c-8350-669dabe39605.008.png)

**B. Weird Crypto**

Memberi tahu toko tentang algoritma atau library enkripsi yang seharusnya tidak digunakan.

1. Pada web OWASP Juice Shop, pergi kehalaman customer feedback yang berada pada sidebar menu web

![Screenshot](Aspose.Words.055ad41d-12c1-487c-8350-669dabe39605.009.png) ![Screenshot](Aspose.Words.055ad41d-12c1-487c-8350-669dabe39605.010.png)

1. Masukkan comment dengan inputan "MD5" lalu submit jawaban. Maka setelah itu akan muncul notifikasi berhasil menyelesaikan challange Weird Crypto

![Screenshot](Aspose.Words.055ad41d-12c1-487c-8350-669dabe39605.011.png) ![Screenshot](Aspose.Words.055ad41d-12c1-487c-8350-669dabe39605.012.png)

Pesan yang ingin disampaikan dari challange Weird Crypto ini adalah, kita sudah harus tau algoritma atau library enkripsi apa yang sebaiknya kita gunakan dan yang sudah harus kita tinggalkan. Salah satu contoh algoritma yang sebaiknya sudah ditinggalkan adalah MD5.

MD5 adalah versi lama dari alogaritma kriptografi, di mana kata kunci masih bisa menggunakan 4 huruf. Didesain oleh Ronald Rivest pada 1991. Lima tahun kemudian, pada 1996 ditemukan cacat dalam desainnya sehingga mulai ditinggalkan dan digantikan dengan alogaritma baru seperti SHA-1 dan SHA-2. Saat ini, di pasaran juga tersedia aplikasi untuk membuka enkripsi MD5 yang disebut "MD5 Hash Generator". Secara teori enkripsi MD5 memang kurang aman dibanding SHA2 sebab hanya memiliki panjang 128 bit.

