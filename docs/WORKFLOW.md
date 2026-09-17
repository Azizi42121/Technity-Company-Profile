# Workflow Project

Penjelasan mengenai bagaimana alur kerja di dalam project ini

## Prasyarat

Sebelum memulai project, pastikan kamu memiliki hal-hal ini di dalam komputermu

1. **Code Editor** (Seperti VSCode atau Sublime Text)
2. **Git** (Pastikan git telah terinstal di komputermu)
3. **Akun Github** (Untuk mengakses repository dan membuat pull request)

## Alur Kerja

1. **Klon repository**
Buat folder untuk project ini lalu jalankan perintah git ini
```
bash
    git clone https://github.com/Azizi42121/Technity-Company-Profile
```

2. **Lihat issues atau board project di repository**
Sebelum memulai mengerjakan tugas, lihat issue di repository github
```link repository: https://github.com/Azizi42121/Technity-Company-Profile```
atau lihat *Projects* di repository github

3. **Pindah ke branch dev**
Pastikan untuk berada di branch dev ketika ingin mengerjakan tugas agar branch main selalu aman
```
bash
    git checkout dev
```

4. **Buat branch baru**
Selalu buat branch baru dari branch dev sebelum mengerjakan tugas atau fitur. Gunakan format yang jelas:
- Fitur baru: `feature/nama-fitur`
- Perbaikan bug: `fix/nama-bug`

5. **Lakukan perubahan dan commit**
Simpan perubahan kode secara berkala di komputer lokal menggunakan pesan *commit* yang deskriptif dan konsisten. Dengan konvensi format commit:
- menambahkan kode: `feat: fitur/kode yang ditambah`
- memperbaiki kode: `fix: fitur/kode yang diperbaiki`
- perubahan pada dokumentasi: `docs: perubahan isi docs`

6. **Kirim perubahan (push)**
Unggah branch yang sudah dikerjakan ke repository github:
```
bash
    git push origin nama-branch
```

7. **Buat pull request (PR)**
Buka halaman Github, buat *Pull Request* dari branch kamu ke branch dev agar kodenya bisa direview terlebih dahulu sebelum digabung (merge).
```tutorial pull request (menit 1): https://www.youtube.com/watch?v=nCKdihvneS0```

8. **Git Pull**
Jika sudah di push dan ingin mengerjakan kembali. Lakukan git pull sebelum memulai kode.
```
bash
    git pull
```