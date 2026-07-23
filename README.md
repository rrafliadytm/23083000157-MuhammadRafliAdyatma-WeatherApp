# Weather Forecast App - Muhammad Rafli Adyatma

Aplikasi prakiraan cuaca modern berbasis Android yang dibangun menggunakan **Jetpack Compose**. Aplikasi ini memungkinkan pengguna untuk mencari cuaca di berbagai kota dengan data real-time, menampilkan ramalan cuaca 7 hari ke depan dengan antarmuka yang bersih dan interaktif.

## 📸 Snapshots

| Main Weather Screen | Search Suggestion | Error State |
|:---:|:---:|:---:|
| ![Main Screen](https://via.placeholder.com/200x400?text=Main+Weather) | ![Search](https://via.placeholder.com/200x400?text=Search+City) | ![Error](https://via.placeholder.com/200x400?text=Error+State) |

> *Catatan: Silakan ganti placeholder di atas dengan screenshot asli dari folder `screenshots/` Anda.*

## ✨ Fitur Utama

- **Pencarian Kota Real-time**: Mencari koordinat lokasi menggunakan Geocoding API dengan fitur auto-suggestion saat mengetik.
- **Ramalan Cuaca 7 Hari**: Menampilkan suhu harian (Max/Min), probabilitas hujan, dan total curah hujan.
- **Antarmuka Modern (Material 3)**: Menggunakan komponen Material 3, gradient background, dan kartu (cards) yang responsif.
- **Indikator Visual**: Ikon cuaca dinamis (Sunny, Cloudy, Stormy) dan progress bar untuk probabilitas hujan.
- **Pull-to-Refresh**: Memperbarui data cuaca terbaru dengan menggeser layar ke bawah.
- **Shimmer Loading**: Efek loading animasi modern saat memuat data.
- **Error Handling**: Tampilan error yang informatif jika koneksi gagal atau kota tidak ditemukan, lengkap dengan tombol *Retry*.

## 🚀 Teknologi yang Digunakan

- **Bahasa**: [Kotlin](https://kotlinlang.org/)
- **UI Framework**: [Jetpack Compose](https://developer.android.com/jetpack/compose)
- **Networking**: [Retrofit](https://square.github.io/retrofit/) & [Gson](https://github.com/google/gson) (Open-Meteo API)
- **Architecture**: MVVM (Model-View-ViewModel)
- **State Management**: Kotlin Flows & StateFlow
- **Dependency**: Material Icons Extended untuk ikon cuaca yang lengkap.

## 🛠️ Cara Penggunaan

1. **Melihat Cuaca Default**: Saat pertama kali dibuka, aplikasi akan menampilkan cuaca di lokasi default (**Malang**).
2. **Mencari Kota**:
   - Ketik nama kota pada kolom pencarian di bagian atas.
   - Pilih kota yang muncul pada daftar saran (dropdown).
   - Tekan tombol *Enter* pada keyboard untuk memulai pencarian.
3. **Memperbarui Data**: Tarik layar dari atas ke bawah (**Pull-to-Refresh**) untuk mengambil data terbaru.
4. **Membaca Informasi**:
   - Bagian atas kartu menampilkan tanggal dan kondisi umum.
   - Bagian tengah menampilkan suhu maksimum dan minimum.
   - Bagian bawah menampilkan probabilitas hujan dalam persen dan volume air (mm).

## 📁 Struktur Folder

```text
com.example.week6_weatherforecast/
├── data/
│   ├── api/          # Konfigurasi Retrofit & API Service
│   ├── model/        # Data Classes (POJO) untuk API Response
│   └── repository/   # Logika pengambilan data (WeatherRepository)
├── ui/
│   ├── screen/       # WeatherScreen.kt (UI Utama)
│   ├── state/        # WeatherUiState.kt (State UI)
│   ├── theme/        # Tema Material 3, Warna, dan Tipografi
│   └── viewmodel/    # WeatherViewModel.kt (Logika Bisnis UI)
└── MainActivity.kt   # Entry point aplikasi
```

## 👨‍💻 Author

**Muhammad Rafli Adyatma**  
NIM: 23083000157  
Mata Kuliah: Pemrograman Mobile (Semester 6)
