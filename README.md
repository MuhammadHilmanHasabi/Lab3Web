# Lab3Web

Codingan:

![Screenshot (89)1](https://github.com/user-attachments/assets/7aa57df8-2108-4fc4-b3b8-6b862c8d4be2)
![Screenshot (90)1](https://github.com/user-attachments/assets/c4aaffb0-122c-40df-b951-710208ee8c90)
![Screenshot (91)1](https://github.com/user-attachments/assets/443d768e-a357-4ef7-a71e-ebd7284e5bf3)


Hasil:

![Screenshot (92)1](https://github.com/user-attachments/assets/9d8b81d0-1498-4018-a382-2e4db7d4ae31)

Penjelasan:

1. File `index.html` (HTML):
   - Menyusun struktur dasar form dengan dropdown dan listbox.
   - Pada elemen dropdown `<select>`, digunakan atribut `onchange="updateSelection()"` untuk memanggil fungsi JavaScript setiap kali pengguna memilih sesuatu.
   - Listbox dibuat dengan atribut `multiple` yang memungkinkan pemilihan lebih dari satu item.
   - Script `scripts.js` dihubungkan di bagian akhir dengan `<script src="scripts.js"></script>`.

2. File `styles.css` (CSS):
   - Menambahkan beberapa styling sederhana, seperti font default, margin, serta lebar dan tinggi untuk listbox.

3. File `scripts.js` (JavaScript):
   - Fungsi `updateSelection()` bertanggung jawab untuk:
   - Mengambil nilai yang dipilih dari dropdown (`selectedDropdown`).
   - Mengambil nilai yang dipilih dari listbox (`selectedListbox`), menggunakan metode `.filter()` untuk menemukan opsi yang dipilih, dan `.map()` untuk mendapatkan teks dari opsi       
     tersebut.
   - Memperbarui tampilan hasil pilihan dengan menulis ulang konten dari elemen `<p>` yang memiliki id `selection`.
   - Fungsi ini dipanggil setiap kali ada perubahan di dropdown atau listbox. Untuk listbox, event listener dipasang untuk mendeteksi perubahan dengan `addEventListener("change", 
     updateSelection)`.
