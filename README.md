# Panduan Kontribusi Pengumpulan Tugas

Terima kasih telah mengumpulkan tugas! Mohon ikuti langkah-langkah di bawah ini dengan teliti untuk menambahkan data ke dalam daftar.

## Alur Kerja Pengumpulan Tugas

Pastikan sudah memiliki akun GitHub.

---

### 1. Fork Repositori

Klik tombol **Fork** di pojok kanan atas halaman repositori ini untuk membuat salinan repositori di akun GitHub.

---

### 2. Clone Repositori Hasil Fork

Masuk ke halaman repositori **hasil fork** milik Anda.  
Klik tombol hijau **Code**, salin URL-nya, lalu jalankan perintah berikut di terminal:

```bash
git clone https://github.com/Aglalrizal/pengumpulan-tugas-promnet.git
```

---

### 3. Buat Branch Baru

Pindah ke direktori proyek dan buat branch baru khusus untuk tugas Anda.  
**Jangan lakukan perubahan langsung di branch `master`!**

```bash
# Pindah ke direktori proyek
cd NAMA_REPO_HASIL_FORK

# Buat dan langsung pindah ke branch baru
# Contoh nama branch: add-dzaky-syauqi
git checkout -b add-nama-kalian
```

---

### 4. Tambahkan Data Anda

- Buka file `index.html` dengan teks editor.
- Cari bagian komentar yang sudah disediakan.
- Tambahkan data Anda **di bawah komentar tersebut** menggunakan template `<tr>...</tr>`.

⚠️ **Ingat:**

- Tambahkan **hanya satu blok `<tr>`** untuk data Anda.
- Jangan mengubah atau menghapus data mahasiswa lain.

---

### 5. Commit & Push

Simpan perubahan, lalu jalankan perintah berikut:

```bash
# Tambahkan perubahan ke staging area
git add index.html

# Buat commit dengan pesan yang jelas
git commit -m "feat: menambahkan Nama Lengkap Anda ke daftar tugas"

# Push branch Anda ke repositori fork
git push origin nama-branch-anda
```

---

### 6. Buat Pull Request

- Masuk ke halaman repositori **hasil fork** Anda di GitHub.
- Akan muncul notifikasi untuk membuat **Pull Request**. Klik tombol **Compare & pull request**.
- Pastikan:
  - **base repository** → repositori asli
  - **head repository** → repositori hasil fork
- Beri judul Pull Request yang jelas, contoh:
  ```
  Pengumpulan Tugas - Nama Lengkap
  ```
- Klik **Create pull request**.

✅ Tugas dianggap terkumpul setelah Pull Request di-_merge_ oleh dosen/asisten.
