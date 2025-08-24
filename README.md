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

1. **Kustomisasi Navbar dengan Hamburger Menu**    
   Navbar Bootstrap dimodifikasi dengan hamburger menu kustom untuk layar kecil (≤768px), menggunakan `nav-toggle` dan animasi CSS untuk transisi halus.  
   ```css
    .nav-toggle:checked ~ .nav-links {
      max-height: 500px;
    }
    .nav-toggle-label .hamburger {
      transition: all 0.3s ease-in-out;
    }

2. **Background Override**    
   Bootstrap default tidak menggunakan gambar latar. Di sini diganti dengan kombinasi `background-image` dan **linear-gradient** untuk menciptakan kesan modern.

   ```css
    body {
      background-image: url('assets/bg.jpg');
      background-size: cover;
      background-position: center;
      background-attachment: fixed;
      min-height: 100vh;
      padding: 20px;
      display: flex;
      flex-direction: column;
      justify-content: flex-start;
      align-items: center;
    }
    
    .profile-container {
      background: linear-gradient(160deg, rgba(5,3,29,0.9), rgba(11,54,82,0.9));
   ```

3. **Tombol Back-to-Top**  
  Ditambahkan tombol`Back to Top` dengan desain melayang untuk navigasi lebih mudah.

   ```css
    #back-to-top {
      position: fixed;
      bottom: 20px;
      right: 20px;
      background-color: rgba(109, 128, 141, 0.451);
      border-radius: 50%;
      transition: background-color 0.3s ease;
    }
   ```

4. **Video Portofolio Proyek Responsif**  
    Video proyek (misalnya, Roblox - Tower Indonesia, Space Invaders) ditampilkan dalam container responsif menggunakan `padding-bottom: 50%` untuk menjaga rasio aspek.

   ```css
    .video-container {
      position: relative;
      padding-bottom: 50%;
      height: 0;
      overflow: hidden;
    }
   ```

5. **Tipografi & Daftar Kustom**  
   Heading diberi garis bawah dekoratif, sedangkan daftar menggunakan `list-style-type: circle`.

   ```css
    .about-section h3 {
      font-size: 1.5em;
      margin: 15px 20px 12px 20px;
      color: white;
      border-bottom: 2px solid rgba(255, 255, 255, 0.2);
      padding-bottom: 5px;
    }

    .about-section li {
      line-height: 1.5;
      color: rgb(255, 255, 255);
      list-style-type: circle;
      margin: 5px 25px 5px 5px;
      text-align: left;
    }
   ```

6. **Media Query Kustom**  
   Penyesuaian pada breakpoint ≤768px untuk navbar, kontak, dan ukuran font, meningkatkan pengalaman pengguna di perangkat mobile.
 
   ```css
    @media (max-width: 768px) {
      .navbar {
        flex-direction: column;
        align-items: flex-end;
      }
      .contact-row {
        flex-direction: column;
        align-items: center;
      }
    }
   ```
Dibuat dengan ❤️ oleh **Muhammad Ihsan Ramadhan**
