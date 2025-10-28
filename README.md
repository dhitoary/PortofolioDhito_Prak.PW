# Portofolio — Dhito Aryo Trengginas

[![HTML](https://img.shields.io/badge/HTML-%3E%3D5-orange.svg)](https://developer.mozilla.org/en-US/docs/Web/HTML) [![CSS](https://img.shields.io/badge/CSS-%3E%3D3.0-green.svg)](https://developer.mozilla.org/en-US/docs/Web/CSS) [![License: MIT](https://img.shields.io/badge/License-MIT-lightgrey.svg)](LICENSE)

Ringkasan cepat: ini adalah portofolio statik yang dibuat hanya dengan HTML & CSS. Desain modern menggunakan glassmorphism dan tema "army / olive". README ini menampilkan tangkapan layar (screenshot) hasil render halaman agar mudah ditunjukkan pada tugas/praktikum.

Contents
- Demo & Screenshot
- Fitur
- Struktur Proyek
- Cara Menjalankan (lokal)
- Menambahkan Screenshot ke README (cara cepat)
- Tips Deploy ke GitHub Pages
- Kontribusi & Lisensi

---

Demo & Screenshot
- Live demo (opsional): https://dhitoary.github.io/Portofolio-Dhito (ganti sesuai repositori Anda)
- Letakkan screenshot hasil render UI ke folder `assets/` dengan nama:
  - `assets/screenshot-hero.png`  (tampilan header + hero/profile)
  - `assets/screenshot-education.png` (tampilan bagian Education & Skills)
  - `assets/screenshot-contact.png` (tampilan bagian Contact / form)
- Contoh cara menyisipkan screenshot di README (sudah disertakan di bawah).

Gallery (screenshot hasil render)
![Hero view — profil & tentang saya](assets/screenshot-hero.png)
*Gambar 1 — Hero / bagian profil dan ringkasan.*

![Education & Skills](assets/screenshot-education.png)
*Gambar 2 — Bagian Education dan Skills.*

![Contact](assets/screenshot-contact.png)
*Gambar 3 — Bagian Kontak dan form (non-fungsional).*

Jika Anda ingin menampilkan gambar dengan ukuran atau gaya tertentu, gunakan HTML di README seperti ini:
```html
<div>
  <img src="assets/screenshot-hero.png" alt="Hero view" width="900">
</div>
```

Fitur
- Desain modern dan responsif (Grid + Flexbox).
- Glassmorphism cards, kontras dan tipografi yang rapi.
- Tema default: collage hijau (army/olive). Mudah diubah melalui CSS variables di `styles.css`.
- Hanya HTML & CSS — form pada halaman hanya tampilan (non-fungsional).
- Bagian lengkap: About, Experience (timeline), Education, Skills, Contact.

Struktur Proyek (contoh)
```
Portofolio-Dhito/
├─ index.html
├─ styles.css
├─ assets/
│  ├─ profile.jpg
│  ├─ screenshot-hero.png
│  ├─ screenshot-education.png
│  └─ screenshot-contact.png
└─ README.md
```

Cara Menjalankan (lokal)
1. Clone repository:
   git clone https://github.com/dhitoary/Portofolio-Dhito.git
2. Masuk folder:
   cd Portofolio-Dhito
3. Buka `index.html` di browser (double-click atau `open index.html` / `xdg-open index.html`).
   - Anda juga bisa menjalankan server lokal untuk preview:
     - `npx http-server` atau `python -m http.server 8000`

Menambahkan Screenshot ke README (cara cepat)
1. Buka halaman `index.html` di browser.
2. Sesuaikan ukuran viewport agar tampilannya mirip yang Anda inginkan (contoh: 1365×768).
3. Ambil screenshot (PrintScreen / Snipping Tool / DevTools → Capture).
4. Simpan file ke folder `assets/` dengan nama yang sudah dicontohkan di atas.
5. Commit & push:
   git add assets/screenshot-*.png README.md  
   git commit -m "Add screenshots to README"  
   git push

Tips Deploy ke GitHub Pages
1. Push semua file ke repository GitHub Anda.
2. Buka Settings → Pages → pilih branch `main` (atau `gh-pages`) → save.
3. Tunggu beberapa menit, akses: `https://<username>.github.io/<repo-name>/`

Kontribusi
- Fork repo → buat branch feature → PR.  
- Untuk perubahan kecil (typo, update data), buat PR langsung ke `main`.

License
- Project ini memakai lisensi MIT. Sesuaikan jika ingin lisensi berbeda.

---

Catatan singkat:
- README ini sudah disusun agar siap menampilkan screenshot hasil render UI. Letakkan tiga file gambar yang direkomendasikan ke folder `assets/` supaya gambar muncul dalam README di GitHub. Untuk saya bantu lebih lanjut, saya bisa: (a) membuat file screenshot placeholder otomatis di repo, atau (b) menggabungkan README langsung ke repositori—sebutkan opsi mana yang Anda ingin lakukan.
