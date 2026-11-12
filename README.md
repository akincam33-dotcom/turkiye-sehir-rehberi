# Türkiye Şehir Rehberi

Türkiye'nin 15 şehri için gezilecek yerleri, yöresel lezzetleri, doğasını ve tarihini tanıtan çok sayfalı bir web sitesi. Herhangi bir kütüphane veya framework kullanılmadan, saf HTML, CSS ve JavaScript ile geliştirilmiştir.

**Canlı demo:** https://akincam33-dotcom.github.io/turkiye-sehir-rehberi/

![Ana sayfa](docs/ana-sayfa.jpg)

## Özellikler

- **15 şehir sayfası:** Ankara, İzmir, İstanbul, Antalya, Trabzon, Nevşehir, Erzurum, Edirne, Gaziantep, Hatay, Çanakkale, Eskişehir, Ordu, Şanlıurfa, Samsun
- **Fotoğraf slider'ı (carousel):** Her sayfada "Gezilecek Yerler" ve "Yenecekler" için ileri/geri oklarla gezilebilen görsel şeridi
- **Bilgi pencereleri (modal):** Bir görsele tıklandığında o yer veya yemek hakkında açıklama açılır; dışına tıklayınca kapanır
- **Karanlık / aydınlık mod:** `prefers-color-scheme` ile kullanıcının sistem temasına otomatik uyum
- **Mobil uyumlu:** CSS Grid ile ekran boyutuna göre yeniden dizilen kart düzeni
- **Google Maps bağlantısı:** Her şehir için haritaya hızlı erişim
- **Lazy loading:** Ana sayfa görselleri `loading="lazy"` ile gerektiğinde yüklenir

![Şehir sayfası](docs/sehir-sayfasi.jpg)

## Kullanılan Teknolojiler

| Teknoloji | Kullanım amacı |
| --- | --- |
| HTML5 | Sayfa yapısı, semantik etiketler, erişilebilirlik (alt metinleri) |
| CSS3 | Grid düzeni, geçiş animasyonları, medya sorguları, karanlık mod |
| JavaScript (ES6) | Slider kontrolü, modal açma/kapama, DOM manipülasyonu |

## Proje Yapısı

```
turkiye-sehir-rehberi/
├── index.html          # Ana sayfa – şehir kartları
├── ankara.html         # Şehir sayfaları (15 adet)
├── izmir.html
├── ...
├── fotograflar/        # Ana sayfa kart görselleri ve arka planlar
├── gezilecekyerler/    # Şehir sayfalarındaki gezi görselleri
└── yemekler/           # Yöresel lezzet görselleri
```

## Çalıştırma

Projenin herhangi bir kuruluma ihtiyacı yoktur:

1. Depoyu indirin veya klonlayın: `git clone https://github.com/akincam33-dotcom/turkiye-sehir-rehberi.git`
2. `index.html` dosyasını tarayıcıda açın.

## Öğrendiklerim

- `data-*` özniteliği ile her slider'ın kendi durumunu (aktif slayt) HTML üzerinde tutmak
- Olay yayılımını (`event.stopPropagation`) kullanarak modal'ın yalnızca dışına tıklandığında kapanmasını sağlamak
- `prefers-color-scheme` medya sorgusu ile tek CSS dosyasında iki tema yönetmek
- CSS Grid'in `auto-fill` ve `minmax` ile ekran boyutuna göre esnek kart düzeni kurmak

## Geliştirici

**Akın Çam** – Ordu Üniversitesi, Bilgisayar Programcılığı
[LinkedIn](https://www.linkedin.com/in/ak%C4%B1n-%C3%A7am-73a9aa406) · [GitHub](https://github.com/akincam33-dotcom)

---
Bu proje okul projesi kapsamında hazırlanmıştır. Görseller ve metinler bilgilendirme amaçlıdır.
