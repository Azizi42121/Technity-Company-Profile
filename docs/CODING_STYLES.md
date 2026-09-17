# Coding Style Guidelines - Technity Website

Dokumen ini berisi aturan penulisan kode untuk proyek Technity. Tujuannya adalah menjaga keterbacaan, konsistensi, dan kemudahan perawatan kode antar-developer.

## 1. Aturan Umum

* **Indentasi:** Gunakan **Tab** untuk semua file HTML, CSS, dan JS.
* **Bahasa:** Gunakan bahasa inggris untuk penamaan file, variable, fungsi, dan nama class/id

## 2. HTML Guidelines

### A. Penamaan Class & ID
* Gunakan format **`kebab-case`** untuk nama class dan id
    * *Benar:* `hero-section`, `btn-primary`, `nav-link`
    * *Salah:* `heroSection`, `btn_primary`, `navlink`

### B. Struktur & Semantic HTML
* Gunakan tag HTML5 yang semantik (`<header>, <nav>, <main>, <section>, <aside>, <article>, <footer>`)
* Jangan gunakan tag `<div>` secara berlebihan tanpa alasan teknis.
* Semua elemen gambar (`<img>`) **wajib** memiliki atribut `alt` yang deskriptif.

```
html
<!--Contoh HTML yang benar-->
<section class="portofolio-section">
    <h2 class="section-title">Portofolio Kami</h2>
    <img src="assets/images/project-1.jpg" alt="Pratinjau Aplikasi Technity" class="portofolio-img">
</section>
```

## 3. CSS Guidelines

### A. Konvensi Penamaan & Struktur
* Gunakan format `kebab-case` untuk semua properti dan variabel CSS.
* Kelompokkan CSS berdasarkan modul atau komponen menggunakan komentar yang jelas.

### B. Variabel CSS (CSS Custom Properties)
* Semua warna dan font utama wajib menggunakan variabel CSS yang telah didefinisikan d `:root` sesuai `docs/UI_GUIDELINES.md`

```
\* Contoh CSS yang baik *\
:root {
    --primary-color: #2563eb;
    --font-main: 'inter', sans-serif;
}

.btn-primary {
    background-color: var(--primary-color);
    font-family: var(--font-main);
    border-radius: 8px;
    padding: 12px 14px;
}
```

## 4. Javascript Guidelines

### A. Penamaan Variabel & Fungsi
* Variabel & fungsi menggunakan `camelCase`.
    Contoh: `portofolioData`, `fetchProject()`, `isMenuOpen`
* Konstanta (Constant) memakai `UPPER_SNAKE_CASE` jika nilainya tetap dan bernilai global.
    Contoh: `MAX_ITEM_PER_PAGE`

### B. Deklarasi Variabel
* Gunakan `const` secara default. Gunakan `let` jika variabel memang akan diubah.
* Dilarang menggunakan `var`.

### C. Tanda Petik & Titik Koma
* Gunakan titik tunggal (') untuk string, atau backticks (``) untuk string templat.
* Wajib menggunakan titik koma (;) di akhir baris statement.

```
// Contoh JS yang Baik
const API_BASE_URL = '[https://api.technity.com/v1](https://api.technity.com/v1)';

async function fetchProjects() {
  try {
    const response = await fetch(`${API_BASE_URL}/projects`);
    const data = await response.json();
    return data;
  } catch (error) {
    console.error('Gagal mengambil data portofolio:', error);
  }
}
```

## 5. Penamaan File & Folder
* Nama File menggunakan format `kebab-case` dan huruf kecil (lowercase).
    * Benar: `about-us.html`, `main-style.css`
    * Salah: `AboutUs.html`, `main_style.css`
* Aset gambar disimpan di folder `assets/images/` dengan penamaan yang menjelaskan isinya (contoh: bg-hero.jpg)