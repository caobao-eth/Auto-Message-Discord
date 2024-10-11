# Penjelasan :
send_message: Mengirim pesan menggunakan API Discord, kemudian mengembalikan ID pesan yang dikirim agar bisa dihapus nantinya.
delete_message: Menghapus pesan menggunakan API Discord berdasarkan ID pesan yang diterima dari fungsi send_message.

Alur Pengiriman dan Penghapusan:
Kirim pesan dari file messages.txt.
Tunggu selama 60 detik.
Hapus pesan yang sudah dikirim.
Tunggu lagi selama 30 detik sebelum mengirim pesan berikutnya.
Ulangi hingga semua pesan di file habis, lalu ulangi dari pesan pertama.

# Cara Kerja:
Pesan dikirim dari file messages.txt, satu per satu.
Setelah setiap pesan dikirim, bot menunggu selama 60 detik sebelum menghapus pesan tersebut.
Setelah pesan dihapus, bot menunggu lagi selama 30 detik sebelum mengirim pesan berikutnya.
Proses ini akan terus berulang, kembali ke pesan pertama setelah semua pesan habis.
