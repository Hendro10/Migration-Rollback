# Migration-Rollback
Menggunakan Firmwork Laravel
Copy paste file: 'create_users_table.php', 'create_password_resets_table.php', 'failed_jobs_table.php', 'create_personal_access_tokens_table.php' ke folder "universitas"=>"database"=>"migrations".
Jalankan Apache dan MySQL dari xampp.
Buat database dengan nama: 'universitas'.
Buka CMD kemudian alihkan ke cd C:\xampp\htdocs\universitas, jalankan perintah: "php artisan migrate"
Untuk menghapus isi tabel migrations dan juga semua tabel yang ada jalankan perintah: "php artisan migrate:reset"
Untuk mengembalikan semua tabel yang terhapus atau membuat ulang semua tabel jalankan perintah: "php artisan migrate:fresh"
Untuk melihat daftar urutan migration, bisa dari perintah: "php artisan migrate:status"
Jika ingin mengembalikan posisi sebelum file migration terakhir, bisa menggunakan perintah berikut: php artisan migrate:rollback --step=1
Jalankan kembali perintah: php artisan migrate:status
Untuk menjalankan file migration yang terhapus jalankan perintah: php artisan migrate
Terima kasih.
