# StrukturData-Q1-2501010350-Vivekananda-C

### 1. Karakteristik Memori dan Akses Data
Array bisa mengakses elemen secara langsung karena lokasinya berurutan dan dapat dihitung secara matematis, sedangkan singly linked list harus menelusuri satu per satu node karena lokasinya tersebar dan hanya terhubung melalui pointer.

### 2. Analisis Efisiensi Operasi Manipulasi
Linked List lebih unggul dibanding Array ketika:

- Banyak operasi insert/delete (terutama di tengah/depan)
- Ukuran data dinamis
- Tidak membutuhkan akses langsung berbasis indeks

Hal ini karena Linked List hanya perlu memanipulasi pointer, sedangkan Array harus menggeser elemen dalam memori kontinu, yang membutuhkan waktu lebih besar.

### 3. Konsep Doubly Linked List
Penambahan pointer prev pada Doubly Linked List memberikan:

Keuntungan:
- Traversal dua arah
- Operasi insert/delete lebih fleksibel dan efisien
- Tidak perlu traversal ulang untuk akses node sebelumnya
Kerugian:
- Konsumsi memori lebih besar
- Implementasi lebih kompleks

### 4. Mekanisme Circular Linked List
Circular Linked List berbeda dari Linked List biasa karena:

- Tidak memiliki akhir (NULL)
- Membentuk siklus
- Mendukung traversal berulang secara alami

Struktur ini lebih efektif digunakan pada sistem yang:

- Bersifat loop/berulang
- Membutuhkan rotasi berkelanjutan, seperti penjadwalan, playlist, atau sistem antrian melingkar

### 5. Array Dinamis di Python
Mekanisme yang Terjadi
1. Cek kapasitas
Jika size == capacity, array sudah penuh dan tidak bisa menampung elemen baru.
2. Alokasi array baru
Sistem membuat array baru dengan kapasitas lebih besar (biasanya diperbesar dengan faktor tertentu, bukan hanya +1).
3. Penyalinan elemen
Semua elemen dari array lama disalin ke array baru → membutuhkan waktu O(n).
4. Menambahkan elemen baru
Elemen yang di-append dimasukkan ke posisi berikutnya di array baru.
5. Menghapus array lama
Memori array lama dilepas (garbage collection).
