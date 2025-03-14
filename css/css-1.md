# **CSS Ödevi: Kişisel Profil Sayfası Tasarımı**

## **Amaç**  
Bu ödevde, CSS kullanarak basit ama şık bir kişisel profil sayfası tasarlayacaksınız. Sayfa, CSS selectors, colors ve background özelliklerini içerecektir.

## **Gereksinimler**  
### **1. HTML Yapısı**  
- `index.html` adlı bir dosya oluşturun.
- Aşağıdaki bölümleri içermelidir:
  - Başlık (Adınız ve Soyadınız)
  - Kısa bir tanıtım paragrafı
  - İlgi alanları listesini içeren bir `<ul>`
  - Profil fotoğrafınız (`img` etiketi)
  - Dış bir bağlantı (örn. sosyal medya profili - a)

### **2. CSS Kuralları (`style.css` dosyası içinde tanımlanmalıdır)**  
- **CSS Seçiciler:** En az bir `class` ve bir `id` seçicisi kullanın.
- **CSS Ekleme Yöntemleri:**  
  - **External CSS:** Sayfaya `style.css` dosyasını bağlayın.  
  - **Inline CSS:** Bir etikete inline stil ekleyin.  
  - **Internal CSS:** `<style>` etiketi içinde en az bir stil tanımlayın.
- **Renk Kullanımı:**  
  - Sayfa arka plan rengi `rgb` veya `hex` formatında olmalıdır.
  - Başlık rengi belirgin bir renk olmalıdır.
- **Arka Plan Özellikleri:**  
  - `background-color` kullanarak belirli bir bölüme arka plan rengi ekleyin.
  - `background-image` ile sayfanın arka planına bir resim ekleyin.
  - `background-position`, `background-repeat`, `background-attachment` özelliklerini kullanarak arka planı düzenleyin.

## **Örnek HTML Kodu (`index.html`)**  
```html
<!DOCTYPE html>
<html lang="tr">
<head>
    <meta charset="UTF-8">
    <title>Kişisel Profil</title>
    <link rel="stylesheet" href="style.css">
    <style>
        h1 {
            color: #3498db;
        }
    </style>
</head>
<body>
    <header>
        <h1 id="baslik">Merhaba, Ben Ali!</h1>
    </header>
    <section class="profil">
        <img src="profil.jpg" alt="Profil Fotoğrafı">
        <p>Ben bir web geliştirme öğrencisiyim ve HTML & CSS öğreniyorum.</p>
    </section>
    <section>
        <h2>İlgi Alanlarım</h2>
        <ul>
            <li>Programlama</li>
            <li>Fotoğrafçılık</li>
            <li>Oyun Geliştirme</li>
        </ul>
    </section>
    <footer>
        <p>Beni takip edin: <a href="https://www.instagram.com/kullaniciadi" target="_blank">Instagram</a></p>
    </footer>
</body>
</html>
```

## **Örnek CSS Kodu (`style.css`)**  
```css
body {
    background-image: url('arka-plan.jpg');
    background-size: cover;
    background-repeat: no-repeat;
    background-attachment: fixed;
}

#baslik {
    text-align: center;
    font-size: 32px;
}

.profil {
    background-color: rgba(255, 255, 255, 0.8);
    padding: 20px;
    width: 300px;
    margin: auto;
    text-align: center;
    border-radius: 10px;
}

