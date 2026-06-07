# Screen Translate - Web Site Projesi

## 📱 Proje Bilgileri

**Uygulama Adı:** Screen Translate
**Geliştirici:** AURSAL
**Platform:** Android
**Package ID:** com.esarikaya.screentranslate
**Mevcut Sürüm:** 3.0.0 (Build 50)
**Google Play Store:** https://play.google.com/store/apps/details?id=com.esarikaya.screentranslate

## 🌐 Web Site Yapısı

Bu web site, Screen Translate Android uygulaması için hazırlanmış resmi tanıtım sitesidir.

### 📄 Sayfa Yapısı

```
web sayfası/
├── index.html              # Ana sayfa (Türkçe)
├── hakkimizda.html         # Hakkımızda sayfası
├── kullanici-sozlesmesi.html # Kullanıcı Sözleşmesi
├── gizlilik-politikasi.html  # Gizlilik Politikası
└── README.md               # Bu dosya
```

### 🎨 Tasarım Özellikleri

- **Responsive Design:** Mobil ve masaüstü uyumlu
- **Modern UI:** Gradient arka planlar, cam efekti
- **Interactive Elements:** Hover efektleri, smooth scrolling
- **Professional Typography:** Segoe UI font family
- **Color Scheme:** Ana renk: #667eea - #764ba2 gradient

## 🚀 Uygulama Özellikleri

### 📊 Dil Desteği
- **OCR Kaynak Dilleri:** 50 dil
  - European: English, Spanish, French, German, Italian, Portuguese, Turkish
  - Asian: Chinese, Japanese, Korean, Thai, Vietnamese, Indonesian, Hindi, Bengali
  - Middle Eastern: Arabic, Persian, Urdu, Hebrew
  - Slavic: Russian, Ukrainian, Polish, Czech, Bulgarian, Croatian, Slovak, Serbian, Lithuanian
  - Nordic: Danish, Norwegian, Finnish, Swedish
  - Other: Tamil, Nepali, Sinhala, Burmese, Khmer, Lao, Mongolian
  - Regional: Catalan, Afrikaans, Tagalog, Kazakh, Azerbaijani

- **Çeviri Hedef Dilleri:** 50+ dil
  - Tüm OCR dilleri + Greek, Dutch, Malay, Hungarian, Romanian, Swahili
  - ve daha fazlası

### 🛡️ Teknik Özellikler
- **Minimum Android:** 6.0 (API 23)
- **Compile SDK:** API 36
- **Hedef Android:** 16 (API 36)
- **Mimari Desteği:** ARM64-v8a, ARMv7, x86_64
- **16KB Alignment:** Android 15 ve 16 için optimize
- **OCR Engine:** Google ML Kit
- **AI Framework:** TensorFlow Lite GPU

### 🔒 Gizlilik Özellikleri
- **3 Çeviri Motoru:** Gemini AI (premium), Google Cloud (hızlı), ML Kit (tamamen çevrimdışı)
- **2 OCR Seçeneği:** ML Kit OCR (yerel) veya Cloud Vision OCR (bulut)
- **Kullanıcı Kontrolü:** OCR ve çeviri motorunu kendiniz seçin
- **Çeviri Metinleri Saklanmaz:** Çeviriler kayıt altına alınmaz
- **AdMob Reklam:** Reklam ID ve teknik veriler toplanır
- **Hassas Veri Koruması:** Otomatik filtreleme
- **ML Kit Offline Seçeneği:** Veriler cihazınızdan hiç çıkmaz (tam gizlilik)

## 🔧 Teknik Altyapı

### 📱 Android Bileşenleri
```kotlin
// Ana izinler
SYSTEM_ALERT_WINDOW         // Overlay arayüzü
FOREGROUND_SERVICE          // Arka plan hizmeti
MEDIA_PROJECTION            // Ekran yakalama
POST_NOTIFICATIONS          // Bildirimler
INTERNET                    // API erişimi (isteğe bağlı)
WAKE_LOCK                   // Android 15 uyumluluğu
```

