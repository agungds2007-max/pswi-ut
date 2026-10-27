…or create a new repository on the command line
echo "# pswi-ut" >> README.md
git init
git add README.md
git commit -m "first commit"
git branch -M main
git remote add origin https://github.com/agungds2007-max/pswi-ut.git
git push -u origin main


…or push an existing repository from the command line
git remote add origin https://github.com/agungds2007-max/pswi-ut.git
git branch -M main
git push -u origin main



# Pendaftaran Kegiatan

Tugas pembuatan formulir pendaftaran kegiatan menggunakan HTML dan CSS, lalu di-push ke Git.

## Pembuat

- Nama: (isi namamu)
- NIM: (isi NIM)
- Program studi: (isi prodi)

## Ketentuan Tugas

- [x] Pembuatan form menggunakan HTML
- [x] Penggunaan dan penerapan CSS
- [x] Push project ke Git
- [x] Membuat file `README.md`
- [x] Menyertakan bukti pengerjaan

## Struktur Folder

```
.
├── index.html     # halaman formulir pendaftaran
├── style.css      # tampilan halaman
├── README.md      # dokumentasi
└── bukti/         # screenshot bukti pengerjaan
```

## 1. Form HTML

Formulir dibuat di `index.html` dengan elemen semantik (`header`, `nav`, `main`, `form`, `fieldset`, `legend`, `figure`) dan kolom berikut:

| Kolom | Elemen | Validasi |
|---|---|---|
| Nama lengkap | `input` | wajib |
| Email | `input type="email"` | wajib, format email |
| Telepon | `input type="tel"` | wajib |
| Program studi | `select` | wajib dipilih |
| Jumlah tiket | `input type="number"` | wajib, 1 sampai 5 |
| Kode peserta | `input` + `pattern` | wajib, tepat 6 angka |
| Mode kehadiran | `radio` | wajib, Luring atau Daring |
| Minat belajar HTML | `radio` | wajib, Ya atau Tidak |
| Catatan | `textarea` | opsional, maksimal 300 karakter |

## 2. Penerapan CSS

Tampilan diatur di `style.css` dan dihubungkan lewat `<link rel="stylesheet" href="style.css">`. CSS yang diterapkan:

- Warna latar, header, dan tombol bertema biru-teal.
- Form berada di dalam kartu putih yang rata tengah.
- Input, select, dan textarea memiliki lebar penuh, border, dan sudut membulat.
- Kolom yang salah isi diberi border merah (`:user-invalid`).
- Gambar responsif (`max-width: 100%`).

## 3. Push ke Git

```bash
git init
git add .
git commit -m "Tambah form pendaftaran kegiatan dengan HTML dan CSS"
git branch -M main
git remote add origin <url-repositori>
git push -u origin main
```

Link repositori: (isi link GitHub kamu)

## 4. Cara Menjalankan

1. Pastikan `index.html` dan `style.css` berada di folder yang sama.
2. Buka `index.html` di browser.

## 5. Bukti Pengerjaan

**Tampilan halaman**

![Tampilan halaman](bukti/tampilan.png)

**Validasi form (kolom kosong atau format salah)**

![Validasi form](bukti/validasi.png)

**Form berhasil dikirim (data muncul di URL)**

![Form terkirim](bukti/terkirim.png)

**Riwayat commit dan push**

![Git log](bukti/git-log.png)

**Repositori di GitHub**

![Repositori GitHub](bukti/github.png)

## Catatan

- Formulir memakai `method="get"`, jadi data muncul di URL setelah tombol **Daftar** ditekan dan belum disimpan ke server.
- Halaman `kegiatan.html` dan `daftar.html` pada menu belum tersedia.