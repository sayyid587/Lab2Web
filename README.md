# Lab2Web


## 📝 Langkah-Langkah Praktikum  

### 1. Membuat Dokumen HTML
Buat file baru dengan nama **lab2_css_dasar.html**, isi dengan kode berikut:  

```html
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>CSS Dasar</title>
</head>
<body>
  <header>
    <h1>CSS Internal dan <i>Inline CSS</i></h1>
  </header>
  <nav>
    <a href="lab2_css_dasar.html">CSS Dasar</a>
    <a href="lab2_css_eksternal.html">CSS Eksternal</a>
    <a href="lab1_tag_dasar.html">HTML Dasar</a>
  </nav>

  <!-- CSS ID Selector -->
  <div id="intro">
    <h1>Hello World</h1>
    <p>Kami sedang belajar HTML dan CSS dasar pada mata kuliah <b>Pemrograman Web</b>.</p>
    <!-- CSS Class Selector -->
    <a class="button btn-primary" href="#intro">Informasi selengkapnya</a>
  </div>
</body>
</html>
```

📷 **Screenshot hasil:**  
![Screenshot Step 1](images/step1.png)  

---

### 2. Menambahkan CSS Internal
Tambahkan kode berikut di dalam tag `<head>`:  

```html
<head>
  <title>CSS Dasar</title>
  <style>
    body {
      font-family: 'Open Sans', sans-serif;
    }
    header {
      min-height: 80px;
      border-bottom: 1px solid #77CCEF;
    }
    h1 {
      font-size: 24px;
      color: #0F189F;
      text-align: center;
      padding: 20px 10px;
    }
    h1 i {
      color: #6d6a6b;
    }
  </style>
</head>
```

📷 **Screenshot hasil:**  
![Screenshot Step 2](images/step2.png)  

---

### 3. Menambahkan Inline CSS
Inline CSS ditulis langsung pada elemen HTML:  

```html
<p style="text-align: center; color: #ccd8e4;">
  Ini adalah paragraf dengan inline CSS.
</p>
```

📷 **Screenshot hasil:**  
![Screenshot Step 3](images/step3.png)  

---

### 4. Membuat CSS Eksternal
1. Buat file baru dengan nama **style_eksternal.css**.  
2. Isi dengan kode berikut:  

```css
body {
  font-family: Arial, sans-serif;
  background: #f0f0f0;
}
```

3. Hubungkan ke file HTML dengan `<link>`:  

```html
<head>
  <link rel="stylesheet" href="style_eksternal.css" type="text/css">
</head>
```

📷 **Screenshot hasil:**  
![Screenshot Step 4](images/step4.png)  

---

### 5. Menambahkan CSS Selector
Tambahkan kode di file **style_eksternal.css**:  

```css
/* ID Selector */
#intro {
  background: #418fb1;
  border: 1px solid #099249;
  min-height: 100px;
  padding: 10px;
}
#intro h1 {
  text-align: left;
  color: #fff;
}

/* Class Selector */
.button {
  padding: 15px 20px;
  background: #bebcbd;
  color: #fff;
  display: inline-block;
  margin: 10px;
  text-decoration: none;
}
.btn-primary {
  background: #E42A42;
}
```

📷 **Screenshot hasil:**  
![Screenshot Step 5](images/step5.png)  

---

## ❓ Pertanyaan
1. Lakukan eksperimen dengan menambah/mengubah properti CSS.  
2. Apa perbedaan antara `h1 { ... }` dengan `#intro h1 { ... }`?  
3. Jika ada CSS internal, eksternal, dan inline pada elemen yang sama, manakah yang diprioritaskan browser?  
4. Jika sebuah elemen memiliki ID dan Class sekaligus, deklarasi manakah yang lebih kuat?  

---
