# Elektronik Prangko Indonesia

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

Paparan :
* [Prangko Digital Twin](./ppt/DigitalTwinPrangko.pdf) Beberapa Negara

## Pembuatan Standar Penerbitan Eprangko

Maka definisi prangko elektronik diantaranya :
1. Menggunakan secure paper. memiliki dua carik, carik utama dan carik lampiran. Carik utama berisi QR PGP publik key, carik lampiran berisi private key atau passphrase. Carik utama berfungsi untuk dikirimkan ke pada pengirim surel, sedangkan carik lampirang yang berisi PGP Private key di simpan oleh penerima. Carik lampiran bisa di tambahkan keamanan dengan cara di gosok untuk bisa melihat qrcode di dalamnya. 

![image](https://user-images.githubusercontent.com/11188109/229650984-cdce0f06-92fa-446d-a1c2-f3d01cd5e27c.png)

2. QR Code berisi Keyring PGP dengan masa kedaluarsa 1 tahun. Berfungsi untuk pengiriman surel terenskripsi sesuai dengan standar [RFC 2350 Gov-CSIRT Indonesia](https://www.idsirtii.or.id/halaman/tentang/rfc-2350-gov-csirt-indonesia.html)
3. [Penyelenggara Sertifikasi Elektronik PSrE](https://www.rootca.id/) bisa menyediaan key server untuk kepentingan validasi pengirim dan penerima surel.
4. eprangko bisa menjadi bea kirim. Dengan cara ditempel pada paket, surat atau kartu pos. Bisa untuk dikirimkan kepada pengirim surel sebagai keamanan tambahan verifikasi alamat pengirim(MFA : Multi Factor Authentication). QR Public Key bisa menjadi track and trace kiriman.
5. Augmented reality(AR) berfungsi untuk menambah informasi tentang prangko, platform AR menggunakan kode sumber terbuka dan infrastruktur yang di sepakati bersama dalam rangka kontribusi riset dan ilmu pengetahuan, supaya konten terus tumbuh berkembang. Sebagai contoh : Google's ARCore, AR.js, ARToolKit, DroidAR.
6. Edisi khusus prangko kripto seperti full sheet atau souvenir yang terbit minimal setahun sekali. Yang disebut sebagai prangko kripto disini adalah prangko yang berisikan koleksi NFT yang ditaruh di dalam alamat wallet(QR) yang di cetak dalam carik utama, dan private key(QR) di bagian carik lampiran.
