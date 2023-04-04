# Draft Prangko Elektronik Indonesia

Dasar Hukum :
* [Undang-Undang Nomor 38 Tahun 2009](./dh/UUNomor38Tahun2009.pdf)
  * Pasal 22 tentang fungsi prangko:
    * Bukti pembayaran biaya pengiriman pos
    * Alat edukasi masyarakat
    * Alat penyebarluasan informasi publik
    * Benda filateli
* [Permen kominfo No. 21 Tahun 2012](./dh/PermenkominfoNo21Tahun2012.pdf)
  * Pasal 1 Tentang Definisi Perangko adalah carik kertas
  * ![image](https://user-images.githubusercontent.com/11188109/229653892-8fcb7522-4b99-4bfc-8927-6e6bae4bd7c3.png)
* [Peraturan Pemerintah No. 71 Tahun 2019](./dh/71TAHUN2019PP.pdf)
  * Tentang penyelenggara sertifikat elektronik
* [Peraturan Bapepti Nomor 11 Tahun 2022](./dh/sk_kep_kepala_bappebti_2022_08_01_fx03j2mm_id.pdf)
  * ![image](https://user-images.githubusercontent.com/11188109/229658397-4f33cc66-0572-4999-bc50-0cde8d23ea4f.png)
  

Paparan :
* [Prangko Digital Twin](./ppt/DigitalTwinPrangko.pdf) Beberapa Negara

## Draft Standar Penerbitan Eprangko

Eprangko bisa menjadi Bukti pembayaran biaya pengiriman pos. Dengan cara menempelkan carik utama pada surat atau kartu pos. Dengan fungsi utama sebagai media keamanan pengiriman surel. Baik itu surel yang bersifat rahasia, penting atau biasa. EPrangko menjadi salah satu metode untuk meningkatkan faktor keamanan MFA (MFA : Multi Factor Authentication) pada pengiriman surel pelanggan. 
Alurnya pengiriman surel terenkripsi :

![how-pgp-encryption-works](https://user-images.githubusercontent.com/11188109/229703654-33cce3a3-425e-436b-95e2-32a6f260c173.jpg)

1. Simpan dengan baik carik pengaman.
2. Carik Utama dikirimkan kepada calon pengirim surel sebagai keamanan tambahan verifikasi alamat pengirim(MFA : Multi Factor Authentication) menggunakan jasa pengiriman surat pos atau alat komunikasi lainnya. 
3. QR Carik Utama bisa menjadi track and trace kiriman. 
4. Penerima Carik Utama menggunakan kunci tersebut untuk mengirimkan surel yang di enkripsi.
5. Surel terenkripsi diterima oleh pengirim carik utama dibuka dengan menggunakan kode dari carik pengaman.

### Kerangka Dasar Desain EPrangko

1. Menggunakan secure paper. Memiliki dua carik yang dipisahkan oleh perforasi, carik utama dan carik lampiran. Carik utama berisi QR(Quick Response) Code PGP publik key, carik lampiran berisi QR(Quick Response) Code PGP private key. Carik utama berfungsi sebagai bukti bayar biaya pengiriman pos untuk dikirimkan ke pada calon pengirim surel, sedangkan carik lampirang di simpan oleh penerima. Carik lampiran bisa di tambahkan keamanan dengan menambahkan scratch-area, sehingga untuk membaca QR dengan cara di gosok. 

![image](https://user-images.githubusercontent.com/11188109/229650984-cdce0f06-92fa-446d-a1c2-f3d01cd5e27c.png)

2. QR Code berisi Keyring PGP dengan masa kedaluarsa 1 tahun, disposable atau reuse. Berfungsi untuk pengiriman surel terenskripsi sesuai dengan standar [RFC 2350 Gov-CSIRT Indonesia](https://www.idsirtii.or.id/halaman/tentang/rfc-2350-gov-csirt-indonesia.html)
3. Bisa di kerjasamakan dengan [Penyelenggara Sertifikasi Elektronik PSrE](https://www.rootca.id/) untuk menyediaan key server untuk kepentingan validasi pengirim dan penerima surel.

### Augmented Reality

Augmented reality(AR) berfungsi untuk menambah informasi tentang prangko, platform AR menggunakan kode sumber terbuka dan infrastruktur yang di sepakati bersama dalam rangka kontribusi riset dan ilmu pengetahuan, supaya konten terus tumbuh berkembang. Sebagai contoh : Google's ARCore, AR.js, ARToolKit, DroidAR.

### Prangko NFT

Edisi khusus prangko NFT dalam format standar carik kenangan atau souvenir sheet yang terbit minimal setahun sekali. Yang disebut sebagai prangko NFT disini adalah prangko yang berisikan koleksi NFT yang di simpan dalam wallet address dicetak pada carik utama(QR). Akses wallet adress menggunakan private key atau pass phrase (QR) di bagian carik keamanan. Sehingga pemilik Carik Kenangan merupakan pemilik NFT sepenuhnya, tanpa harus melakukan klaim lagi dari sistem.
