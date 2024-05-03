# test-pintu

#CICD ini menggunakan github action

1. Aplikasi nodejs di build dan di test menggunakan perintah node app.js, hanya untuk mengeluarkan console log supaya pada job tes berhasil

2. Aplikasi yang sudah berhasil di build dan di test maka akan di build dan di push ke container registry

3. Jika sudah berhasil maka akan dilanjutkan deploy ke kubernetes, akan tetapi karena tidak memiliki akun di azure makan step di sini akan gagal. Untuk proses deploy tetap saya buat jika sewaktu-waktu memiliki akun

4. Di kubernetes sudah dibuatkan deployment, service dan ingress sehingga nanti bisa diakses melalui public

#Image yang sudah dibuat akan ditaruh di sini https://hub.docker.com/repository/docker/ravencalamitous/test-pintu/general

