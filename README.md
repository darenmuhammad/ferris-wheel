# 🎡 ***Ferris Wheel*** 

Proyek ini mendemonstrasikan animasi **ferris wheel** menggunakan HTML dan CSS. Animasi ini dibuat menggunakan **CSS keyframes**, sehingga roda berputar terus-menerus dan warna kabin berubah secara dinamis. ✨

## 🚀 Fitur
- Bianglala yang berputar menggunakan animasi CSS.
- Enam kabin yang tersebar merata dan ikut beranimasi bersama roda.
- Transisi warna yang halus pada kabin di berbagai tahap animasi.

## 📌 Animasi CSS

| Properti CSS                 | Penjelasan |
|------------------------------|------------|
| `@keyframes`                 | Mendefinisikan animasi dengan perubahan gaya pada persentase tertentu dalam durasi animasi. |
| `animation-name`             | Nama animasi yang akan diterapkan ke elemen. |
| `animation-duration`         | Lama waktu animasi berlangsung sebelum mengulang atau berhenti. |
| `animation-timing-function`  | Mengatur bagaimana kecepatan animasi berubah sepanjang waktu, misalnya `linear`, `ease`, `ease-in-out`, dll. |
| `animation-iteration-count`  | Menentukan berapa kali animasi akan berjalan, bisa berupa angka atau `infinite`. |
| `transform-origin`           | Menentukan titik asal transformasi (misalnya `0% 0%` berarti sudut kiri atas, `50% 50%` berarti tengah elemen). |

### 1️⃣ `@keyframes wheel`
Animasi ini diterapkan pada kelas `.wheel`, membuat bianglala berputar terus-menerus. 🔄
```css
@keyframes wheel {
    0% {
        transform: rotate(0deg);
    }
    100% {
        transform: rotate(360deg);
    }
}
```
- **Diterapkan pada**: `.wheel`
- **Efek**: Memutar seluruh roda dalam satu putaran halus.
- **Durasi**: `10s`
- **Timing function**: `linear` (agar kecepatan tetap stabil)
- **Jumlah pengulangan**: `infinite` (berputar terus-menerus)

### 2️⃣ `@keyframes cabins`
Animasi ini diterapkan pada kelas `.cabin`, membuat setiap kabin berputar ke arah berlawanan sambil mengubah warna. 🎭
```css
@keyframes cabins {
    0% {
        transform: rotate(0deg);
    }
    25% {
        background-color: yellow;
    }
    50% {
        background-color: purple;
    }
    75% {
        background-color: yellow;
    }
    100% {
        transform: rotate(-360deg);
    }
}
```
- **Diterapkan pada**: `.cabin`
- **Efek**:
  - Mengubah warna pada interval `25%`, `50%`, dan `75%`.
  - Berputar berlawanan arah dengan roda.
- **Durasi**: `10s`
- **Timing function**: `ease-in-out` (memungkinkan percepatan dan perlambatan yang halus)
- **Jumlah pengulangan**: `infinite`

---
© 2025 | **Ferris Wheel Project**
