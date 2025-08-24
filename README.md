# 🌐 CV Pribadi – Muhammad Ihsan Ramadhan  

Website ini adalah **CV pribadi** yang dirancang untuk menampilkan profil, keahlian, portofolio, pendidikan, dan pengalaman secara profesional. Dibangun dengan pendekatan **responsif** sehingga dapat diakses dengan baik pada berbagai ukuran perangkat, serta menggunakan desain modern yang sederhana namun elegan.  

🔗Anda dapat mengakses CV saya di [**ihsan-ramadhan.github.io/CV-Ihsan**](https://ihsan-ramadhan.github.io/CV-Ihsan/)

## 🚀 Teknologi yang Digunakan
- **HTML5**
- **CSS3**
- **Bootstrap 5.3.7**
  
## 🛠️ Dokumentasi & Modifikasi
Proyek ini menggunakan **Bootstrap 5.3.7** sebagai basis, kemudian dimodifikasi dengan file `styles.css` untuk menyesuaikan desain dan fungsionalitas.  

### 🔧 Modifikasi Utama

1. **Background Override**  
   Bootstrap default tidak menggunakan gambar latar. Di sini diganti dengan kombinasi `background-image` dan **linear-gradient** untuk menciptakan kesan modern.  
   ```css
   body {
     background-image: url('assets/bg.jpg');
     background-size: cover;
     background-position: center;
     background-attachment: fixed;
   }

   .profile-container {
     background: linear-gradient(160deg, rgba(5,3,29,0.9), rgba(11,54,82,0.9));
   }

2. **Profile Container dengan Efek Modern**
   Ditambahkan **box-shadow** dan **border-radius** untuk memberikan kedalaman visual.

   ```css
   .profile-container {
     border-radius: 15px;
     box-shadow: 0 8px 20px rgba(0, 0, 0, 0.4);
     padding: 25px;
     max-width: 1000px;
   }
   ```

3. **Profile Image Kustom**
   Mengubah foto profil menjadi bulat sempurna dengan border putih, serta memanfaatkan `object-fit: cover`.

   ```css
   .profile-image {
     width: 140px;
     height: 140px;
     border-radius: 100%;
     border: 4px solid white;
     object-fit: cover;
   }
   ```

4. **Contact Section dengan Flexbox Kustom**

   ```html
   <div class="contact-row">
     <div class="contact-column">
       <li>☎️ +62 823-7927-2365</li>
       <li>✉️ m.ihsan.r30@gmail.com</li>
     </div>
     <div class="contact-column">
       <li>🔗 <a href="#">LinkedIn</a></li>
       <li>💻 <a href="#">GitHub</a></li>
     </div>
   </div>
   ```

   ```css
   .contact-row {
     display: flex;
     justify-content: center;
   }

   .contact-column {
     display: flex;
     flex-direction: column;
     margin: 5px 40px;
   }
   ```

5. **Tipografi & Daftar Kustom**
   Heading diberi garis bawah dekoratif, sedangkan daftar menggunakan `list-style-type: circle`.

   ```css
   .about-section h3 {
     font-size: 1.6em;
     border-bottom: 2px solid rgba(255, 255, 255, 0.2);
     padding-bottom: 5px;
   }

   .about-section li {
     list-style-type: circle;
     margin: 5px 25px;
   }
   ```

6. **Media Query Kustom**
   Untuk responsivitas, dibuat aturan tambahan pada breakpoint `768px`. Dengan ini, kontak berubah menjadi susunan kolom saat layar kecil.

   ```css
   @media (max-width: 768px) {
     .contact-row {
       flex-direction: column;
       align-items: center;
     }

     .contact-column {
       width: 100%;
       align-items: center;
       margin: 0;
     }
   }
   ```
Dibuat dengan ❤️ oleh **Muhammad Ihsan Ramadhan**
