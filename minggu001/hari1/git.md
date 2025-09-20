Konfigurasi Awal :
- git config --global user.name "Nama Anda" <-- menyetel nama pengguna global untuk identifikasi commit.
- git config --global user.email "email@example.com" <-- menyetel email pengguna global untuk identifikasi commit.
- git config --list <-- menampilkan semua konfigurasi Git yang telah disetel.

Inisialisasi dan Kloning :
- git init <-- untuk menginisialisasi
- git clone alamaturl.com <-- untuk mengclone repo di github

Perubahan :
- git add <file> <-- untuk menambah nama 1 file
- git add . <-- untuk menambah seluruh file yang baru ditambahkan
- git commit -m "Pesan peubahan" <-- mengirimkan pesan perubahan
- git reset <file> <-- untuk menggagalkan commit pada 1 file
- git reset --hard <-- menggagalkan semua commit sebelumnya

Pengecekan :
- git status <-- melihat status file yg akan di commit
- git diff <-- melihat letak perubahan jika ada perubahan dibeberapa file dimana
- git show <-- menampilkan perubahan dari commit tertentu
- git log <-- menampilkan riwayat commit

Singkronisasi
- git push
- git pull
- git fetch
- git push

Branch
- git branch
- git checkout
- git merge
- git tag.