# Deprem Radar - Android APK ve Mobil Kurulum Rehberi

Bu proje, AFAD canlı verilerini kullanan mobil öncelikli (Mobile First) harita destekli ve modern tasarımlı deprem takip uygulamasıdır.

Uygulama dosyaları:
- **Ana Arayüz & Harita:** [index.html](file:///C:/Users/SaidNurs/.gemini/antigravity/scratch/DepremAppMobile/DepremAppMobile/index.html)
- **Manifest (PWA/Mobil):** [manifest.json](file:///C:/Users/SaidNurs/.gemini/antigravity/scratch/DepremAppMobile/DepremAppMobile/manifest.json)
- **.NET MAUI / C# Projesi:** [DepremAppMobile.csproj](file:///C:/Users/SaidNurs/.gemini/antigravity/scratch/DepremAppMobile/DepremAppMobile/DepremAppMobile.csproj)

---

## 🚀 Seçenek 1: Web2APK / PWABuilder ile Anında APK Üretme (En Hızlı & En Pratik Yol)
Yerel bilgisayarınızda GB'larca Android SDK / Android Studio indirmeye gerek kalmadan dakikalar içinde resmi imzalı APK almak için:

1. Bu klasördeki dosyaları (`index.html`, `manifest.json`) ücretsiz olarak GitHub Pages, Netlify veya Vercel'e yükleyin (veya yerel test için açın).
2. [PWABuilder.com](https://www.pwabuilder.com/) veya [Web2APK](https://websitetoapk.com/) adresine linkinizi yapıştırın.
3. **"Package for Android"** butonuna basın.
4. Sistem size doğrudan telefonunuza kurabileceğiniz `.apk` dosyasını verecektir.

---

## 🛠️ Seçenek 2: C# (.NET MAUI) ile Yerel APK Derleme
Eğer Android Studio veya .NET Android Workload ortamınız varsa doğrudan C# üzerinden APK derleyebilirsiniz:

```powershell
# 1. Android iş yükünü yükleyin:
dotnet workload install maui-android

# 2. Release APK dosyasını derleyin:
cd C:\Users\SaidNurs\.gemini\antigravity\scratch\DepremAppMobile\DepremAppMobile
dotnet publish -f net8.0-android -c Release
```
Derlenen `.apk` dosyası `bin/Release/net8.0-android/publish/` altında oluşacaktır.

---

## 📱 Seçenek 3: Android Telefona Doğrudan Yükleme (PWA)
1. Tarayıcınızda `index.html` sayfasını açın.
2. Sağ üstteki 3 noktaya tıklayıp **"Ana Ekrana Ekle"** veya **"Uygulamayı Yükle"** deyin.
3. Tıpkı bir APK gibi telefonunuzun ana ekranında bağımsız bir mobil uygulama olarak çalışacaktır.
