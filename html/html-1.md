# HTML Ödevleri

## Ödev 1: Kişisel Tanıtım Sayfası

### Amaç

Bu ödevde, kendinizi tanıtan basit bir web sayfası oluşturacaksınız. Bu sayfa, temel HTML etiketlerini kullanarak kişisel bilgilerinizi, ilgi alanlarınızı ve becerilerinizi göstermenizi sağlayacak.

### Gereksinimler

1. Sayfanızda aşağıdaki HTML etiketlerini kullanmalısınız:
    - `<!DOCTYPE html>`, `<html>`, `<head>`, `<body>` (temel HTML yapısı)
    - `<title>` (sayfa başlığı)
    - `<h1>`, `<h2>`, `<h3>` (başlıklar)
    - `<p>` (paragraflar)
    - `<img>` (en az bir resim)
    - `<ul>` veya `<ol>` ve `<li>` (listeler)
    - `<a>` (linkler)
2. Sayfanız aşağıdaki bölümleri içermelidir:
    - Başlık (adınız ve soyadınız)
    - Kısa bir kişisel tanıtım
    - Eğitim bilgileriniz
    - Hobileriniz veya ilgi alanlarınız
    - Becerileriniz
    - İletişim bilgileriniz (e-posta adresi gibi)

### Örnek Kod

```html
<!DOCTYPE html>
<html lang="tr">
<head>
    <meta charset="UTF-8">
    <title>Benim Sayfam - Ali Yılmaz</title>
</head>
<body>
    <h1>Ali Yılmaz</h1>
    
    <img src="profil.jpg" alt="Profil Fotoğrafım" width="200">
    
    <h2>Hakkımda</h2>
    <p>Merhaba! Ben Ali Yılmaz. 15 yaşındayım ve 9. sınıf öğrencisiyim. Bilgisayar ve teknolojiye ilgi duyuyorum.</p>
    
    <h2>Eğitim</h2>
    <ul>
        <li>Atatürk İlkokulu (2014-2018)</li>
        <li>Cumhuriyet Ortaokulu (2018-2022)</li>
        <li>Bilim Lisesi (2022-devam ediyor)</li>
    </ul>
    
    <h2>Hobilerim</h2>
    <ol>
        <li>Bilgisayar oyunları oynamak</li>
        <li>Kitap okumak</li>
        <li>Bisiklet sürmek</li>
        <li>Müzik dinlemek</li>
    </ol>
    
    <h2>Becerilerim</h2>
    <ul>
        <li>HTML öğreniyorum</li>
        <li>Scratch ile programlama</li>
        <li>İngilizce (orta seviye)</li>
    </ul>
    
    <h2>İletişim</h2>
    <p>E-posta: <a href="mailto:ornek@email.com">ornek@email.com</a></p>
    <p>Instagram: <a href="https://www.instagram.com/kullaniciadi" target="_blank">@kullaniciadi</a></p>
</body>
</html>
```


### İpuçları

- Gerçek bir profil fotoğrafı kullanabilir veya internetten uygun bir resim bulabilirsiniz.
- Bilgilerinizi gerçek veya hayali olarak yazabilirsiniz.

---

## Ödev 2: Basit Anket Formu

### Amaç

Bu ödevde, kullanıcılardan bilgi toplamak için basit bir anket formu oluşturacaksınız. Bu form, HTML form etiketlerini ve farklı input türlerini kullanmanızı sağlayacak.

### Gereksinimler

1. Formunuzda aşağıdaki HTML etiketlerini kullanmalısınız:
    - `<form>` (form yapısı)
    - `<input>` (farklı türlerde: text, email, radio, checkbox)
    - `<textarea>` (çok satırlı metin girişi)
    - `<label>` (form elemanları için etiketler)
    - `<button>` (gönder butonu)
2. Anketiniz aşağıdaki bilgileri toplamalıdır:
    - Ad ve soyad
    - E-posta adresi
    - Yaş veya yaş aralığı
    - Cinsiyet
    - Eğitim düzeyi
    - İlgi alanları (birden fazla seçilebilir)
    - Açık uçlu bir soru için metin alanı

