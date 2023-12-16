# Tubes Inteligensi Buatan

## Contribute

- Chrisnico Alexander Hutapea 120140244
- Yudha Kurnia 120140241

## Getting Started:

1. Follow the steps below to get the code and running:
2. Clone this repository to your local machine:

   ```bash
   https://github.com/Chrisnico123/tubes-ib-120140244-120140241.git

   ```

3. Install Required Dependencies

## Explain Solution

Solusi dari kode yang dibuat oleh kami adalah merancang solusi untuk menyelesaikan permasalahan terkait penjadwalan keluarga dengan mempertimbangan preferensi keluarga terhadap hari tertentu dan juga meminimalkan biaya akuntansi yang terkait dengan jumlah orang yang ditempatkan pada setiap hari.

Pendekatan solusi yang kami ambil adalah localsearch, MIP dan melakukan pemrosesan data. berikut penjelasan dari beberapa fungsi yang kami kembangkan :

1. Pembentukan Matriks biaya
   - GetAssignmentCostMatrix: Membentuk matriks biaya penugasan berdasarkan preferensi keluarga.
   - GetAccountingCostMatrix: Membentuk matriks biaya akuntansi berdasarkan jumlah orang per hari.
2. Pemrosesan dan Pemangkasan-
   - preprocessing: Melakukan pemrosesan dan pemangkasan untuk mengurangi jumlah kemungkinan penugasan.
3. LocalSearch
   - LocalSearch: Implementasi pencarian lokal untuk memperbaiki solusi secara iteratif.
   - local_search_shift_and_swap: Melakukan pencarian lokal dengan menggunakan metode shift dan swap untuk memperbaiki solusi saat ini.
4. Pemrograman Bilangan bulat Campuran(MIP)
   - MIP: Membentuk dan menyelesaikan masalah MIP dengan menggunakan solver ortools.
5. Support Function
   - calculate_solution_cost: Menghitung biaya solusi saat ini.
   - perform_move: Melakukan perpindahan keluarga dari satu hari ke hari lainnya.
   - linearize: Melakukan linearisasi untuk biaya akuntansi menggunakan regresi linier.
6. Storage Solution
   - Menyimpan hasil solusi ke dalam file CSV.
