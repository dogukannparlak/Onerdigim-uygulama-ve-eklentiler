# Playnite

## Playnite Nedir?

**Playnite**, tüm oyun platformlarınızı tek bir arayüzde toplayan açık kaynaklı, ücretsiz oyun kütüphanesi yöneticisidir. Steam, Epic Games Store, GOG, Xbox Game Pass, PlayStation, Uplay ve daha birçok platformdan oyunlarınızı merkezi bir konumdan yönetebilirsiniz.

### Ana Avantajları:

- 🎮 **Birleşik Oyun Kütüphanesi** - Tüm platformlardan oyunları tek arayüzde
- 🎨 **Özelleştirilebilir Arayüz** - Tema desteği ve kişiselleştirme seçenekleri
- 📺 **Big Picture Mode** - TV/büyük ekranlar için tam ekran modu
- 🔄 **Otomatik Metadata** - Oyun bilgileri ve görsellerin otomatik indirilmesi
- 🆓 **Tamamen Ücretsiz** - Açık kaynaklı ve reklamsız
- 🔌 **Eklenti Desteği** - Geniş eklenti ekosistemi

### ⚡ Mimari Yaklaşım: “Simbiyotik Parazit” Modeli

**Önemli Not**: Playnite bir “değiştirici” değil, bir “ön uç” olarak işlev görür. Bu demek oluyor ki:

- ✅ **Birleşik görünüm** sağlar - tüm oyunlarınızı tek arayüzde görebilirsiniz
- ⚠️ **Orijinal başlatıcılar** hala gerekli - çoğu oyun için platform kurulu olmalı
- 🔄 **Güncelleme ve DRM** işlemleri yine orijinal başlatıcılar üzerinden
- 🎯 **Oyun başlatma** gerçek platformlar aracılığıyla yapılır

Bu “simbiyotik parazit” modelinin avantajları:
- Platform API’lerini resmi olarak kullanma
- Geniş platform desteği
- Güvenilir oyun başlatma

Dezavantajları:
- Platform değişikliklerine bağımlılık
- Başlatıcı güncellemelerinden etkilenme
- Tam bağımsızlık eksikliği

## Özellikler

### 🚀 Temel Özellikler

- **Multi-platform desteği**: 20+ oyun platformu entegrasyonu
- **Otomatik oyun tespiti**: Yüklü oyunları otomatik bulma
- **Metadata yönetimi**: IGDB, RAWG, Steam ve diğer kaynaklardan bilgi çekme
- **Filtre ve kategorileme**: Gelişmiş arama ve sıralama seçenekleri
- **İstatistik takibi**: Oyun süresi ve aktivite izleme

### 📊 Desteklenen Platformlar

| Platform | Otomatik Tespit | Metadata | Store Link |
| --- | --- | --- | --- |
| Steam ✅ | ✅ | ✅ | ✅ |
| Epic Games Store ✅ | ✅ | ✅ | ✅ |
| GOG Galaxy ✅ | ✅ | ✅ | ✅ |
| Xbox Game Pass ✅ | ✅ | ✅ | ✅ |
| MS store✅ | ❌ | ✅ | ✅ |
| PlayStation ✅ | ❌ | ✅ | ❌ |
| Ubisoft Connect ✅ | ✅ | ✅ | ✅ |
| Origin/EA App ✅ | ✅ | ✅ | ✅ |
| Battle.net ✅ | ✅ | ✅ | ✅ |
| Emülatörler ✅ | ⚙️ | ✅ | ❌ |

### 🎨 Görsel ve Kullanıcı Deneyimi

- **Grid/List görünümü**: Farklı görüntüleme seçenekleri
- **Kapak/banner görselleri**: Otomatik görsel indirme
- **Video preview**: Oyun trailerları ve gameplay videolar
- **Screenshot galerisi**: Oyun içi ekran görüntüleri
- **Metadata düzenleme**: Manuel bilgi düzenleme imkanı

## Kurulum

### 🔽 İndirme ve Kurulum

### 1️⃣ Resmi Web Sitesinden (Önerilen)

