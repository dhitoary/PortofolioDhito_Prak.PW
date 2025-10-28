# Portofolio — Dhito Aryo Trengginas

[![HTML](https://img.shields.io/badge/HTML-%3E%3D5-orange.svg)](https://developer.mozilla.org/en-US/docs/Web/HTML) [![CSS](https://img.shields.io/badge/CSS-%3E%3D3.0-green.svg)](https://developer.mozilla.org/en-US/docs/Web/CSS) [![License: MIT](https://img.shields.io/badge/License-MIT-lightgrey.svg)](LICENSE)

Ringkasan cepat: ini adalah portofolio statik yang saya buat menggunakan hanya HTML & CSS — desain modern dengan glassmorphism dan tema "army / olive" sebagai opsi warna utama. Struktur proyek sederhana sehingga mudah untuk dikembangkan, dipersonalisasi, dan di-host (mis. GitHub Pages).

Contents
- Demo & Screenshot
- Fitur
- Struktur Proyek
- Cara Menjalankan (lokal)
- Kustomisasi Cepat (foto, teks, tema warna)
- Tips Deploy ke GitHub Pages
- Kontribusi & Lisensi

---

Demo & Screenshot
- Live demo: https://dhitoary.github.io/Portofolio-Dhito (ganti sesuai repo dan branch jika sudah deploy)
- Screenshot: `assets/screenshot.png` (letakkan screenshot UI di folder `assets`)

Fitur
- Desain modern, responsif (Grid + Flexbox).
- Glassmorphism cards, transisi halus.
- Tema default: collage hijau (army/olive) — mudah diubah lewat CSS variables.
- Semua konten statis: hanya HTML & CSS (form tampilan non-fungsional).
- Section lengkap: About, Experience (timeline), Education, Skills, Contact.

Struktur Proyek (contoh)
```
Portofolio-Dhito/
├─ index.html
├─ styles.css
├─ assets/
│  ├─ profile.jpg
│  ├─ screenshot.png
│  └─ background.jpg (opsional)
└─ README.md
```

Cara Menjalankan (lokal)
1. Clone repository:
   git clone https://github.com/dhitoary/Portofolio-Dhito.git
2. Masuk folder:
   cd Portofolio-Dhito
3. Buka `index.html` di browser (double-click atau `open index.html` / `xdg-open index.html`).
   - Tidak perlu server karena hanya HTML/CSS. Untuk preview yang lebih mirip hosting: jalankan `npx http-server` atau `python -m http.server 8000`.

Kustomisasi Cepat
- Ganti foto profil:
  - Letakkan foto Anda di `assets/profile.jpg` dan pastikan file name cocok atau ubah path di `index.html`.
- Edit isi teks:
  - Semua teks berada di dalam `index.html`. Cari bagian "Tentang Saya", "Experience", "Education", dan ganti sesuai CV Anda.
- Ubah warna tema (collage hijau → variasi lain):
  - Buka `styles.css`, temukan :root dan ubah variabel:
    - --olive-1, --olive-2, --khaki, --sand, --bg-dark, dsb.
  - Contoh:
    ```
    :root {
      --olive-1: #6b7a45;
      --olive-2: #43502a;
      --khaki: #cfc79a;
      --bg-dark: #0e140e;
    }
    ```
  - Simpan dan refresh browser.

Header & Background Konsistensi
- Jika header menutup konten ketika sticky, cek `:root` atau `body { padding-top: ... }` di `styles.css` — sudah ditangani di repo ini dengan variabel `--header-h`. Ubah sesuai tinggi header Anda.
- Jika background terlihat patchy (radial overlays), buka `styles.css` dan ubah atau hapus layer radial-gradient supaya latar jadi seragam.

Menambahkan Foto / Screenshot untuk README
- Tempatkan screenshot di `assets/screenshot.png`, lalu tambahkan di README:
  ```md
  ![Tampilan Portofolio](assets/screenshot.png)
  ```

Deploy ke GitHub Pages (singkat)
1. Push semua file ke repository GitHub Anda.
2. Buka Settings → Pages → pilih branch `main` (atau `gh-pages`) → save.
3. Tunggu beberapa menit, akses: `https://<username>.github.io/<repo-name>/`

Kontribusi
- Fork repo → buat branch feature → PR.  
- Untuk request kecil (mis. typo, update data) cukup buat PR langsung ke `main` dengan deskripsi singkat.

License
- Project ini memakai lisensi MIT. Sesuaikan jika ingin lisensi berbeda.

---

Saya sudah menyiapkan README yang ringkas namun informatif, menampilkan cara menjalankan, menyesuaikan, dan men‑deploy portofolio Anda. Selanjutnya saya akan menambahkan contoh screenshot dan snippet konfigurasi GitHub Pages jika Anda mau; saya juga bisa langsung menggabungkan README ini ke repo Anda dan membuat PR atau commit (sebutkan nama branch target) — saya sudah siap untuk melanjutkan langkah itu.
