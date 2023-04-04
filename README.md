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

* [Peraturan Pemerintah No. 71 Tahun 2019](./dh/71TAHUN2019PP.pdf)
  * Tentang penyelenggara sertifikat elektronik

## Pembuatan Standar Penerbitan Eprangko

Paparan [Prangko Digital Twin](./ppt/DigitalTwinPrangko.pdf)

Maka definisi prangko elektronik diantaranya :

1. Memiliki dua carik, carik utama dan carik lampiran. Carik utama berisi QR PGP publik key, carik lampiran berisi private key atau passphrase. Carik utama berfungsi untuk dikirimkan ke pada pengirim surel, sedangkan carik lampirang yang berisi PGP Private key di simpan oleh penerima. Carik lampiran bisa di tambahkan keamanan dengan cara di gosok untuk bisa melihat qrcode di dalamnya. 

![image](https://user-images.githubusercontent.com/11188109/229650984-cdce0f06-92fa-446d-a1c2-f3d01cd5e27c.png)

2. QR Code berisi Keyring PGP dengan masa kedaluarsa 1 tahun. Berfungsi untuk pengiriman surel terenskripsi sesuai dengan standar [RFC 2350 Gov-CSIRT Indonesia](https://www.idsirtii.or.id/halaman/tentang/rfc-2350-gov-csirt-indonesia.html)
3. [Penyelenggara Sertifikasi Elektronik PSrE](https://www.rootca.id/) bisa menyediaan key server untuk kepentingan validasi pengirim dan penerima surel.
4. eprangko bisa dikirimkan melalui pos dengan cara ditempel pada surat atau kartu pos, untuk dikirimkan kepada pengirim surel sebagai keamanan tambahan verifikasi alamat pengirim(MFA : Multi Factor Authentication).
5. Bisa ditambahkan AR untuk menambah informasi tentang prangko, platform AR menggunakan kode sumber terbuka yang di sepakati bersama dalam rangka kontribusi riset dan ilmu pengetahuan, supaya konten terus tumbuh berkembang. Sebagai contoh : Google's ARCore, AR.js, ARToolKit, DroidAR.
6. Edisi khusus prangko kripto seperti full sheet atau souvenir yang terbit minimal setahun sekali. Yang disebut sebagai prangko kripto disini adalah prangko yang berisikan koleksi NFT yang ditaruh di dalam alamat wallet(QR) yang di cetak dalam carik utama, dan private key(QR) di bagian carik lampiran.
