# 🎨 [Digital Art Collection](https://talha-uk.github.io/digital-art-collection/collection.html)

Modern ve interaktif bir dijital sanat galerisi. Midjourney tarzı detay görünümü ile sanat eserlerinizi profesyonel bir şekilde sergileyin.

![Digital Art Collection](https://img.shields.io/badge/Version-1.0.0-blue.svg)
![HTML5](https://img.shields.io/badge/HTML5-E34F26?logo=html5&logoColor=white)
![CSS3](https://img.shields.io/badge/CSS3-1572B6?logo=css3&logoColor=white)
![JavaScript](https://img.shields.io/badge/JavaScript-F7DF1E?logo=javascript&logoColor=black)

## ✨ Özellikler

### 🖼️ **Gelişmiş Galeri Sistemi**
- **Masonry Layout**: Pinterest tarzı esnek grid düzeni
- **Lazy Loading**: Performans optimizasyonu için gecikmeli yükleme
- **Responsive Design**: Tüm cihazlarda mükemmel görünüm
- **Hover Efektleri**: Interaktif görsel deneyim

### 🎯 **Midjourney Tarzı Detay Görünümü**
- **Üç Bölümlü Layout**: Sol (büyük resim), orta (bilgiler), sağ (thumbnail galeri)
- **Smooth Navigasyon**: Klavye, mouse wheel ve thumbnail desteği
- **Etiket Sistemi**: Her resim için özelleştirilebilir etiketler
- **Modal Interface**: Tam ekran detay deneyimi

### 🔍 **Akıllı Filtreleme**
- **Kategori Filtreleri**: Pokemon, Anime, Art, Photography, Cyberpunk, Nature
- **Dinamik Sayaçlar**: Anlık resim istatistikleri
- **Smooth Geçişler**: Animasyonlu filtre değişimleri

### 🎮 **Gelişmiş Kontroller**
- **Klavye Navigasyonu**: ← → ok tuşları, ESC ile çıkış
- **Mouse Wheel**: Ana resim üzerinde scroll ile geçiş
- **Touch Support**: Mobil cihazlar için optimize edilmiş
- **Auto-scroll**: Aktif thumbnail otomatik ortalama

## 🚀 Kurulum

### Hızlı Başlangıç

1. **Projeyi klonlayın:**
```bash
git clone https://github.com/kullaniciadi/digital-art-collection.git
cd digital-art-collection
```

2. **Resimlerinizi ekleyin:**
```
img/
├── resim1.jpg
├── resim2.png
└── ...
```

3. **Tarayıcıda açın:**
```bash
# Basit HTTP sunucusu ile
python -m http.server 8000
# veya
npx serve .
```

4. **http://localhost:8000** adresine gidin

## 📁 Proje Yapısı

```
digital-art-collection/
├── 📄 collection.html      # Ana HTML dosyası
├── 📁 img/                 # Resim klasörü
│   ├── resim1.jpg
│   ├── resim2.png
│   └── ...
└── 📄 README.md           # Bu dosya

```

## ⚙️ Konfigürasyon

### Resim Bilgilerini Özelleştirme

`collection.html` dosyasındaki `imageConfig` objesini düzenleyerek resim bilgilerini özelleştirebilirsiniz:

```javascript
const imageConfig = {
    'resim-adi.jpg': {
        title: 'Resim Başlığı',
        description: 'Detaylı açıklama...',
        category: 'art', // art, photography, concept, cyberpunk, nature, pokemon, anime
        tags: ['etiket1', 'etiket2', 'etiket3']
    }
};
```

### Kategori Ekleme

Yeni kategoriler eklemek için:

1. **HTML'de filtre butonu ekleyin:**
```html
<button class="filter-btn" data-filter="yeni-kategori">Yeni Kategori</button>
```

2. **CSS'de kategori rengini tanımlayın** (isteğe bağlı)

3. **JavaScript'te imageConfig'e kategoriyi ekleyin**

## 🎨 Özelleştirme

### Renk Teması Değiştirme

CSS değişkenlerini düzenleyerek renk temasını özelleştirebilirsiniz:

```css
:root {
    --primary-color: #0ff;      /* Ana renk */
    --secondary-color: #ff0066; /* İkincil renk */
    --bg-color: #0a0a0a;        /* Arka plan */
    --text-color: #fff;         /* Metin rengi */
}
```

### Layout Ayarları

```css
.gallery {
    column-count: 4;        /* Kolon sayısı (desktop) */
    column-gap: 20px;       /* Kolon arası boşluk */
}

@media (max-width: 768px) {
    .gallery {
        column-count: 2;    /* Mobilde kolon sayısı */
    }
}
```

## 📱 Responsive Tasarım

- **Desktop**: 5 kolon masonry layout
- **Tablet**: 4 kolon layout
- **Mobil**: 2 kolon layout
- **Küçük ekranlar**: 1 kolon layout

## 🔧 Teknik Detaylar

### Kullanılan Teknolojiler
- **HTML5**: Semantic markup
- **CSS3**: Flexbox, Grid, Animations, Media Queries
- **Vanilla JavaScript**: ES6+ özellikleri
- **CSS Variables**: Dinamik tema desteği

### Performans Optimizasyonları
- **Lazy Loading**: Görünür olmayan resimler gecikmeli yüklenir
- **CSS Animations**: GPU hızlandırmalı animasyonlar
- **Efficient DOM Manipulation**: Minimal DOM güncellemeleri
- **Image Optimization**: WebP desteği hazır

### Tarayıcı Desteği
- ✅ Chrome 60+
- ✅ Firefox 55+
- ✅ Safari 12+
- ✅ Edge 79+

## 🤝 Katkıda Bulunma

1. **Fork** edin
2. **Feature branch** oluşturun (`git checkout -b feature/amazing-feature`)
3. **Commit** edin (`git commit -m 'Add amazing feature'`)
4. **Push** edin (`git push origin feature/amazing-feature`)
5. **Pull Request** açın

## 📝 Lisans

Bu proje MIT lisansı altında lisanslanmıştır. 
Kodu veya tasarımı özgürce kullanabilir, düzenleyebilir ve paylaşabilirsiniz.
Ancak lütfen orijinal projeye atıfta bulunun. 🙏

## 🙏 Teşekkürler

- **Midjourney** - UI/UX ilhamı için
- **Unsplash** - Örnek resimler için
- **CSS Grid** ve **Flexbox** - Modern layout teknolojileri

## 📞 İletişim

- **GitHub**: [@talha-uk](https://github.com/talha-uk)
- **Email**: talhaubeyd51@gmail.com
- **Website**: [Canlı Site](https://talha-uk.github.io/digital-art-collection/collection.html)

---

⭐ **Bu projeyi beğendiyseniz yıldız vermeyi unutmayın!**

## 🔄 Güncellemeler

### v1.0.0 (2024-12-XX)
- ✨ İlk sürüm yayınlandı
- 🎨 Midjourney tarzı detay görünümü
- 📱 Tam responsive tasarım
- 🔍 Gelişmiş filtreleme sistemi
- ⚡ Performans optimizasyonları

## 🔄 Planlanan Güncellemeler

### v1.1.0 (2025)
- 🎨 Kullanıcıların resim yükleme sistemi 
- 📱 Kullanıcı tabanlı Yorum ve Değerlendirme özelliği
---

<div align="center">
  <img src="https://img.shields.io/badge/Made%20with-❤️-red.svg"/>
  <img src="https://img.shields.io/badge/Built%20with-HTML%20CSS%20JS-blue.svg"/>
</div>
