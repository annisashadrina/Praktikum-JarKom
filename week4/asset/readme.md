1. UDP
![Gambar 1](Screenshot%202026-04-14%20191740.png)

2. Port 53, tujuan dan balasan sama yaitu 53.
![Gambar 2](Screenshot%202026-04-14%20191757.png)

3. Alamat IP tujuan adalah fe80::1 (ipv6), IP DNS lokal juga sama yaitu fe80::1
![Gambar 3](Screenshot%202026-04-14%20191807.png)

4. Type pesannya adalah AAAA. Pesan permintaan tidak mengandung answer.
![Gambar 4](Screenshot%202026-04-14%20191816.png)

5. Terdapat 2 jawaban. Keduanya memberikan alamat IPv6 untuk www.ietf.org:
   - `2606:4700:6810:2c63`
   - `2606:4700:6810:2d63`

6. Sesuai, paket TCP dengan flag SYN yang dikirim oleh host menunjukkan destination ke alamat IP 2606:4700::6810:2c63.
![Gambar 5](Screenshot%202026-04-14%20191823.png)

7. Tidak perlu, setelah host berhasil mendapatkan alamat IP dari proses permintaan DNS yang pertama kali, alamat IP tersebut disimpan dalam memori cache DNS lokal komputer. Saat browser memuat gambar lagi dari domain web yang sama, host langsung menggunakan alamat IP yang ada di cache tanpa harus mengirimkan pesan request baru.

---

1. Port 53, keduanya sama.
![Gambar 6](Screenshot%202026-04-14%20191842.png)

2. fe80::1. Ya, alamat ini adalah default alamat IP server DNS lokal saya.
![Gambar 7](Screenshot%202026-04-14%20191919.png)

3. Jenis dari pesan query adalah AAAA (meminta IPv6). Tidak mengandung jawaban/answers.
![Gambar 8](Screenshot%202026-04-14%20191931.png)

4. Ada 4.
   - Sebuah nama alias yang mengarah ke `www.mit.edu.edgekey.net`
   - Sebuah nama alias yang mengarah ke `e9566.dscb.akamaiedge.net`
   - Sebuah alamat IPv6 (Type AAAA) dari server tujuan akhir tersebut, yaitu `2600:1417:6000:1be::255e`
   - Sebuah alamat IPv6 alternatif (Type AAAA) dari server tujuan akhir tersebut, yaitu `2600:1417:6000:1a3::255e`
![Gambar 9](Screenshot%202026-04-14%20191943.png)
