# ⚡ Deprem Radar - Canlı & Geçmiş Deprem Takip Uygulaması (Android APK & Web)

<p align="center">
  <img src="icon.svg" width="120" height="120" alt="Deprem Radar Logo" />
  <br>
  <b>Türkiye ve Dünya Geneli Canlı & Geçmiş Sismik Hareket Takip Radarı</b>
  <br>
  <i>Tüm Android telefonlarla ve modern tarayıcılarla %100 uyumludur.</i>
</p>

<p align="center">
  <a href="https://github.com/said19605353gemini-cell/DepremAppMobile/releases"><img src="https://img.shields.io/github/v/release/said19605353gemini-cell/DepremAppMobile?style=for-the-badge&color=blue" alt="Release"></a>
  <a href="https://github.com/said19605353gemini-cell/DepremAppMobile/actions"><img src="https://img.shields.io/github/actions/workflow/status/said19605353gemini-cell/DepremAppMobile/build-apk.yml?style=for-the-badge&label=Build%20APK" alt="Build Status"></a>
  <img src="https://img.shields.io/badge/Lisans-MIT-green?style=for-the-badge" alt="License">
</p>

---

## 📱 Doğrudan Android APK İndir
En son kararlı sürümü doğrudan telefonunuza indirip kurabilirsiniz:
👉 **[Deprem Radar Son APK Sürümünü İndir (Releases)](https://github.com/said19605353gemini-cell/DepremAppMobile/releases)**

---

## 🌟 Öne Çıkan Özellikler

- **🌍 Çift Veri Kaynağı:**
  - **AFAD (Türkiye):** Afet ve Acil Durum Yönetimi Başkanlığı resmi açık veri servisi.
  - **USGS (Dünya Geneli):** Amerika Jeolojik Araştırmalar Kurumu global sismik akışı.
- **🕒 Çift Saat Dilimi Desteği:**
  - **Türkiye Saati (TR):** Depremin gerçekleştiği an Türkiye'de saatin kaç olduğu.
  - **Yerel Saat (Yerel):** Depremin gerçekleştiği ülkedeki (boylamına göre) gerçek yerel saat.
- **📅 Kapsamlı Tarih Filtreleme:**
  - 3 Gün, 7 Gün, 15 Gün, 30 Gün, 45 Gün
  - **1 Sene, 3 Sene, 5 Sene ve 10 Senelik** tarihsel büyük deprem arşivi.
- **📊 Gelişmiş Sıralama Ölçütleri:**
  - 🔥 **En Yüksek Şiddet:** En büyük depremden en küçüğe doğru.
  - 🌱 **En Düşük Şiddet:** Küçük sarsıntılardan yukarıya.
  - 🕒 **En Yeni ➔ Eski:** Standart canlı zaman akışı.
  - ⏳ **Eskiden ➔ Yeniye:** Geçmişten bugüne kronolojik sıralama.
- **📑 50'şerli Sayfalama (Pagination):**
  - Depremleri 50'şerli gruplara böler, sayfa numaralarıyla (`[◀] [1] [2] [3] ... [▶]`) hızlı ve kasmadan gezinme sağlar.
- **🗺️ Canlı İnteraktif Harita:**
  - Depremler büyüklüklerine göre renkli dairelerle haritada konumlanır; tıklandığında konum, derinlik ve saat balonu açılır.
- **🔍 Akıllı Arama & Akordiyon Detay:**
  - Şehir (İzmir, Malatya, Van) veya Ülke (Japan, Greece, Italy) bazlı canlı arama.
  - Karta tıklandığında açılan tam konum, koordinat ve derinlik kutusu.
- **🌑 Modern OLED Dark Mod:** Gece gözü yormayan batarya dostu arayüz.

---

## 📂 Proje Dizin Yapısı

```
DepremAppMobile/
├── .github/
│   └── workflows/
│       └── build-apk.yml     # GitHub Actions ile otomatik APK derleyici ve Release üretici
├── android/                  # Capacitor ile oluşturulmuş yerel Android Gradle projesi
├── www/                      # Mobil ve web kaynak dosyaları
│   ├── index.html            # Ana responsive arayüz, Leaflet harita ve API mantığı
│   ├── manifest.json         # PWA mobil kurulum manifestosu
│   └── icon.svg              # Vektörel radar ikonu
├── capacitor.config.json     # Mobil paketleme konfigürasyonu
├── package.json              # Bağımlılıklar (@capacitor/core, @capacitor/android)
└── README.md                 # Proje dokümantasyonu
```

---

## 🛠️ Yerel Geliştirme ve Derleme

### Web Arayüzünü Test Etme:
Herhangi bir statik sunucuyla veya doğrudan tarayıcıda `www/index.html` dosyasını açarak test edebilirsiniz.

### Yerel Android APK Derleme (Opsiyonel):
```bash
# Bağımlılıkları yükleyin
npm install

# Web varlıklarını Android projesine senkronize edin
npx cap sync android

# Android Studio ile açın:
npx cap open android
```
veya terminalden Gradle ile doğrudan derleyin:
```bash
cd android
./gradlew assembleDebug
```
*Derlenen `.apk` çıktısı `android/app/build/outputs/apk/debug/app-debug.apk` yolunda oluşur.*

---

## 📡 Veri Sağlayıcıları (Data Sources)
- [AFAD Deprem Dairesi Başkanlığı](https://deprem.afad.gov.tr/)
- [USGS Earthquake Hazards Program](https://earthquake.usgs.gov/)

---

## 📄 Lisans
Bu proje [MIT Lisansı](LICENSE) kapsamında açık kaynak olarak geliştirilmiştir.
