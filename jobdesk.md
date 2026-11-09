Pembagian paling sehat itu potong vertikal per lapisan, bukan"A ngerjain semua UI, B semua backend" — karena kalau gitu, Bkelar duluan terus nganggur, dan A jadi bottleneck.

Orang (Baskara) — Fondasi & Data Layer

• Setup Supabase: tabel mata_kuliah + tugas, relasi FK, seeddata
• ApiService (semua HTTP call: GET/POST/PATCH/DELETE)
• Tugas & MataKuliah model + fromJson() / toJson()
• Setup GetX routing + config.dart
• Ini wajib paling cepat, semua orang nungguin

Orang (Fahmi) — Halaman Baca & Logika Prioritas

• TugasController (.obs, Obx, state loading/error/retry)
• Halaman daftar tugas + sorting prioritas + badge urgensi
• Halaman detail + countdown sisa hari
• Ini yang jadi fitur tambahan di laporan

Orang (Nailul) — Halaman Tulis & CRUD

• Halaman form tambah/edit + validasi input
• Operasi create / update / delete tugas (nyambung keApiService Orang 1)
• Halaman CRUD mata kuliah
• Error handling saat submit gagal