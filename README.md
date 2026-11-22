# 🌍 Deprem Radar - Canlı ve Geçmiş Deprem Takip Sistemi (Mobil Android)

[![Build Android APK (High Performance)](https://github.com/said19605353gemini-cell/DepremAppMobile/actions/workflows/build-apk.yml/badge.svg)](https://github.com/said19605353gemini-cell/DepremAppMobile/actions/workflows/build-apk.yml)
[![GitHub Release](https://img.shields.io/github/v/release/said19605353gemini-cell/DepremAppMobile?color=blue&label=Son%20S%C3%BCr%C3%BCm)](https://github.com/said19605353gemini-cell/DepremAppMobile/releases)

Türkiye ve tüm dünyadaki sismik aktiviteleri anlık olarak takip eden, kullanıcı dostu mobil arayüze ve yüksek performanslı harita desteğine sahip Android uygulaması.

---

## 📱 Ekran Görüntüleri ve Tasarım Standartları
- **Modern Mobil Arayüz**: `DepremAppMobile` native standartlarında hazırlanmış koyu tema (`#0B1120`).
- **Genişletilmiş Filtreler**: 24 Saat, 3 Gün, 7 Gün, 15 Gün, 30 Gün, 90 Gün, 1 Sene, 3 Sene, 5 Sene ve 10 Sene seçenekleri.
- **Kesintisiz Karanlık Harita**: Esri ArcGIS World Dark Gray altyapısıyla 403 ve API anahtarı hatası olmadan akıcı harita deneyimi.
- **Çift Saat ve Tarih Şeridi**: Hem Türkiye Saati (TSİ) hem de yerel saat desteği, net gün.ay.yıl formatı.
- **Akordiyon Bilgi Kartları**: Depremin derinliği, koordinatları, merkez üssü ve kaynak kurumu detayları.

---

## 📡 Veri Kaynakları
- 🇹🇷 **AFAD** (Afet ve Acil Durum Yönetimi Başkanlığı)
- 🇹🇷 **Kandilli Rasathanesi** (Boğaziçi Üniversitesi KRDAE)
- 🌍 **USGS** (United States Geological Survey - Küresel Depremler)
- 🇪🇺 **EMSC** (European-Mediterranean Seismological Centre)

---

## ⚡ Derleme & Kurulum

### Hazır APK İndir
En son kararlı sürümü doğrudan telefonunuza indirip kurmak için [**Releases Sayfası**](https://github.com/said19605353gemini-cell/DepremAppMobile/releases)'na gidin ve `app-debug.apk` dosyasını indirin.

### Kaynak Koddan Derleme (Geliştiriciler İçin)
```bash
# Bağımlılıkları yükleyin
npm install

# Android katmanını senkronize edin
npx cap sync android

# Gradle ile 4 çekirdekli hızlı derleme
cd android
./gradlew assembleDebug --parallel --build-cache --max-workers=4
```