### 🏗️ Geliştirme Teknolojileri
- **Dil:** Kotlin
- **UI Framework:** Jetpack Compose + View Binding
- **Build Tool:** Gradle with Kotlin DSL
- **Min/Compile/Target SDK:** 23/36/36
- **Architecture:** MVVM pattern

## 📈 Performans Optimizasyonları

### 🚀 Android 15 Hazırlığı
- 16KB page alignment desteği
- Modern packaging (useLegacyPackaging = false)
- Native library optimizasyonları
- APK boyut optimizasyonu

### ⚡ Runtime Optimizasyonları
- GPU accelerated processing
- Memory leak prevention
- Proguard/R8 obfuscation
- Debug symbol stripping

## 📋 İçerik Yapısı

### 🏠 Ana Sayfa (index.html)
- Hero section dengan CTA buttons
- 6 temel özellik kartı
- Dil desteği istatistikleri
- Teknik özellikler grid
- Download section

### ℹ️ Hakkımızda (hakkimizda.html)
- Şirket hikayesi ve misyon
- Geliştirme timeline'ı (2023-2024)
- Ekip ve roller
- Teknik mükemmellik vurgusu

### 📋 Kullanıcı Sözleşmesi (kullanici-sozlesmesi.html)
- 10 ana bölüm hukuki madde
- Android özel kullanım koşulları
- OCR ve çeviri hizmet şartları
- Sorumluluk sınırları

### 🛡️ Gizlilik Politikası (gizlilik-politikasi.html)
- KVKK/GDPR uyumlu
- 8 detaylı gizlilik bölümü
- Interactive privacy features
- Veri işleme tabloları

## 🔗 Dış Linkler

- **Google Play Store:** https://play.google.com/store/apps/details?id=com.esarikaya.screentranslate
- **Ana Site:** index.html
- **Legal Pages:** Kullanıcı sözleşmesi ve gizlilik politikası

## 📱 Mobile Responsiveness

### 📐 Breakpoints
- **Desktop:** 1200px+
- **Tablet:** 768px - 1199px  
- **Mobile:** < 768px

### 🎯 Mobile Optimizations
- Collapsed navigation menu
- Stacked card layouts
- Touch-friendly buttons (44px min)
- Optimized font sizes
- Compressed images

## 🎨 Brand Guidelines

### 🎨 Color Palette
```css
Primary Gradient: linear-gradient(135deg, #667eea 0%, #764ba2 100%)
Secondary: #ff6b6b (CTA buttons)
Success: #28a745
Warning: #ffeaa7
Text Primary: #333
Text Secondary: #666
Background: #f8f9fa
```

### 📝 Typography
- **Primary Font:** 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif
- **Heading Sizes:** 3.5rem (h1) → 1.2rem (h6)
- **Line Height:** 1.6-1.8
- **Font Weights:** 300, 500, 600, 700, 800

## 📊 SEO & Metadata

### 🔍 SEO Elements
- Semantic HTML structure
- Meta descriptions
- Open Graph tags (can be added)
- Structured data markup (can be added)
- Alt texts for images

### 🌐 Language & Localization
- **Primary Language:** Turkish (tr)
- **Alt Languages:** Can be extended
- **Direction:** LTR
- **Character Set:** UTF-8

## 🚀 Deployment Notları

### 📦 File Structure Ready
- All files self-contained
- No external dependencies
- Can be deployed to any web server
- CDN ready (no local assets dependencies)

### 🔧 Web Server Requirements
- **Minimum:** Static file hosting
- **Recommended:** HTTPS support
- **Optional:** Gzip compression
- **Optional:** CDN integration

---

**Son Güncellenme:** 28 Mart 2026
**Web Site Sürümü:** 2.2
**Uygulama Sürümü:** 3.0.0 (Build 50)
**Geliştirici:** AURSAL

*Bu web site Screen Translate Android uygulaması için hazırlanmıştır.*