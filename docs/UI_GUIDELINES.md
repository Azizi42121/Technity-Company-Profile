# UI/UX Guidelines - Technity Website

Dokumen ini berisi standar acuan visual dan komponen antarmuka (UI) sementara yang digunakan dalam pengembangan front-end situs profil perusahaan Technity sebelum desain final dari tim UI/UX diberikan.

## 1. Palet Warna
Buat variabel CSS berikut agar warna tetap konsisten:

* **Primary (Warna Utama):** `#256EB` (Digunakan untuk tombol utama, link, dan aksen penting)
* **Primary Hover:** `#1D4ED8` (Efek saat kursor diarahkan ke tombol)
* **Neutral Dark (Teks Utama):** `#0F172A` (Digunakan untuk judul dan paragraf)
* **Neutral Light (Background):** `#F8FAFC` (Digunakan untuk latar belakang section sekunder)
* **Surface (Card/Box):** `#FFFFFF` (Digunakan untuk latar belakang card portofolio atau form)
* **Border/Line:** `#E2E8F0` (Garis pembatas tipis)

## 2. Tipografi
* **Font Family Utama:** `'Inter', sans-serif`
* **Skala Ukuran Teks:**
    * **Heading 1 (`<h1>`):** `2.5rem` (40px) / Line-height: `1.2` (Judul Hero Section).
    * **Heading 2 (`<h2>`):** `2rem` (32px) / Line-height: `1.3` (Judul Section/Bagian).
    * **Heading 3 (`<h3>`):** `1.25rem` (20px) / Line-height: `1.4` (Judul Card/Sub-bagian).
    * **Body Text (`<p>`):** `1rem` (16px) / Line-height: `1.6` (Teks paragraf biasa).
    * **Small / Caption:** `0.875rem` (14px) / Line-height: `1.5`.

## 3. Komponen Utama

### A. Tombol (Buttons)
* **Primary Button:**
  * Background: `#2563EB`, Teks: Putih (`#FFFFFF`).
  * Border-radius: `8px` (Sedikit melengkung modern).
  * Padding: `12px 24px`.
* **Secondary Button / Outline:**
  * Background: Transparan, Border: `1px solid #2563EB`, Teks: `#2563EB`.

### B. Card Portofolio
* **Rasio Gambar:** `16:9` (Gunakan properti CSS `object-fit: cover` agar gambar tidak gepeng).
* **Shadow / Bayangan:** Lembut untuk memberikan efek kedalaman (`box-shadow: 0 4px 6px -1px rgb(0 0 0 / 0.1)`).
* **Border-radius Card:** `12px`.

## 4. Responsivitas
Soon.