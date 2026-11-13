\# Contributing Guide



Dokumen ini berisi standar penggunaan Git yang wajib diikuti oleh seluruh anggota kelompok selama pengembangan proyek. Tujuannya adalah menjaga konsistensi kode, riwayat perubahan, dan kolaborasi antaranggota.



\## 1. Branch Convention



Format penamaan branch:



`<type>/<short-description>`



| Type | Kegunaan | Contoh |

|---|---|---|

| `feature/` | Menambahkan fitur baru | `feature/123-user-login` |

| `fix/` | Memperbaiki bug | `fix/cart-total` |

| `hotfix/` | Perbaikan darurat | `hotfix/payment-down` |

| `refactor/` | Merapikan kode | `refactor/order-service` |

| `docs/` | Mengubah dokumentasi | `docs/api-reference` |

| `test/` | Menambahkan pengujian | `test/checkout-flow` |

| `chore/` | Pemeliharaan proyek | `chore/update-deps` |



\*\*Aturan penamaan:\*\*

\- Menggunakan huruf kecil.

\- Menggunakan tanda hubung (`-`), bukan spasi.

\- Menyertakan nomor tiket jika tersedia.

\- Maksimal 50 karakter.



\## 2. Commit Convention



Format commit:



`<type>(<scope>): <subject>`



\*\*Jenis commit:\*\*



`feat`, `fix`, `docs`, `style`, `refactor`, `perf`, `test`, `build`, `ci`, `chore`, dan `revert`.



\*\*Contoh commit yang benar:\*\*



\- `feat(auth): add user login`

\- `fix(cart): correct total calculation`

\- `docs(readme): update installation steps`



\*\*Contoh commit yang salah:\*\*



\- `update`

\- `wip`

\- `fix bug`

\- `asdf`



\*\*Aturan commit:\*\*

\- Subject menggunakan huruf kecil.

\- Menggunakan kalimat perintah (imperative mood).

\- Tidak diakhiri tanda titik.

\- Maksimal 50 karakter untuk subject.

\- Body dipisahkan dengan satu baris kosong.

\- Gunakan referensi issue jika ada, misalnya `Closes #123`.



\## 3. Pull Request



Setiap perubahan kode harus diajukan melalui Pull Request (PR).



\*\*Aturan PR:\*\*

\- Judul PR mengikuti format commit message.

\- Ukuran PR diusahakan kurang dari 400 baris perubahan.

\- Minimal satu reviewer memberikan persetujuan.

\- Semua pemeriksaan CI wajib berhasil.

\- Penggabungan menggunakan metode Squash and Merge.



\## 4. Code Review



Setiap anggota wajib melakukan pemeriksaan kode sebelum perubahan digabungkan.



Label komentar yang digunakan:



\- `blocking:` Perubahan wajib diperbaiki sebelum merge.

\- `nit:` Saran kecil yang bersifat opsional.

\- `question:` Pertanyaan atau permintaan klarifikasi.

\- `praise:` Apresiasi terhadap bagian kode yang baik.



\## 5. Workflow Git



1\. Pindah ke branch utama dan ambil perubahan terbaru:

&#x20;  `git checkout main \&\& git pull origin main`

2\. Buat branch baru:

&#x20;  `git checkout -b feature/nama-fitur`

3\. Kerjakan perubahan dan buat commit secara bertahap.

4\. Push branch ke GitHub:

&#x20;  `git push -u origin feature/nama-fitur`

5\. Buat Pull Request melalui GitHub.

6\. Tunggu proses review dan pemeriksaan CI.

7\. Lakukan Squash and Merge setelah disetujui.

8\. Hapus branch yang sudah selesai digunakan.



\## 6. Hal yang Dilarang



\- Melakukan push langsung ke branch `main`.

\- Menggunakan commit message yang tidak jelas seperti `wip`, `test`, atau `asdf`.

\- Mengunggah file `.env`, folder `node\_modules/`, atau informasi rahasia seperti credentials.

\- Melakukan rebase pada branch yang sudah di-push dan sedang digunakan anggota lain.



\## 7. Teknologi Proyek



Proyek ini dikembangkan menggunakan teknologi yang disepakati oleh kelompok. Teknologi yang digunakan perlu dicantumkan dan diperbarui sesuai kebutuhan proyek.



Contoh:

\- Bahasa pemrograman: sesuaikan dengan proyek.

\- Framework: sesuaikan dengan proyek.

\- Database: sesuaikan dengan proyek.

\- Version Control: Git dan GitHub.



Seluruh anggota kelompok wajib mengikuti panduan ini agar proses pengembangan berjalan konsisten dan terorganisasi.

