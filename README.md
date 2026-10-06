# Praktikum 3: CSS Dasar - Pemrograman Web

Repository ini dibuat untuk menyelesaikan tugas **Praktikum 3: CSS Dasar** pada mata kuliah **Pemrograman Web** di Universitas Pelita Bangsa.

## Tujuan Praktikum
1. Mahasiswa mampu memahami konsep dasar CSS.
2. Mahasiswa mampu memahami aturan penulisan pada CSS.
3. Mahasiswa mampu memahami selector sebagai pengontrol CSS.
4. Mahasiswa mampu membuat pengaturan CSS pada HTML.

---

## Langkah-Langkah Praktikum

### 1. Membuat Dokumen HTML (`lab2_css_dasar.html`)
Membuat struktur dasar dokumen HTML yang berisi bagian header, navigasi, serta konten dengan elemen `div` (ber-ID `#intro`) dan tautan ber-kelas (`button btn-primary`).

### 2. Mendeklarasikan CSS Internal
Menambahkan tag `<style>` di dalam bagian `<head>` dokumen HTML untuk mengatur font global, header, elemen `h1`, serta format teks miring di dalam `h1`.

### 3. Menambahkan Inline CSS
Menambahkan atribut `style` secara langsung pada tag paragraf `<p>` untuk mengatur perataan teks dan warna secara spesifik pada baris tersebut.

### 4. Membuat CSS Eksternal (`style_eksternal.css`)
Memisahkan kode styling ke dalam file eksternal `style_eksternal.css` dan menghubungkannya menggunakan tag `<link>` pada bagian `<head>` HTML. Mengatur tampilan elemen navigasi dan link agar lebih rapi serta interaktif (`hover`).

### 5. Menambahkan CSS Selector (ID & Class Selector)
Menambahkan deklarasi ID Selector (`#intro`, `#intro h1`) dan Class Selector (`.button`, `.btn-primary`) pada file CSS eksternal untuk mempercantik tata letak kotak konten dan tombol interaktif.

---

## Jawaban Pertanyaan & Tugas

1. **Eksperimen CSS Cheat Sheet:** 
   Eksperimen properti tambahan seperti `box-shadow`, `border-radius`, dan `transition` pada tombol berhasil diterapkan untuk memperkaya tampilan antarmuka.
2. **Perbedaan `h1 {...}` dengan `#intro h1 {...}`:**
   - `h1 {...}` adalah *Element Selector* yang bersifat global, artinya aturan CSS tersebut akan diterapkan ke **seluruh** elemen `h1` di dalam halaman web.
   - `#intro h1 {...}` adalah *Descendant Selector* (kombinasi ID dan Element), yang hanya akan diterapkan pada elemen `h1` yang berada **di dalam** kontainer atau elemen dengan `id="intro"`.
3. **Prioritas Deklarasi CSS (Internal vs Eksternal vs Inline):**
   - **Inline CSS** memiliki prioritas tertinggi, diikuti oleh **Internal/Eksternal CSS** (tergantung urutan pemuatannya, di mana yang terakhir dimuat akan menimpa yang sebelumnya). 
   - *Contoh:* Jika elemen `<p>` diberi warna hijau di eksternal, lalu diberi warna biru melalui inline style `style="color: blue;"`, maka browser akan menampilkan warna **biru**.
4. **Prioritas ID Selector vs Class Selector:**
   - **ID Selector** memiliki tingkat spesifisitas (specificity) yang lebih tinggi dibandingkan **Class Selector**. 
   - *Contoh:* Jika `<p id="paragraf-1" class="text-paragraf">` memiliki aturan `#paragraf-1 { color: red; }` dan `.text-paragraf { color: green; }`, maka teks akan berwarna **merah** karena ID selector lebih spesifik daripada class selector.

---
## Author
- **Mata Kuliah:** Pemrograman Web
- **Dosen Pengampu:** Agung Nugroho, S.Kom., M.Cs.
- **Institusi:** Universitas Pelita Bangsa, Bekasi