### Örnek Kod

```html
<!DOCTYPE html>
<html lang="tr">
<head>
    <meta charset="UTF-8">
    <title>Öğrenci İlgi Anketi</title>
</head>
<body>
    <h1>Öğrenci İlgi Anketi</h1>
    <p>Lütfen aşağıdaki soruları cevaplayarak ilgi alanlarınız hakkında bilgi veriniz.</p>
    
    <form action="tesekkurler.html" method="get">
        <!-- Kişisel Bilgiler -->
        <h2>Kişisel Bilgiler</h2>
        
        <label for="ad">Adınız:</label>
        <input type="text" id="ad" name="ad" required><br><br>
        
        <label for="soyad">Soyadınız:</label>
        <input type="text" id="soyad" name="soyad" required><br><br>
        
        <label for="email">E-posta Adresiniz:</label>
        <input type="email" id="email" name="email" required><br><br>
        
        <!-- Yaş Aralığı -->
        <h2>Yaş Aralığınız</h2>
        <input type="radio" id="yas1" name="yas" value="10-13">
        <label for="yas1">10-13</label><br>
        
        <input type="radio" id="yas2" name="yas" value="14-17">
        <label for="yas2">14-17</label><br>
        
        <input type="radio" id="yas3" name="yas" value="18-21">
        <label for="yas3">18-21</label><br><br>
        
        <!-- Cinsiyet -->
        <h2>Cinsiyetiniz</h2>
        <input type="radio" id="kadin" name="cinsiyet" value="kadin">
        <label for="kadin">Kadın</label><br>
        
        <input type="radio" id="erkek" name="cinsiyet" value="erkek">
        <label for="erkek">Erkek</label><br>
        
        <input type="radio" id="belirtmek-istemiyorum" name="cinsiyet" value="belirtmek-istemiyorum">
        <label for="belirtmek-istemiyorum">Belirtmek istemiyorum</label><br><br>
        
        <!-- Eğitim Düzeyi -->
        <h2>Eğitim Düzeyiniz</h2>
        <select id="egitim" name="egitim">
            <option value="ilkokul">İlkokul</option>
            <option value="ortaokul">Ortaokul</option>
            <option value="lise">Lise</option>
            <option value="universite">Üniversite</option>
        </select><br><br>
        
        <!-- İlgi Alanları -->
        <h2>İlgi Alanlarınız</h2>
        <input type="checkbox" id="spor" name="ilgi" value="spor">
        <label for="spor">Spor</label><br>
        
        <input type="checkbox" id="muzik" name="ilgi" value="muzik">
        <label for="muzik">Müzik</label><br>
        
        <input type="checkbox" id="teknoloji" name="ilgi" value="teknoloji">
        <label for="teknoloji">Teknoloji</label><br>
        
        <input type="checkbox" id="sanat" name="ilgi" value="sanat">
        <label for="sanat">Sanat</label><br>
        
        <input type="checkbox" id="bilim" name="ilgi" value="bilim">
        <label for="bilim">Bilim</label><br><br>
        
        <!-- Açık Uçlu Soru -->
        <h2>Gelecekte hangi mesleği yapmak istiyorsunuz?</h2>
        <textarea id="meslek" name="meslek" rows="4" cols="50"></textarea><br><br>
        
        <!-- Gönder Butonu -->
        <button type="submit">Anketi Gönder</button>
    </form>
</body>
</html>
```


### İpuçları

- Form elemanlarını düzenli ve anlaşılır bir şekilde yerleştirin.
- Her form elemanı için açıklayıcı etiketler (`<label>`) kullanın.
- Gerekli alanları `required` özelliği ile işaretleyin.


## Yardımcı Kaynaklar

- [W3Schools HTML Tutorial](https://www.w3schools.com/html/)
- [MDN Web Docs - HTML](https://developer.mozilla.org/en-US/docs/Web/HTML)
- [HTML Form Elements](https://www.w3schools.com/html/html_form_elements.asp)

