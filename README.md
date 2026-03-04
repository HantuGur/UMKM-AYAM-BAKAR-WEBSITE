# 🍗 Ayam Bakar Pak Karto — Website

Website landing page untuk usaha kuliner **Ayam Bakar Pak Karto**, dibangun dengan HTML, CSS, dan JavaScript murni dalam satu file tanpa framework atau dependency eksternal.

---

## 📸 Preview

> Buka file `ayam-bakar.html` langsung di browser untuk melihat hasilnya.

---

## 🚀 Fitur

- **Hero Section** — Animasi bara api (ember particles) + glow efek arang
- **Cerita / About** — Sejarah warung & statistik
- **Menu Grid** — Kartu menu dengan harga & tombol pesan langsung ke WhatsApp
- **Cara Pesan** — Panduan 4 langkah pemesanan
- **Ulasan Pelanggan** — Testimoni dengan rating bintang
- **CTA Kontak** — Tombol WhatsApp besar di bagian bawah
- **Floating WhatsApp Button** — Tombol WA selalu terlihat di semua halaman dengan animasi pulse
- **Responsive** — Tampil baik di desktop, tablet, dan mobile
- **Aksesibilitas** — ARIA labels, semantic HTML, keyboard-navigable

---

## 🔒 Keamanan

| Fitur | Keterangan |
|---|---|
| `Content-Security-Policy` | Mencegah XSS & resource injection |
| `X-Frame-Options: SAMEORIGIN` | Mencegah clickjacking |
| `X-Content-Type-Options: nosniff` | Mencegah MIME-type sniffing |
| `rel="noopener noreferrer"` | Mencegah tab-napping pada link eksternal |
| Strict-mode JS (IIFE) | Isolasi scope, tidak ada global variable leak |
| Zero `innerHTML` dinamis | Tidak ada celah injeksi dari input user |

---

## 📁 Struktur Project

```
ayam-bakar-website/
│
├── ayam-bakar.html   # File utama (HTML + CSS + JS dalam 1 file)
└── README.md         # Dokumentasi project ini
```

---

## ⚙️ Cara Pakai

### 1. Clone repository

```bash
git clone https://github.com/username/ayam-bakar-website.git
cd ayam-bakar-website
```

### 2. Buka di browser

Cukup double-click file `ayam-bakar.html` atau buka via browser:

```bash
# Mac / Linux
open ayam-bakar.html

# Windows
start ayam-bakar.html
```

Tidak perlu install apapun. Tidak ada dependency. Langsung jalan.

---

## ✏️ Cara Kustomisasi

Buka `ayam-bakar.html` dengan text editor (VS Code, Notepad++, dll), lalu ubah bagian berikut:

### Nomor WhatsApp
Cari dan ganti semua `6281234567890` dengan nomor WA aktif kamu (format internasional, tanpa `+`):

```html
href="https://wa.me/628XXXXXXXXXX?text=..."
```

### Nama & Info Warung
Cari teks seperti `Ayam Bakar Pak Karto`, `Jl. Raya Bantul No. 88`, `10.00 – 21.00`, dll — lalu ganti sesuai data warungmu.

### Menu
Tiap kartu menu ada di dalam tag `<article class="menu-card">`. Ubah nama, deskripsi, harga, dan teks pesan WA sesuai menuму.

### Warna Tema
Ubah CSS variable di bagian `:root` untuk ganti palet warna:

```css
:root {
  --ember: #c8440a;   /* warna utama / tombol */
  --flame: #f07030;   /* aksen api */
  --gold:  #e8a830;   /* warna emas / harga */
}
```

---

## 🌐 Deploy

Website ini adalah static file, bisa di-host di mana saja:

| Platform | Cara |
|---|---|
| **GitHub Pages** | Push ke branch `main`, aktifkan GitHub Pages di Settings |
| **Netlify** | Drag & drop folder project ke [netlify.com/drop](https://app.netlify.com/drop) |
| **Vercel** | `vercel deploy` atau import dari GitHub |
| **Shared Hosting** | Upload `ayam-bakar.html` via FTP/cPanel, rename jadi `index.html` |

---

## 🛠️ Teknologi

- **HTML5** — Semantic markup
- **CSS3** — Custom properties, Grid, Flexbox, animasi keyframe
- **Vanilla JavaScript** — DOM manipulation, IntersectionObserver
- **Google Fonts** — Playfair Display + DM Sans
- **WhatsApp API** — `wa.me` deep link untuk direct chat

---

## 📄 Lisensi

Project ini bebas digunakan untuk keperluan pribadi maupun komersial.  
Silakan fork, modifikasi, dan kembangkan sesuai kebutuhan.

---

> Dibuat dengan ❤️ untuk UMKM kuliner Indonesia 🇮🇩
