# EarTrumpet

> Microsoft Store Community Choice Awards 2022 Kazananı
> 
> 
> Windows için En İyi Ses Kontrol Uygulaması
> 

# 🎯 Genel Bakış

**EarTrumpet**, Windows işletim sistemi için geliştirilmiş gelişmiş ses kontrol uygulamasıdır. Windows’un varsayılan ses karıştırıcısının sunduğu sınırlı özellikler yerine, her uygulama için ayrı ses kontrolü ve gelişmiş ses yönetimi sunar.

# ✨ Özellikler

## 🎚️ Ses Kontrolü

### Uygulama Başına Ses Kontrolü

Her çalışan uygulamanın ses seviyesini bağımsız olarak kontrol edebilme:

- 🎮 **Steam oyunları**
- 🎵 **Spotify/iTunes/YouTube Music**
- 💬 **Discord/Teams/Skype**
- 🌐 **Web tarayıcıları**
- 📺 **VLC/Media Player**
- 🔔 **Sistem bildirimleri**

### Çok Kanallı Ses Görselleştirme

- 🔵 Peak level indicators
- 📈 Real-time waveforms
- 🌈 Color-coded levels
- 📊 Multi-channel display

### Gelişmiş Ses Karışımı

- ⚡ Düşük gecikme (<10ms)
- 🎯 Hassas seviye kontrolü
- 🔄 Gerçek zamanlı güncelleme
- 💾 Ayar hafızası

## 🔄 Cihaz Yönetimi

### Dinamik Cihaz Değişimi

- 🎧 Kulaklıktan hoparlöre geçiş
- 📺 HDMI TV’ye ses yönlendirme
- 🔊 Bluetooth hoparlör bağlantısı
- 🎙️ USB mikrofon değişimi

### Varsayılan Cihaz Yönetimi

- 🎧 Kulaklık Profili
- 🔊 Masaüstü Profili
- 📺 TV/Projeksiyon Profili
- 🎙️ Podcast/Streaming Profili

## 🎨 Arayüz

### Tema Desteği

- 🌙 **Dark Mode** (Koyu tema)
- ☀️ **Light Mode** (Açık tema)
- 🔄 **System Theme** (Otomatik)
- 🎨 **Accent Colors** (Vurgu renkleri)

### Modern Kullanıcı Arayüzü

- 📊 Görsel ses çubukları
- 🎛️ Hassas ayar sliderları
- 🎯 Bağlam menüleri
- 🔄 Drag & drop desteği
- ⌨️ Klavye kısayolları

### Sistem Tepsisi Entegrasyonu

- 👆 Sol tık → Ana pencere açma
- 👆 Sağ tık → Bağlam menüsü
- 🖱️ Scroll → Ana ses kontrolü
- 🎯 Hover → Hızlı bilgi görüntüleme

# 📦 Kurulum

## 🏪 Microsoft Store (Önerilen)

**Avantajları:**
- ✅ Otomatik güncellemeler
- ✅ Güvenli kurulum
- ✅ Kolay kaldırma
- ✅ Windows ile tam entegrasyon

**Kurulum Adımları:**
1. Microsoft Store’u açın
2. “EarTrumpet” aratın
3. File-New-Project tarafından geliştirilmiş olanı seçin
4. “Get” veya “Install” butonuna tıklayın

**Direkt Link:** [Microsoft Store’dan İndir](https://www.microsoft.com/store/productId/9NBLGGH516XP)

## 💻 Windows Package Manager (winget)

```bash
# Kurulum
winget install File-New-Project.EarTrumpet

# Güncelleme
winget upgrade File-New-Project.EarTrumpet
```

## 🍫 Chocolatey

```bash
# Kurulum
choco install eartrumpet

# Güncelleme
choco upgrade eartrumpet -y
```

# ⚙️ Konfigürasyon

### 🔧 Temel Ayarlar

1. **Sistem tepsisindeki EarTrumpet simgesine sağ tıklayın**
2. **“Settings” seçeneğini seçin**
3. **Temel ayarları yapılandırın:**

### 🎚️ Ses Kontrolü Ayarları

### Uygulama Başına Ses Kontrolü

1. EarTrumpet ana penceresini açın
2. Her uygulamanın ses çubuğunu ayrı ayrı ayarlayın
3. Sağ tıklayarak uygulama özel ayarlarına erişin

### Cihaz Yönetimi

```
🔊 Çıkış Cihazları
├── 🎧 Kulaklık (Varsayılan)
├── 🔊 Hoparlörler
└── 📺 HDMI TV

🎤 Giriş Cihazları
├── 🎙️ Mikrofon (Varsayılan)
└── 🎧 Kulaklık Mikrofonu
```

# 🔍 Sorun Giderme

### ❌ Yaygın Sorunlar ve Çözümleri

### EarTrumpet Açılmıyor

```
🔧 Çözüm Adımları:
1. Windows'u yeniden başlatın
2. Microsoft Store'dan güncelleyin
3. Windows Audio Service kontrolü:
   - services.msc açın
   - Windows Audio servisini bulun
   - Yeniden başlatın
4. Uyumluluk modunda çalıştırın
```

### Ses Kontrolü Çalışmıyor

```
🔧 Çözüm Adımları:
1. Windows ses ayarlarını kontrol edin
2. Ses sürücülerini güncelleyin
3. Yönetici olarak çalıştırın
4. Ses hizmetlerini yeniden başlatın
5. Çakışan ses yazılımları kapatın
```

### Hotkey’ler Yanıt Vermiyor

```
🔧 Çözüm Adımları:
1. Ayarlardan hotkey'leri yeniden tanımlayın
2. Çakışan uygulamaları kontrol edin
3. Windows güncellemelerini yükleyin
4. EarTrumpet'i yeniden başlatın
```

### Tam Yeniden Kurulum

```bash
# winget ile kaldırma
winget uninstall File-New-Project.EarTrumpet

# Registry temizliği
reg delete HKEY_CURRENT_USER\Software\EarTrumpet /f

# Yeniden kurulum
winget install File-New-Project.EarTrumpet
```

---

> ⚠️ Not: Bu uygulama, Windows ses yönetimini tamamen dönüştüren ve Microsoft Store Community Choice Awards kazanan bir projedir. Gelişmiş ses kontrolü ihtiyacınız varsa kesinlikle denemeye değer!
>