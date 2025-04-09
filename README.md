## Belajar Android

### 1. Pengenalan Android Development

**Android Studio**  
Android Studio adalah lingkungan pengembangan resmi dari Google untuk membuat aplikasi Android. Di dalamnya sudah termasuk editor kode, tools debugging, emulator, dan integrasi dengan library Android.

**Struktur Project Android**  
- `AndroidManifest.xml`: mendeklarasikan komponen aplikasi, seperti activity dan permission.
- `java/` atau `kotlin/`: folder tempat kamu menulis logika aplikasi.
- `res/`: berisi resource seperti file XML layout, gambar, dan string.
- `build.gradle`: digunakan untuk mengelola versi SDK, dependencies, dan konfigurasi project.

**Menjalankan Emulator atau Perangkat Nyata**  
Emulator digunakan untuk menjalankan aplikasi tanpa harus memiliki perangkat fisik. Namun, testing di perangkat nyata juga penting untuk memastikan performa dan kompatibilitas.

---

### 2. Dasar UI Android

#### A. XML Layout  
XML adalah cara tradisional untuk mendesain antarmuka pengguna di Android. Contohnya:
```xml
<Button
    android:id="@+id/buttonClick"
    android:layout_width="wrap_content"
    android:layout_height="wrap_content"
    android:text="Klik Aku"/>
```
Layout yang umum digunakan:
- `LinearLayout`: menyusun elemen secara vertikal atau horizontal.
- `RelativeLayout`: menyusun elemen relatif terhadap elemen lainnya.
- `ConstraintLayout`: layout paling fleksibel dan efisien untuk UI kompleks.

#### B. Jetpack Compose  
Jetpack Compose adalah toolkit UI modern dari Google. Dibuat menggunakan Kotlin dan mendukung pendekatan deklaratif:
```kotlin
@Composable
fun Greeting(name: String) {
    Text(text = "Hello $name")
}
```
Keuntungan Compose:
- Kode UI lebih ringkas dan mudah dibaca.
- Mudah mengatur state dan responsif terhadap perubahan data.

---
