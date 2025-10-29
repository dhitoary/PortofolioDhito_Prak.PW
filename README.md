# Dhito Aryo Trengginas — Portofolio Praktikum Pemrograman Web

[![HTML](https://img.shields.io/badge/HTML-%3E%3D5-orange.svg)](https://developer.mozilla.org/en-US/docs/Web/HTML) [![CSS](https://img.shields.io/badge/CSS-%3E%3D3.0-green.svg)](https://developer.mozilla.org/en-US/docs/Web/CSS) [![Live Demo](https://img.shields.io/badge/Live%20Demo-Open-green.svg)](https://raw.githack.com/dhitoary/Portofolio-Dhito/main/index.html)

Selamat datang! Ini adalah portofolio tugas praktikum Pemrograman Web saya — dibuat hanya dengan HTML dan CSS. README ini menampilkan preview animasi (GIF) dan menyediakan snippet CSS kecil bila Anda ingin menambahkan animasi langsung ke halaman.

---

## Animated preview
Klik gambar untuk membuka live preview (raw.githack) — atau lihat GIF yang sudah saya siapkan sebagai contoh.

[![Hero animated preview](assets/screenshot-hero.gif)](https://raw.githack.com/dhitoary/Portofolio-Dhito/main/index.html)

![Education animated preview](assets/screenshot-education.gif) ![Contact animated preview](assets/screenshot-contact.gif)

> Catatan: letakkan file GIF di `assets/` dengan nama di atas agar gambar muncul di README.

---

## Tentang singkat
Saya Dhito Aryo Trengginas — Mahasiswa Teknik Informatika (NPM 2315061015). Tugas praktikum ini menuntut pembuatan portofolio statis menggunakan HTML & CSS. Fokus: desain yang estetis, responsif, dan mudah dikustomisasi.

- Bahasa: HTML & CSS (tanpa JavaScript)
- Fitur utama: About, Experience (timeline), Education, Skills, Contact
- Tema: Collage hijau (army/olive) — mudah diubah lewat CSS variables

---

## Cara menjalankan cepat
1. Clone repo:
   git clone https://github.com/dhitoary/Portofolio-Dhito.git  
2. Masuk folder dan buka `index.html` di browser.  
3. Untuk live preview via raw.githack:
   https://raw.githack.com/dhitoary/Portofolio-Dhito/main/index.html

---

## Cara membuat GIF/animasi preview cepat
1. Buka `index.html` di browser.
2. Atur ukuran jendela agar sesuai (mis. 1365×768).
3. Rekam area layar dengan Snipping Tool, ShareX, atau DevTools → Capture full size screenshot untuk membuat GIF (tools seperti ScreenToGif atau ShareX bisa merekam dan menyimpan sebagai GIF).
4. Simpan hasil ke `assets/screenshot-hero.gif`, `assets/screenshot-education.gif`, `assets/screenshot-contact.gif`.
5. Commit & push — README akan menampilkan GIF otomatis.

---

## Snippet animasi CSS (opsional)
Anda bisa menambahkan animasi halus ke elemen di `index.html`. Salin dan tempel ke `styles.css` Anda di bagian bawah.

```css
/* subtle float for hero profile */
@keyframes floaty {
  0% { transform: translateY(0); }
  50% { transform: translateY(-6px); }
  100% { transform: translateY(0); }
}
.profile-photo {
  animation: floaty 4s ease-in-out infinite;
  will-change: transform;
}

/* fade-in sections on load */
.fade-in {
  opacity: 0;
  transform: translateY(8px);
  animation: fadeInUp 0.8s forwards;
}
@keyframes fadeInUp {
  to { opacity: 1; transform: translateY(0); }
}

/* gentle hover for cards */
.glass:hover {
  transform: translateY(-6px);
  transition: transform 220ms ease;
  box-shadow: 0 20px 40px rgba(0,0,0,0.5);
}
```

Tambahkan class `fade-in` pada elemen section yang ingin Anda munculkan dengan transisi ketika halaman dibuka.

---

## Struktur rekomendasi (singkat)
```
Portofolio-Dhito/
├─ index.html
├─ styles.css
├─ assets/
│  ├─ profile.jpg
│  ├─ screenshot-hero.gif
│  ├─ screenshot-education.gif
│  └─ screenshot-contact.gif
└─ README.md
```

---

## Kontak
- Email: aryodhito20@gmail.com  
- GitHub: https://github.com/dhitoary  
- LinkedIn: https://www.linkedin.com/in/dhito-aryo-trengginas-1b886629

---

Terima kasih sudah melihat. Jika Anda mau, saya bisa langsung:
- Membuat dan menambahkan GIF placeholder (dummy) ke `assets/` lalu commit ke repo, atau
- Menggabungkan snippet CSS animasi langsung ke `styles.css` dan meng-commit perubahan. Saya siap melanjutkan mana yang Anda pilih.