1. [playnite.link](https://playnite.link/) adresine gidin
2. “Download” butonuna tıklayın
3. **Installer** veya **Portable** sürümünü seçin:
    - **Installer**: Sistem entegrasyonu, otomatik güncellemeler
    - **Portable**: USB’de taşınabilir, sistem değişikliği yok

### 2️⃣ Winget ile Kurulum

```bash
winget install playnite.playnite
```

### 3️⃣ Chocolatey ile Kurulum

```bash
choco install playnite
```

### 4️⃣ GitHub Releases

- [GitHub Releases](https://github.com/JosefNemec/Playnite/releases) sayfasından en son sürümü indirin
- Pre-release sürümler beta özellikler içerebilir

### ⚙️ Kurulum Seçenekleri

### Installer Kurulumu:

```
✅ ÖNERİLER:
☑️ Desktop shortcut oluştur
☑️ Start Menu shortcut oluştur
☑️ File associations ekle
☑️ Playnite URI handler kaydet
```

## İlk Kurulum ve Konfigürasyon

### 🚀 İlk Çalıştırma Sihirbazı

### 1. Platform Entegrasyonu

İlk açılışta Playnite size yüklü oyun platformlarını otomatik olarak tespit eder:

```
Tespit Edilen Platformlar:
├── Steam → C:\Program Files (x86)\Steam
├── Epic Games → C:\Program Files (x86)\Epic Games
├── GOG Galaxy → C:\Program Files (x86)\GOG Galaxy
├── Xbox Game Pass → Microsoft Store
└── Ubisoft Connect → C:\Program Files (x86)\Ubisoft
```

### 2. Kütüphane Entegrasyon Ayarları

Her platform için ayrı ayarlar yapabilirsiniz:

| Platform | Oyunları İçe Aktar | Meta Veri İndir | Arka Plan İndirme |
| --- | --- | --- | --- |
| Steam | ✅ Önerilen | ✅ Otomatik | ✅ Arka plan |
| Epic Games | ✅ Önerilen | ✅ Otomatik | ✅ Arka plan |
| GOG | ✅ Önerilen | ✅ Otomatik | ✅ Arka plan |
| …. |  |  |  |

### 3. Meta Veri Kaynak Seçimi

```
Önerilen Meta Veri Kaynakları:
├── 🎮 IGDB (Birincil) → En kapsamlı veritabanı
├── 🎯 RAWG (İkincil) → Topluluk odaklı
├── 🏪 Steam Store → Mağaza bilgileri
└── 📊 ScreenScraper → Retro oyunlar için
....
```

### ⚙️ Temel Ayarlar

### Kütüphane Ayarları

```
Ayarlar → Kütüphane:
├── Meta verileri otomatik indir: ✅
├── Görselleri otomatik indir: ✅
├── Görsel indirme önceliği: Kapak → Arkaplan → İkon
└── Başlangıçta kütüphaneyi güncelle: ✅
```

## Oyun Kütüphanesi Yönetimi

### 📚 Oyun İçe Aktarma

### Otomatik İçe Aktarma

Playnite yüklü platformları tarar ve oyunları otomatik olarak ekler:

```
Kütüphane → Oyun Kütüphanesini Güncelle (Ctrl+F5)
├── Platform başlatıcı taraması
├── Kayıt defteri kontrolü
├── Yüklü oyun tespiti
└── Meta veri indirme
```

### Manuel Oyun Ekleme

```
Kütüphane → Oyun Ekle (Ctrl+Shift+A)
├── 🎮 El ile → Manuel oyun ekleme
├── 💿 Emülatör Oyunu → Emülatör oyunları
├── 📁 Klasör Tara → Dizin tarama
└── 🔗 Oyun Yükle → Platform mağazasından kurulum
```

### 🏷️ Oyun Bilgileri ve Meta Veri Yönetimi

### Meta Veri Düzenleme

Her oyun için detaylı bilgi düzenleyebilirsiniz:

```
Oyun → Sağ Tık → Düzenle (F3)
├── 📋 Genel: Ad, açıklama, çıkış tarihi
├── 🎨 Görseller: Kapak, arkaplan, ikon
├── 🏷️ Kategoriler: Tür, geliştirici, yayıncı
├── 📊 Özellikler: Çok oyunculu, başarımlar
├── 🔗 Bağlantılar: Mağaza sayfaları, web siteleri
└── ⚙️ Eylemler: Çalıştırma komutları
```

### Toplu Meta Veri İndirme

```
Kütüphane → Meta Veri İndir (Ctrl+D)
├── 🎯 Sadece eksik meta veriler
├── 🔄 Mevcut meta verileri güncelle
├── 🎨 Eksik görselleri indir
└── 📊 Oyun detaylarını güncelle
```

### 📂 Kategoriler ve Filtreler

### Kategori Yönetimi

```
📁 Varsayılan Kategoriler:
├── 🎮 Platform (Steam, Epic, GOG...)
├── 🎯 Tür (Aksiyon, RPG, Strateji...)
├── 👥 Geliştirici (Valve, CD Projekt...)
├── 📅 Çıkış Yılı (2023, 2022...)
├── ⭐ Puanlama (5 yıldız, 4 yıldız...)
└── ⏱️ Tamamlanma Durumu (Tamamlandı, Oynuyor...)
```

### Özel Kategoriler

```
Kütüphane → Kategoriler → Kategori Ekle
├── 🏆 "Favorilerim"
├── 🕐 "Oynamayı Planlıyorum"
├── 💯 "100% Tamamlananlar"
├── 👨‍👩‍👧‍👦 "Co-op Oyunlar"
└── 🎮 "Nostalji"
```

### Gelişmiş Filtreleme

```
Filtre Paneli (F2):
├── 🔍 İsim arama
├── 🎮 Platform filtresi
├── 🎯 Tür filtresi
├── ⭐ Puan filtresi
├── 📅 Çıkış tarihi aralığı
├── ⏱️ Oyun süresi filtresi
└── 🏷️ Kategori filtresi
```

## Big Picture Mode (Fullscreen Mode)

### 📺 Tam Ekran Modu Nedir?

Big Picture Mode (Büyük Resim Modu), Playnite’ın TV ve büyük ekranlar için optimize edilmiş tam ekran arayüzüdür. Gamepad ile kontrol edilmek üzere tasarlanmıştır ve oturma odası oyunculuğu deneyimi sunar.

### 🎮 Tam Ekran Modu Özellikleri

### Kontrolcü Öncelikli Tasarım

- **Gamepad navigasyonu**: Xbox, PlayStation, Steam Controller desteği
- **Buton göstergeleri**: Kontrolcü buton ipuçları
- **Dairesel menüler**: Radial menü sistemi
- **Ses komutları**: Sesli kontrol (eklenti ile)

### TV Dostu Arayüz

- **Büyük yazılar**: Uzaktan okunabilir büyük fontlar
- **Yüksek kontrast**: Görsel netlik için optimize edilmiş
- **Basitleştirilmiş navigasyon**: Sade menü yapısı
- **Otomatik gizleme**: Gerektiğinde kaybolabilen UI öğeleri

### 🚀 Tam Ekran Modu Kullanımı

### Tam Ekran Moduna Geçiş

```
🎮 Fullscreen Başlatma:
├── F11 → Masaüstü modundan tam ekrana geçiş
├── Ayarlar → Uygulama → "Başlangıçta fullscreen modu"
├── Desktop icon → "Playnite (Fullscreen)" kısayolu
└── Command line → playnite --fullscreen
```

### Gamepad Kontrolleri

```
🎮 Temel Kontrolcü Navigasyonu:
├── A/X → Seç/Oyna
├── B/Circle → Geri
├── Y/Triangle → Menü
├── X/Square → Filtrele
├── Sol Stick → Navigasyon
├── Sağ Stick → Hızlı scroll
├── LB/RB → Kategoriler arası geçiş
└── Start → Ana menü
```

### Living Room Optimizasyonu

- **TV modu ayarları**: 4K/HDR uyumluluğu
- **Uzaktan kumanda desteği**: HDMI-CEC kontrolü
- **Ses çıkışı**: 5.1/7.1 surround sound ayarları
- **Uyku modu**: Controller’dan otomatik uyku

### Başlatma Yöntemleri

```
Fullscreen Mode Başlatma:
├── 🎮 F11 tuşu → Hızlı geçiş
├── 📺 View → Enter Fullscreen Mode
├── 🕹️ Controller Guide button (uzun basış)
└── ⚙️ Launch argument: --fullscreen
```

### Controller Navigation

```
🎮 Xbox Controller Layout:
├── A Button → Seç/Onayla
├── B Button → Geri/İptal
├── X Button → Context menu
├── Y Button → Search
├── LB/RB → Kategori değiştir
├── LT/RT → Sayfa değiştir
├── D-Pad → Navigasyon
├── Left Stick → Navigasyon
├── Right Stick → Scroll
└── Guide → Ana menü
```

## Tema ve Kişiselleştirme

### 🎨 Yerleşik Temalar

### Masaüstü Modu Temaları

```
Ayarlar → Görünüm → Masaüstü Teması:
├── 🌟 Varsayılan → Standart Playnite teması
├── 🌙 Koyu → Koyu tema
├── 🌞 Açık → Açık tema
└── 🎮 Özel → Özel tema yükle
```

### Tam Ekran Modu Temaları

```
Ayarlar → Görünüm → Tam Ekran Teması:
├── 🎮 Varsayılan → Konsol tarzı arayüz
├── 🖥️ Masaüstü → Masaüstü benzeri arayüz
├── 📺 TV → Büyük ekran odaklı
└── 🕹️ Retro → Nostaljik konsol teması
```

### 🔽 Tema İndirme ve Kurulum

### Playnite Tema Veritabanı

1. [Playnite Database](https://playnite.link/database.html) sayfasına gidin
2. **Temalar** sekmesini seçin
3. Beğendiğiniz temayı indirin (.pthm dosyası)
4. `Ayarlar → Görünüm → Tema Yükle` ile kurun

### Popüler Temalar

```
🌟 Önerilen Desktop Temaları:
├── 🌙 Stardust → Modern, minimal
├── 🎮 Steam-like → Steam benzeri arayüz
├── 🌈 Aurora → Renkli, canlı
└── 🖤 Carbon → Siyah, şık

🎮 Önerilen Fullscreen Temaları:
├── 🎯 Metro → Xbox benzeri arayüz
├── 📺 Console → PlayStation benzeri
├── 🕹️ Retro → Nostaljik konsol
└── 🌌 Nebula → Futuristik tema
```

## Extensions ve Eklentiler

### 🔌 Eklenti Yönetimi

### Eklenti Kurulumu

```
Ayarlar → Eklentiler → Eklentilere Gözat:
├── 🔍 Eklenti ara
├── 📊 Popülerliğe göre sırala
├── ⭐ Puana göre filtrele
└── 📥 Tek tıkla kur
```

### Elle Eklenti Kurulumu

1. `.pext` dosyasını indirin
2. `Ayarlar → Eklentiler → Eklenti Yükle`
3. İndirilen dosyayı seçin
4. Playnite’ı yeniden başlatın

### 🌟 Kritik “Killer Feature” Eklentiler

### 💾 Ludusavi - Evrensel Bulut Kayıtları

**En Önemli Eklenti**: Oyun kayıtlarınızı evrensel olarak yedekleyen ve senkronize eden güçlü araç.

**Özellikler**:
- ✅ **Tüm oyunlar için destek** - Steam, Epic, GOG, emülatörler, DRM-free oyunlar
- ☁️ **Bulut entegrasyonu** - Google Drive, OneDrive, Dropbox ile otomatik sync
- 🔄 **Otomatik yedekleme** - Oyun başlatma/kapama sırasında otomatik kaydet
- 📦 **Batch restore** - Tüm kayıtları tek seferde geri yükleme
- 🎯 **Platform agnostik** - Hangi mağazadan alındığına bakmaksızın çalışır

### 🏆 SuccessStory + Achievement Watcher - Evrensel Başarımlar

**Başarım Takibi Kombinasyonu**: Platform sınırlarını aşan başarım sistemi.

**SuccessStory Özellikleri**:
- 📊 **Birleşik başarımlar** - Tüm platformlardan başarımları tek arayüzde görüntüleme
- 📈 **İlerleme takibi** - Başarım ilerlemesi ve tamamlanma oranları
- 🎯 **İstatistikler** - Tamamlanma oranı, en nadir başarımlar vb.
- 🔔 **Bildirimler** - Yeni başarımlar için masaüstü bildirimleri

**Achievement Watcher Entegrasyonu**:
- 🎮 **Emülatör başarımları** - RetroAchievements sistemi desteği
- 🏴‍☠️ **Platform bağımsız destek** - Tüm oyun türleri için başarım takibi
- 📱 **Gerçek zamanlı bildirimler** - Steam emülasyonu ile anlık uyarılar

### 🎬 ExtraMetadataLoader - Zengin Görsel Deneyim

**Görsel İyileştirme Paketi**: Oyun arayüzünü sinematik seviyeye çıkarır.

**Özellikler**:
- 🎥 **Video fragmanları** - Oyun detay sayfasında otomatik trailer oynatma
- 🖼️ **Logo entegrasyonu** - Temiz, profesyonel oyun logoları
- 📸 **Ek ekran görüntüleri** - Genişletilmiş galeri görünümü
- 🎨 **Gelişmiş meta veri** - Ekstra görsel içerik otomatik indirme

### 🌟 Diğer Popüler Eklentiler

### 📊 Meta Veri ve İçerik Zenginleştirme

```
🔝 Olmazsa Olmaz Eklentiler:
├── 📺 VNDB → Görsel roman veritabanı
├── 🎮 RAWG → Topluluk odaklı oyun veritabanı
├── 🏪 SteamGridDB → Özel oyun görselleri
├── 📱 MobyGames → Vintage oyun bilgileri
└── 🎯 HowLongToBeat → Oyun uzunluğu tahminleri
```

### 🎮 Oyun Deneyimi İyileştirici

```
🎯 Oynanış Eklentileri:
├── 🎮 DS4Windows Entegrasyonu → DualShock 4 desteği
├── 🔊 Ses Kontrolü → Oyun başına ses ayarları
├── 🖥️ Oyun Eylemleri → Özel başlatma/kapama scriptleri
├── ⏱️ Oyun Süresi Takipçisi → Gelişmiş oturum izleme
└── 🌟 Oyun Başlatıcısı → Gelişmiş oyun başlatma
```

### 🔗 Platform Eklentileri

```
🌐 Platform Özel:
├── 🎮 Steam Başlatıcısı → Gelişmiş Steam entegrasyonu
├── 🛒 Epic Games Başlatıcısı → Epic iyileştirmeleri
├── 🎯 GOG Başlatıcısı → GOG Galaxy alternatifi
├── 📱 Android Uygulamaları → Android oyun entegrasyonu
└── 🕹️ Emülasyon İstasyonu → Retro oyun merkezi
```

## Gelişmiş Özellikler

### 🔄 Otomatik Özellikler

### Auto-Sync ve Background Tasks

```
⚙️ Otomasyon Ayarları:
├── 🔄 Library auto-update: Startup/Periodic
├── 📥 Auto-download metadata: New games
├── 🖼️ Auto-download images: Background
├── 🎮 Auto-import new games: Real-time
└── 📊 Auto-backup library: Weekly
```

### Smart Notifications

```
🔔 Bildirim Sistemi:
├── 🆕 New games added: Toast notification
├── ⬇️ Download completed: System tray
├── 🔄 Library updated: Status bar
├── ❌ Game launch failed: Error dialog
└── 🎮 Controller connected: Auto-switch to fullscreen
```

### 📊 İstatistik ve Rapor

### Library Statistics

```
View → Library Statistics:
├── 📊 Total games: 847 games
├── 🎮 By platform: Steam (324), Epic (89)...
├── 📅 By release year: 2023 (45), 2022 (89)...
├── ⏱️ Total playtime: 1,247 hours
├── 🏆 Completion rate: 23% completed
└── 💰 Library value: $12,450 (estimated)
```

### Game Analytics

```
Game Details → Statistics:
├── ⏱️ Total playtime: 45.5 hours
├── 📅 Last played: 3 days ago
├── 🚀 Launch count: 23 times
├── 📊 Session average: 1.9 hours
└── 🏆 Achievement progress: 67%
```

## Sorun Giderme

### ❗ Yaygın Sorunlar ve Çözümler

### 🎮 Oyun Başlatma Sorunları

**Problem**: Oyun başlamıyor veya hata veriyor

```
🔧 Çözüm Adımları:
├── 1️⃣ Platform launcher'ı kontrol et
├── 2️⃣ Game → Edit → Installation sekmesi
├── 3️⃣ Executable path doğruluğunu kontrol et
├── 4️⃣ Arguments ve working directory ayarla
├── 5️⃣ "Run as administrator" seçeneğini dene
└── 6️⃣ Compatibility mode ayarlarını kontrol et
```

**Launcher Problems**:

```
Platform Specific Fixes:
├── Steam: Steam Client çalışıyor mu?
├── Epic: Epic Games Launcher güncel mi?
├── GOG: GOG Galaxy 2.0 kurulu mu?
├── Xbox: Xbox app ile giriş yapıldı mı?
└── Uplay: Ubisoft Connect güncel mi?
```

### 📊 Meta Veri Sorunları

**Problem**: Oyun bilgileri ve görseller eksik

```
🔧 Meta Veri Düzeltme:
├── 1️⃣ Oyun → Düzenle → Genel → "Meta Veri İndir"
├── 2️⃣ Farklı meta veri sağlayıcısı dene (IGDB → RAWG)
├── 3️⃣ Manuel meta veri düzenleme yap
├── 4️⃣ Özel görseller ekle
└── 5️⃣ Topluluk veritabanı katkılarını kontrol et
```

### 🔄 Senkronizasyon Sorunları

**Problem**: Platform ile senkronizasyon sorunu

```
🔧 Senkron Düzeltme Adımları:
├── 1️⃣ Ayarlar → Entegrasyonlar → Platform → Yeniden Bağlan
├── 2️⃣ Platform önbelleğini temizle
├── 3️⃣ Platform'da manuel yenileme
├── 4️⃣ API kimlik bilgilerini kontrol et
└── 5️⃣ Platform'ı yeniden başlat
```

## İpuçları ve Püf Noktaları

### 🎯 Verimlilik İpuçları

### ⌨️ Klavye Kısayolları

```
🚀 Temel Kısayollar:
├── Ctrl+F → Hızlı arama
├── Ctrl+F5 → Kütüphane güncelleme
├── Ctrl+D → Meta veri indirme
├── F2 → Filtre panelini aç/kapat
├── F3 → Seçili oyunu düzenle
├── F5 → Mevcut görünümü yenile
├── F11 → Tam ekran aç/kapat
├── Ctrl+Shift+A → Manuel oyun ekleme
└── Ctrl+, → Ayarlar
```

### 🔍 Gelişmiş Arama İpuçları

```
🎯 Arama Operatörleri:
├── "kesin ifade" → Tam eşleşme
├── -hariçtut → Terimi hariç tut
├── genre:action → Türe göre filtrele
├── platform:steam → Platforma göre filtrele
├── year:2023 → Yıla göre filtrele
├── rating:>8 → Puanlara göre filtrele
└── played:false → Oynalmamış oyunlar
```

### 📊 Kütüphane Organizasyonu

```
🗂️ Organizasyon En İyi Uygulamaları:
├── 🏷️ Ruh hali/tür için özel kategoriler kullan
├── ⭐ Tamamlanan oyunları puanla
├── 📝 Kişisel notlar ve yorumlar ekle
├── 🎯 "Şu An Oynuyor" kategorisi oluştur
├── 🏆 Tamamlanma durumunu takip et
├── 📅 Oyun yığını için "Sonra Oyna" kullan
└── 🔄 Düzenli kütüphane temizliği yap
```

---

### 📚 Resmi Kaynaklar

### Playnite Official

- **🌐 Website**: [playnite.link](https://playnite.link/)
- **📖 Documentation**: [playnite.link/docs](https://playnite.link/docs/)
- **💾 GitHub**: [JosefNemec/Playnite](https://github.com/JosefNemec/Playnite)