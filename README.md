# Undangan Pernikahan Digital
## Fajar Tri Suhartono & Aji Febriyanti

Website undangan pernikahan modern dengan desain kekinian. Siap di-host di **GitHub Pages**.

### Fitur
- Cover opening elegan (klik "Buka Undangan")
- Countdown timer ke hari H
- Profil mempelai
- Detail acara Akad & Resepsi + link Google Maps
- Galeri prewedding dengan lightbox
- Form RSVP (tersimpan di browser)
- Buku tamu & ucapan (tersimpan di browser)
- Wedding gift / rekening
- Tombol musik latar (opsional)
- Responsive (mobile-friendly)
- Navigasi smooth scroll

### Cara Deploy ke GitHub Pages

#### Opsi 1: Repo baru di akun `fajartris17` (disarankan)

```bash
# 1. Buat repo baru di GitHub (bisa lewat website atau CLI)
# Nama: wedding-fajar-aji

# 2. Clone & push
git clone https://github.com/fajartris17/wedding-fajar-aji.git
cd wedding-fajar-aji

# 3. Copy file index.html ke sini
# (file sudah ada di folder ini)

git add .
git commit -m "feat: undangan pernikahan Fajar & Aji"
git push origin main
```

Lalu di GitHub:
1. Buka repo → **Settings** → **Pages**
2. Source: **Deploy from a branch** → Branch: `main` → Folder: `/ (root)`
3. Save

Website akan live di:
`https://fajartris17.github.io/wedding-fajar-aji/`

#### Opsi 2: Push ke repo Aji (`ajifebriyanti03-netizen/bio`)

Jika punya akses:
```bash
git clone https://github.com/ajifebriyanti03-netizen/bio.git
cd bio
# copy index.html (atau buat folder wedding/)
git add .
git commit -m "add: undangan pernikahan"
git push origin main
```

### Yang Perlu Diganti

Buka `index.html` dan cari komentar `<!-- GANTI ... -->`:

1. **Tanggal & jam** — di countdown (`weddingDate`) dan teks di Hero & Event
2. **Alamat lengkap** Akad & Resepsi
3. **Nama orang tua**
4. **Foto prewedding** — ganti URL Unsplash dengan foto asli (upload ke folder atau gunakan link)
5. **Nomor rekening** Wedding Gift
6. **Link Maps** — ganti dengan koordinat / alamat sebenarnya
7. **Musik** — tambahkan file `music.mp3` dan uncomment tag `<source>`

### Struktur Folder (opsional)

```
wedding-fajar-aji/
├── index.html
├── music.mp3          (opsional)
├── images/            (foto prewedding)
│   ├── 1.jpg
│   ├── 2.jpg
│   └── ...
└── README.md
```

### Fitur Baru yang Ditambahkan
- **QR Code** undangan (scan untuk buka di HP)
- Tombol **Tambah ke Google Calendar** di setiap acara
- Opsi **Google Form** untuk RSVP (data terkumpul di Google)
- Tombol share Facebook
- Navigasi ke section QR

### Cara Pakai Google Form untuk RSVP
1. Buat Google Form baru dengan pertanyaan: Nama, Jumlah Tamu, Kehadiran, Ucapan
2. Copy link form
3. Ganti `https://forms.google.com/` di index.html dengan link form kamu

### Musik Latar
- Upload file `music.mp3` ke repo
- Uncomment baris `<source src="music.mp3" ...>` di index.html
- Tombol musik di pojok kanan bawah akan aktif

---

Dibuat dengan ❤️ untuk Fajar & Aji
