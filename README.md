# 📿 Zikirmatik

<p align="center">
  <img src="screenshots/logo.png" width="120" alt="SFA Logo" style="border-radius:50%"/>
</p>

<p align="center">
  <strong>Dijital tesbihiniz her zaman yanınızda.</strong><br>
  Hedef belirleyin, zikrinizi yazın ve saymaya başlayın.
</p>

---

## ✨ Özellikler

### 📿 Sayaç
- Büyük dokunmatik butonla zikir sayma
- Hedef belirleme (33, 99, 100, 500, 1000 veya sınırsız)
- Dairesel ilerleme halkası
- Hedefe ulaşınca otomatik kayıt ve sıfırlama
- Titreşim desteği
- Manuel metin girişi (çok satır destekli)

### 🌟 Görüntü
- Yazılan zikir büyük altın harflerle ekranda parlar
- Ekranın herhangi bir yerine dokunarak sayma
- Dokunma noktasında dalga efekti
- Telefonunuzu önünüze koyup odaklanarak ibadet edin

### 📖 Kütüphane
- **Sureler:** İhlas, Fatiha, Ayetel Kürsi, Felak, Nas
- **Tesbihler:** Sübhanallah, Elhamdülillah, Allahu Ekber ve daha fazlası
- **Dualar:** İstiğfar, Besmele, Hasbünallah, Rabbenâ Duası
- **Salavat:** Salavat-ı Şerife
- **Esmâül Hüsnâ:** Yâ Allah, Yâ Şâfî, Yâ Rezzâk, Yâ Latîf ve daha fazlası
- Arama özelliği
- Tek dokunuşla sayaca ekleme

### 📊 Geçmiş
- Otomatik oturum kaydetme (hedefe ulaşma, sıfırlama, uygulama kapatma)
- Günlere göre gruplanmış kayıt listesi
- İstatistik kartları (bugünkü, toplam, oturum sayısı)
- Geçmişi temizleme

### 🎨 Tasarım
- Koyu lacivert/altın/teal renk teması
- SFA markalı splash screen
- Parçacık animasyonları
- Sayfalar arası kaydırma (swipe) desteği
- Mobil uyumlu (safe area desteği)

---

## 🚀 Kullanım

### Tarayıcıda Açma
`www/index.html` dosyasını herhangi bir tarayıcıda açın.

### Masaüstü Uygulaması Olarak Kurma
1. Chrome veya Edge ile `www/index.html` dosyasını açın
2. **Chrome:** ⋮ → Diğer araçlar → Kısayol oluştur → "Pencere olarak aç" işaretle
3. **Edge:** ⋮ → Uygulamalar → Bu siteyi uygulama olarak yükle

### APK Oluşturma (Android)

#### Gereksinimler
- [Node.js](https://nodejs.org) (LTS)
- [Android Studio](https://developer.android.com/studio)

#### Adımlar

```bash
# 1. Projeyi klonla
git clone https://github.com/KULLANICI_ADIN/zikirmatik.git
cd zikirmatik

# 2. Bağımlılıkları kur
npm init -y
npm install @capacitor/core @capacitor/cli @capacitor/android

# 3. Capacitor'ı başlat
npx cap init Zikirmatik com.sfa.zikirmatik --web-dir www

# 4. Android platformunu ekle
npx cap add android
npx cap sync

# 5. Android Studio'da aç
npx cap open android
```

Android Studio'da:
1. **Build** → **Build Bundle(s) / APK(s)** → **Build APK(s)**
2. APK dosyası: `android/app/build/outputs/apk/debug/app-debug.apk`

#### Uygulama İkonu
Android Studio'da: **Resource Manager** → **+** → **Image Asset** → `screenshots/logo.png` seçin.

#### Durum Çubuğu Rengi
`android/app/src/main/res/values/styles.xml`:
```xml
<item name="colorPrimaryDark">#1a1a1a</item>
```

---

## 📁 Proje Yapısı

```
zikirmatik/
├── www/
│   ├── index.html      # Ana uygulama dosyası
│   └── logo.png        # SFA logosu
├── screenshots/
│   └── logo.png        # README için logo
├── README.md
├── LICENSE
└── .gitignore
```

---

## 📄 Lisans

Bu proje [MIT Lisansı](LICENSE) ile lisanslanmıştır.

---

<p align="center">
  <strong>SFA</strong> tarafından ❤️ ile yapıldı
</p>
