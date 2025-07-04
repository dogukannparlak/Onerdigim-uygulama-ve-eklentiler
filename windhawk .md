# windhawk

---

## 🎯 Genel Bakış

### Araç Hakkında

Windhawk, Windows programlarını özelleştirmeyi kolaylaştırmayı amaçlayan devrimci bir araçtır. Ramen Software tarafından geliştirilen bu platform, kullanıcıların sadece birkaç tıklama ile modlar (özelleştirme modülleri) yüklemesine ve yapılandırmasına olanak tanır. Geliştiriciler için ise bu tür modları geliştirmek ve paylaşmak için uygun bir platform sağlar.

### Temel Özellikler

- ✅ **Kolay Mod Yükleme**: Tek tıkla mod kurulumu ve kaldırma
- ✅ **Açık Kaynak Güvenlik**: Tüm modlar kaynak kod halinde paylaşılır
- ✅ **Gelişmiş Enjeksiyon**: Güvenli ve stabil process injection teknolojisi
- ✅ **Canlı Düzenleme**: Modları gerçek zamanlı olarak düzenleme
- ✅ **Kapsamlı Hata Ayıklama**: Debug logging ve troubleshooting araçları
- ✅ **Çoklu Platform**: Windows 7’den Windows 11’e kadar geniş destek
- ✅ **Topluluk Kataloğu**: Zengin mod kütüphanesi

---

## 🚀 Kurulum ve Başlangıç

### Sistem Gereksinimleri

| Gereksinim | Minimum | Önerilen |
| --- | --- | --- |
| **İşletim Sistemi** | Windows 7 SP1 | Windows 10/11 22H2+ |
| **RAM** | 512 MB | 2 GB+ |
| **Depolama** | 100 MB | 500 MB+ |
| **İşlemci** | x86/x64 | x64/ARM64 |
| **Yetki** | Yönetici hakları | Yönetici hakları |

### Kurulum Yöntemleri

### 1️⃣ Resmi Website’den İndirme (Önerilen)

1. https://ramensoftware.com/windhawk adresine gidin
2. **Download** butonuna tıklayın
3. `windhawk_setup.exe` dosyasını indirin
4. İndirilen dosyayı sağ tık → **Yönetici olarak çalıştır**

### 2️⃣ Winget ile Kurulum

```powershell
winget install windhawk
```

### 3️⃣ Chocolatey ile Kurulum

```powershell
choco install windhawk
```

### ⚙️ İlk Kurulum Ayarları

### İlk Çalıştırma:

1. **Yönetici İzinleri**: UAC onayı verin
2. **Service Başlatma**: Windhawk servisi otomatik başlatılır
3. **Katalog Yenileme**: Mod kataloğu ilk kez yüklenir
4. **Güvenlik Taraması**: Sistem uyumluluğu kontrol edilir

---

## 🖥️ Ana Arayüz ve Navigasyon

### 📱 Ana Pencere Bileşenleri

Windhawk ana arayüzü modern ve kullanıcı dostu bir tasıma sahiptir:

| Bileşen | Konum | İşlev |
| --- | --- | --- |
| **Mod Kataloğu** | Sol panel | Mevcut modları görüntüle |
| **Yüklü Modlar** | Üst sekme | Aktif modları yönet |
| **Ayarlar** | Sağ üst | Genel yapılandırma |
| **Arama Çubuğu** | Üst orta | Mod arama |
| **Durum Çubuğu** | Alt | Sistem durumu |

### 🔍 Arama ve Filtreleme

### Gelişmiş Arama Seçenekleri:

| Filtre | Açıklama | Kullanım |
| --- | --- | --- |
| **Kategori** | Mod türüne göre filtreleme | Taskbar, Explorer, vb. |
| **Popülerlik** | İndirme sayısına göre sıralama | En çok kullanılan modlar |
| **Güncelleme** | Yayın tarihine göre | En yeni modlar |
| **Durum** | Aktif/pasif modlar | Yüklü mod yönetimi |

## 🔧 Mod Yönetimi

### 📦 Mod Kurulumu

### Katalogdan Kurulum:

1. **Mod Seçimi**: Katalogda istenen modu bulun
2. **Detay İnceleme**: Mod açıklamasını ve ayarları inceleyin
3. **Kurulum**: **Install** butonuna tıklayın
4. **Aktivasyon**: Mod otomatik olarak aktif hale gelir

### Manuel Kurulum:

```cpp
// Mod dosyasını (.wh.cpp) kaydedin// Windhawk → Settings → Advanced → Load mod from file
```

### 🔄 Mod Güncelleme

### Otomatik Güncelleme:

```
Settings → Updates → Auto-update mods: ✅
Update frequency: Daily/Weekly
```

### Manuel Güncelleme:

1. **Installed Mods** sekmesine gidin
2. Güncelleme olan modları kontrol edin
3. **Update** butonuna tıklayın
4. Değişiklikleri inceleyin ve onaylayın

---

## 🌟 Popüler Modlar

### 📁 Better File Sizes in Explorer Details

**🔥 En Popüler Explorer Modlarından Biri**

Bu mod, Windows Explorer’ın details görünümünde dosya boyutlarını çok daha kullanışlı ve okunabilir hale getirir. Klasörlerin boyutlarını gösterebilir ve dosya boyutlarını daha anlaşılır formatlarda sunar.

### 📊 Ana Özellikler

| **Özellik** | **Açıklama** | **Örnek** |
| --- | --- | --- |
| **Klasör Boyutları** | Klasörlerin toplam boyutunu gösterir | `📁 Documents: 2.5 GB` |
| **Akıllı Format** | Büyük dosyalar için MB/GB kullanır | `video.mp4: 1.2 GB` |
| **IEC Standartları** | Teknik olarak doğru birimleri kullanır | `KiB, MiB, GiB` |
| **Karışık Sıralama** | Dosya ve klasörleri birlikte sıralar | Boyuta göre karma liste |

### 🔧 Yapılandırma Seçenekleri

### 1. Klasör Boyutlarını Gösterme

**🚀 Everything Entegrasyonu (Önerilen)**

```
✅ "Everything" programını indirin (https://www.voidtools.com)
✅ Everything'de folder size indexing'i aktif edin:
   - Tools → Options → Indexes → Index file size
   - Tools → Options → Indexes → Index folder size
✅ Windhawk ayarları: "Enabled via Everything integration"
✅ Sonuç: Anında klasör boyutu hesaplama (20x daha hızlı!)
```

**⚡ Manuel Hesaplama**

```
- "Enabled, calculated manually": Her zaman hesapla (yavaş)
- "While holding Shift key": Sadece Shift basılıyken hesapla
- Büyük klasörler için zaman alabilir
```

### 2. Boyut Formatları

**Use MB/GB for large files**

```
❌ Kapalı: 1,234,567 KB
✅ Açık:   1.2 GB
```

**Use IEC terms**

```
❌ Kapalı: KB, MB, GB (1000 tabanlı)
✅ Açık:   KiB, MiB, GiB (1024 tabanlı)
```

### 3. Sıralama Seçenekleri

**Mix files and folders when sorting by size**

```
❌ Kapalı: Önce klasörler, sonra dosyalar
✅ Açık:   Boyuta göre karma sıralama
```

### 🎯 Kullanım Senaryoları

### Disk Temizliği

```
1. Klasör boyutlarını aktif edin
2. Size sütununa tıklayın (büyükten küçüğe sırala)
3. En büyük klasörleri görün
4. Gereksiz dosyaları temizleyin
5. Anında disk alanı tasarrufu!
```

### Dosya Yönetimi

```
1. MB/GB formatını aktif edin
2. Büyük dosyaları kolayca tespit edin
3. Karışık sıralama ile tüm öğeleri birlikte görün
4. Daha efektif dosya organizasyonu yapın
```

### 🔧 Kurulum Adımları

1. **Windhawk’da modları arayın**: “Better file sizes”
2. **Install** butonuna tıklayın
3. **Everything indirin** (isteğe bağlı ama önerilen)
4. **Mod ayarlarına gidin** ve tercihinize göre yapılandırın
5. **Explorer’ı yeniden başlatın** (gerekliyse)

---

### 🌐 Chrome/Edge Scroll Tabs with Mouse Wheel

**🚀 Web Tarayıcı Verimliliği için Vazgeçilmez Mod**

Bu mod, web tarayıcılarında mouse wheel ile tab bar üzerinde scroll yaparak sekmeler arasında hızlıca geçiş yapmanızı sağlar. Çok fazla sekme açan kullanıcılar için büyük kolaylık sunar.

### 🎯 Ana Özellikler

| **Özellik** | **Açıklama** | **Faydası** |
| --- | --- | --- |
| **Mouse Wheel Navigation** | Tab bar üzerinde scroll ile sekme geçişi | Hızlı navigasyon |
| **Çoklu Tarayıcı Desteği** | Chrome, Edge, Opera, Brave, Yandex | Geniş uyumluluk |
| **Horizontal Scrolling** | Yatay scroll wheel desteği | Gaming mouse kullanıcıları için |
| **Scroll Area Limit** | Sadece tab bar alanında çalışır | Yanlış aktivasyon önleme |

### 🖱️ Desteklenen Tarayıcılar

```
✅ Google Chrome      - Tam destek
✅ Microsoft Edge     - Tam destek
✅ Opera              - Tam destek
✅ Brave              - Tam destek
✅ Yandex Browser     - Tam destek
```

### ⚙️ Yapılandırma Seçenekleri

### 1. Scroll Yönü Ayarları

**Reverse Scrolling Direction**

```
❌ Kapalı: Wheel yukarı = Sağdaki sekme
✅ Açık:   Wheel yukarı = Soldaki sekme
```

### 2. Horizontal Scrolling

**Gaming Mouse Desteği**

```
✅ Horizontal scroll wheel ile de sekme değiştirme
✅ Logitech, Razer gibi gaming mouse'lar için
✅ Tilt wheel özelliği olan tüm mouse'lar
```

### 3. Scroll Area Limit

**Çalışma Alanı Sınırlandırması**

```
📐 Pixels from top: 0     (Tab bar üst kenarından başlama)
📐 Pixels from left: 0    (Tab bar sol kenarından başlama)
🎯 Sadece tab bar alanında scroll işlemi
🛡️ Sayfa içeriğinde yanlışlıkla tetikleme önleme
```

### 📊 Performans ve Verimlilik

| **Durum** | **Geleneksel Yöntem** | **Bu Mod ile** |
| --- | --- | --- |
| **Sekme Değiştirme** | Ctrl+Tab veya tıklama | Mouse wheel |
| **Hız** | 2-3 saniye | Anında |
| **El Pozisyonu** | İki el gerekli | Tek el yeterli |
| **Hassasiyet** | Tam sekme seçme | Sıralı geçiş |

### 🔧 Kurulum ve Aktivasyon

**Adım Adım Kurulum:**

```
1. Windhawk'da "Chrome Edge scroll tabs" araması yapın
2. Mod'u install edin
3. Desteklenen tarayıcılardan birini açın
4. Tab bar üzerinde mouse wheel ile test edin
5. Ayarları tercihinize göre düzenleyin
```

**Anında Aktif:**

```
🚀 Kurulum sonrası hemen çalışır
🔄 Tarayıcı yeniden başlatma gerekmez
⚙️ Ayar değişiklikleri anında uygulanır
```

### 🎪 Ek Özellikler

| **Özellik** | **Açıklama** | **Kullanım** |
| --- | --- | --- |
| **Multi-Monitor** | Çoklu monitör desteği | Her monitörde bağımsız çalışır |
| **Full-Screen** | Tam ekran modunda çalışır | Presentation modlarında faydalı |
| **Minimized State** | Minimize durumunda bile aktif | Arka planda çalışan sekmelerde |

Bu mod özellikle **power user’lar**, **geliştiriciler** ve **araştırma yapan kullanıcılar** için çok değerli. Web’de çok fazla sekme ile çalışanlar için gerçek bir zaman tasarrufu sağlıyor! 🌐⚡

---

### 🏷️ Taskbar Labels for Windows 11

**⭐ Windows 11’in En Popüler Taskbar Modu**

Windows 11’de taskbar’daki uygulama butonlarına text label’ları (yazı etiketleri) ekler ve çeşitli görsel özelleştirmeler sunar. Windows 10’un klasik taskbar deneyimini Windows 11’e getirir.

### 🎯 Ana Özellikler

| **Özellik** | **Açıklama** | **Görsel Sonuç** |
| --- | --- | --- |
| **Text Labels** | Uygulama isimlerini taskbar’da gösterir | `📁 File Explorer` |
| **4 Farklı Mod** | Çeşitli görüntüleme seçenekleri | Icon+Text kombinasyonları |
| **Running Indicator** | Çalışan uygulamalar için gösterge | Çizgi, nokta veya custom stil |
| **Font Customization** | Yazı tipi ve boyut ayarları | 12pt, custom font |

### 🎨 Görüntüleme Modları

### 1. Show Labels, Don’t Combine (Varsayılan)

```
📸 Görünüm:
[📁 Desktop - File Explorer] [🌐 Chrome] [📁 Downloads - File Explorer]

✅ Her pencere ayrı buton
✅ Full label görünümü
✅ Windows 10 tarzı deneyim
```

### 2. Hide Labels, Combine Taskbar Buttons

```
📸 Görünüm:
[📁] [🌐] [📁]

✅ Sadece iconlar
✅ Aynı uygulama pencereleri birleşir
✅ Minimal görünüm
```

### 3. Show Labels, Combine Taskbar Buttons

```
📸 Görünüm:
[📁 File Explorer] [🌐 Chrome] [📁 Windhawk]

✅ Label + icon birlikte
✅ Aynı uygulamalar birleşir
✅ Dengeli görünüm
```

### 4. Hide Labels, Don’t Combine

```
📸 Görünüm:
[📁] [🌐] [🆔] [📁] [⬇️] [🦅]

✅ Sadece iconlar
✅ Her pencere ayrı
✅ Compact görünüm
```

### ⚙️ Detaylı Yapılandırma

### Font ve Görünüm Ayarları

| **Ayar** | **Varsayılan** | **Açıklama** |
| --- | --- | --- |
| **Font Size** | 12 | Yazı boyutu (8-24 arası) |
| **Font Family** | Segoe UI | Windows 11 font listesi |
| **Text Trimming** | Ellipsis (…) | Uzun isimler için kısaltma |
| **Left/Right Padding** | 8 pixel | Buton iç boşlukları |

### Running Indicator Stilleri

**Centered, Fixed Size (Varsayılan)**

```
📸 Görünüm: Her butonun altında sabit boyut çizgi
✅ Tutarlı görünüm
✅ Windows 11 native stil
```

**Centered, Dynamic Size**

```
📸 Görünüm: Buton genişliğine göre ayarlanan çizgi
✅ Responsive tasarım
✅ Farklı buton boyutlarına uyum
```

**On the Left (Below Icon)**

```
📸 Görünüm: Icon'un sol altında gösterge
✅ Klasik Windows 10 stil
✅ Compact görünüm
```

**Full Width**

```
📸 Görünüm: Butonun tüm genişliğinde çizgi
✅ Belirgin gösterge
✅ Modern görünüm
```

### 🎛️ Gelişmiş Ayarlar

### Program Hariç Tutma

```
Excluded Programs (Örnek):
- mspaint.exe          (Paint uygulaması)
- notepad.exe          (Notepad)
- Calculator.exe       (Hesap makinesi)
- excluded1.exe        (Custom exclusion)
```

### Taskbar Boyut Kontrolü

```
🔧 Taskbar Item Width: 100 pixel
📏 Minimum Width: 50 pixel
📏 Maximum Width: 176 pixel
⚖️ Windows adaptive width: 0 (otomatik)
```

### Running Indicator Özelleştirme

```
📐 Height: 0 (varsayılan boyut)
📐 Vertical Offset: 0 (konumlandırma)
🎨 Progress Indicator: Aynı stil
```

### 🔧 Kurulum ve Aktivasyon

**Hızlı Kurulum:**

```
1. Windhawk'da "Taskbar Labels" araması yapın
2. Mod'u install edin
3. Mod otomatik olarak aktif olur
4. Taskbar'da değişiklikleri görün
5. Settings'den istediğiniz modu seçin
```

**İlk Yapılandırma:**

```
✅ Mode seçimi: "Show labels, don't combine"
✅ Font size: Ekranınıza uygun boyut
✅ Running indicator: "Centered, fixed size"
✅ Excluded programs: İstemediğiniz uygulamaları ekleyin
```

### 🆚 Windows 10 vs Windows 11

| **Özellik** | **Windows 10** | **Bu Mod ile Win11** |
| --- | --- | --- |
| **Taskbar Labels** | ✅ Native | ✅ Custom implementation |
| **Combine Options** | ✅ 3 seçenek | ✅ 4 seçenek |
| **Font Customization** | ❌ Yok | ✅ Full control |
| **Running Indicator** | ⚖️ Basit | ✅ 4 farklı stil |
| **Exclusion List** | ❌ Yok | ✅ Program bazlı kontrol |

### 🎪 Ek Notlar

**Windows 11 Compatibility:**

```
✅ Windows 11 22H2+ tam destek
✅ Eski sürümler: limited implementation
✅ İnsider builds: beta desteği
⚠️ Major updates sonrası kontrol gerekli
```

**Variable Support:**

```
🔤 %name%: Uygulama adı
🔢 %amount%: Pencere sayısı
📋 Tek pencere: %name%
📋 Çoklu pencere: [%amount%] %name%
```

Bu mod, **Windows 11’i Windows 10 taskbar deneyimine** en yakın hale getiren en popüler modlardan biri. Özellikle çok pencere ile çalışan kullanıcılar için vazgeçilmez! 🏷️✨

- 📋 **Gelişmiş Mod Ayarları - Taskbar Labels JSON Konfigürasyonu**
    
    ```json
    {  "mode": "noLabelsWithCombining",  "taskbarItemWidth": 100,  "runningIndicatorStyle": "centerFixed",  "progressIndicatorStyle": "sameAsRunningIndicatorStyle",  "excludedPrograms[0]": "excluded1.exe",  "minimumTaskbarItemWidth": 50,  "maximumTaskbarItemWidth": 176,  "fontSize": 12,  "leftAndRightPaddingSize": 8,  "spaceBetweenIconAndLabel": 8,  "alwaysShowThumbnailLabels": 0,  "labelForSingleItem": "%name%",  "labelForMultipleItems": "[%amount%] %name%",  "fontFamily": "",  "runningIndicatorHeight": 0,  "runningIndicatorVerticalOffset": 0,  "textTrimming": "characterEllipsis"}
    ```
    
    **📝 Ayar Açıklamaları:**
    
    **🎨 Görüntüleme Modları:**
    - `"showLabelsAndDontCombine"`: Label göster, birleştirme
    - `"hideLabelsAndCombine"`: Label gizle, birleştir
    
    - `"showLabelsAndCombine"`: Label göster, birleştir
    - `"noLabelsWithCombining"`: Sadece icon, birleştir
    
    **📏 Boyut Kontrolleri:**
    - `taskbarItemWidth`: Varsayılan buton genişliği (100px)
    - `minimumTaskbarItemWidth`: Minimum genişlik (50px)
    - `maximumTaskbarItemWidth`: Maksimum genişlik (176px)
    - `fontSize`: Yazı boyutu (12pt)
    - `leftAndRightPaddingSize`: Yatay iç boşluk (8px)
    - `spaceBetweenIconAndLabel`: Icon-text arası mesafe (8px)
    
    **🎯 Running Indicator Stilleri:**
    - `"centerFixed"`: Merkez, sabit boyut
    - `"centerDynamic"`: Merkez, dinamik boyut
    - `"leftBelow"`: Sol alt, icon altında
    - `"fullWidth"`: Tam genişlik
    
    **🏷️ Label Template’leri:**
    - `%name%`: Uygulama adı
    - `%amount%`: Pencere sayısı
    - `labelForSingleItem`: Tek pencere → `"Firefox"`
    - `labelForMultipleItems`: Çoklu → `"[3] Firefox"`
    
    **🚫 Program Hariç Tutma:**
    
    ```json
    "excludedPrograms[0]": "notepad.exe","excludedPrograms[1]": "calculator.exe","excludedPrograms[2]": "mspaint.exe"
    ```
    
    **📱 Ek Özellikler:**
    - `alwaysShowThumbnailLabels`: Thumbnail’larda label göster (0/1)
    - `textTrimming`: Uzun metin kısaltması (“characterEllipsis”)
    - `fontFamily`: Özel font (“Segoe UI”, “Consolas”, vb.)
    - `runningIndicatorHeight`: Gösterge yüksekliği (0=varsayılan)
    - `runningIndicatorVerticalOffset`: Dikey ofset (0=merkez)
    
    **🔧 Kullanım:**
    1. Windhawk → Taskbar Labels for Windows 11 → Settings
    2. JSON konfigürasyonunu yapıştırın
    3. Mode ve boyut ayarlarını tercihinize göre düzenleyin
    4. Apply ile uygulayın
    
    **💡 Pro İpuçları:**
    - DPI ayarınıza göre `fontSize` değerini artırın (125% DPI = 14-15pt)
    - Ultrawide monitörlerde `taskbarItemWidth` değerini artırın
    - Çok program kullananlar için excluded programs listesi oluşturun
    

---

### 🔔 Windows 11 Notification Center Styler

**🎨 Bildirim Merkezi Görsel Özelleştirme Modu**

Windows 11’in Notification Center (Bildirim Merkezi) ve Quick Settings (Hızlı Ayarlar) panelinin görünümünü tamamen özelleştirmenizi sağlar. CSS tabanlı theming sistemi ile profesyonel tasarımlar oluşturabilirsiniz.

### 🎯 Ana Özellikler

| **Özellik** | **Açıklama** | **Kapsam** |
| --- | --- | --- |
| **CSS Theming** | Tam CSS desteği ile özelleştirme | Renkler, fontlar, şeffaflık |
| **Pre-built Themes** | Hazır tema şablonları | Dark, Light, Transparent |
| **Quick Settings** | Hızlı ayarlar paneli styling | Butonlar, slider’lar, toggles |
| **Notification Cards** | Bildirim kartları özelleştirme | Arka plan, kenarlıklar, gölgeler |
| **Animation Control** | Animasyon ve geçiş efektleri | Fade, slide, opacity |

### 🎨 Desteklenen Bileşenler

### Notification Center Alanları

```
📋 Notification Header        - Üst başlık alanı
📝 Notification Cards         - Bildirim kartları
🎛️ Quick Settings Panel      - Hızlı ayarlar paneli
🔘 Quick Action Buttons       - Hızlı eylem butonları
🎚️ Brightness Slider         - Parlaklık ayarlayıcısı
🔊 Volume Slider             - Ses seviyesi ayarlayıcısı
⚙️ Settings Button           - Ayarlar butonu
```

### CSS Targeting Sistemi

```css
/* Ana container */.NotificationCenterToast {}
/* Bildirim kartları */.ToastContentContainer {}
/* Quick Settings */.QuickActionsContainer {}
/* Hızlı eylem butonları */.QuickActionButton {}
/* Slider kontrolleri */.SystemVolumeSlider {}
.SystemBrightnessSlider {}
```

### 🎭 Örnek Tema Stilleri

### 1. Dark Glass Theme

```css
/* Ana panel - şeffaf koyu tema */.NotificationCenterToast {
    background: rgba(30, 30, 30, 0.85);    backdrop-filter: blur(20px);    border: 1px solid rgba(255, 255, 255, 0.1);    border-radius: 12px;}
/* Bildirim kartları */.ToastContentContainer {
    background: rgba(45, 45, 45, 0.9);    border: 1px solid rgba(255, 255, 255, 0.05);    box-shadow: 0 8px 32px rgba(0, 0, 0, 0.3);}
/* Quick action butonları */.QuickActionButton {
    background: linear-gradient(135deg, #667eea 0%, #764ba2 100%);    border: none;    border-radius: 8px;    color: white;}
```

### 2. Light Minimalist Theme

```css
/* Minimal açık tema */.NotificationCenterToast {
    background: rgba(255, 255, 255, 0.95);    backdrop-filter: blur(30px);    border: 1px solid rgba(0, 0, 0, 0.05);    box-shadow: 0 10px 40px rgba(0, 0, 0, 0.1);}
.ToastContentContainer {
    background: white;    border: 1px solid #f0f0f0;    border-radius: 6px;}
.QuickActionButton {
    background: #f8f9fa;    border: 1px solid #e9ecef;    color: #495057;    transition: all 0.2s ease;}
```

### 3. Neon Gaming Theme

```css
/* Gaming teması - neon efektler */.NotificationCenterToast {
    background: rgba(10, 10, 20, 0.9);    border: 2px solid #00ff88;    box-shadow: 0 0 20px rgba(0, 255, 136, 0.3);}
.QuickActionButton {
    background: linear-gradient(45deg, #ff006e, #00f5ff);    border: 2px solid transparent;    box-shadow: 0 0 15px rgba(255, 0, 110, 0.5);    text-shadow: 0 0 10px rgba(255, 255, 255, 0.8);}
.SystemVolumeSlider {
    background: linear-gradient(90deg, #ff006e, #00f5ff);    border-radius: 20px;    box-shadow: 0 0 10px rgba(0, 245, 255, 0.4);}
```

### ⚙️ Yapılandırma Seçenekleri

### CSS Injection Metodu

```
🎯 Direct CSS Input: Doğrudan CSS kodu girişi
📁 External CSS File: Harici CSS dosyası bağlama
🔗 Online CSS URL: Web'den CSS yükleme
🎨 Theme Builder: Görsel tema oluşturucu (gelişmiş)
```

### Target Selectors

```css
/* Ana hedef sınıflar - referans için */.NotificationCenterToast         /* Ana bildirim paneli */.ToastContentContainer          /* Bildirim içeriği */.QuickActionsContainer          /* Hızlı eylemler alanı */.QuickActionButton              /* Hızlı eylem butonları */.SystemVolumeSlider             /* Ses slider'ı */.SystemBrightnessSlider         /* Parlaklık slider'ı */.NotificationAppName            /* Uygulama adı */.NotificationContent            /* Bildirim metni */
```

### 🔧 Gelişmiş Özelleştirme

### Animation & Transitions

```css
/* Smooth geçişler */.ToastContentContainer {
    transition: all 0.3s cubic-bezier(0.25, 0.46, 0.45, 0.94);    transform: translateY(0);}
.ToastContentContainer:hover {
    transform: translateY(-2px);    box-shadow: 0 12px 40px rgba(0, 0, 0, 0.2);}
/* Fade-in animasyonu */@keyframes slideIn {
    from { opacity: 0; transform: translateX(100%); }
    to { opacity: 1; transform: translateX(0); }
}
.NotificationCenterToast {
    animation: slideIn 0.4s ease-out;}
```

### Responsive Design

```css
/* Farklı ekran boyutları için */@media (max-width: 1920px) {
    .NotificationCenterToast {
        width: 400px;        max-height: 80vh;    }
}
@media (max-width: 1366px) {
    .NotificationCenterToast {
        width: 350px;        font-size: 14px;    }
}
```

### 🎯 Kullanım Senaryoları

### Profesyonel Ortam

```css
/* Kurumsal tema - sade ve profesyonel */.NotificationCenterToast {
    background: #ffffff;    border: 1px solid #e1e5e9;    font-family: 'Segoe UI', sans-serif;    color: #333333;}
.QuickActionButton {
    background: #0078d4;    color: white;    font-weight: 500;}
```

### Gaming Setup

```css
/* RGB gaming teması */.NotificationCenterToast {
    background: linear-gradient(45deg, #1a1a2e, #16213e, #0f3460);    border: 2px solid;    border-image: linear-gradient(45deg, #ff0080, #00ff80, #0080ff) 1;}
.QuickActionButton:nth-child(odd) {
    background: linear-gradient(135deg, #ff0080, #ff8000);}
.QuickActionButton:nth-child(even) {
    background: linear-gradient(135deg, #00ff80, #0080ff);}
```

### Content Creator

```css
/* Yaratıcı tema - modern ve şık */.NotificationCenterToast {
    background: linear-gradient(135deg, #667eea 0%, #764ba2 100%);    backdrop-filter: blur(25px);    color: white;}
.ToastContentContainer {
    background: rgba(255, 255, 255, 0.1);    border: 1px solid rgba(255, 255, 255, 0.2);    backdrop-filter: blur(10px);}
```

### 🛠️ Kurulum ve Konfigürasyon

### Temel Kurulum

```
1. Windhawk'da "Windows 11 Notification Center Styler" araması yapın
2. Mod'u install edin
3. Mod ayarlarına gidin
4. CSS kodunuzu girin veya hazır tema seçin
5. Apply butonuna tıklayın - anında etki eder!
```

### CSS Dosyası ile Kurulum

```
1. CSS dosyanızı hazırlayın (örn: notification-theme.css)
2. Mod ayarlarında "External CSS File" seçin
3. Dosya yolunu belirtin
4. Auto-reload aktif edin (geliştirme için)
```

### 🎨 Tema Geliştirme İpuçları

### CSS Best Practices

```css
/* Performanslı animasyonlar için */.element {
    will-change: transform, opacity;    transform: translateZ(0); /* Hardware acceleration */}
/* Responsive units kullanın */.NotificationCenterToast {
    font-size: clamp(12px, 2vw, 16px);    padding: clamp(8px, 1.5vw, 20px);}
/* CSS Custom Properties ile tema sistemi */:root {
    --primary-color: #0078d4;    --background-color: rgba(255, 255, 255, 0.9);    --text-color: #333333;    --border-radius: 8px;}
```

### 📚 Tema Kaynakları

GitHub’daki [resmi styling guide](https://github.com/ramensoftware/windows-11-notification-center-styling-guide/blob/main/README.md#themes) referansında:

- **Detaylı CSS selectors** listesi
- **Örnek tema kodları** koleksiyonu
- **Best practices** rehberi
- **Troubleshooting** ipuçları
- **Community themes** paylaşımları

Bu mod, **Windows 11’in bildirim sistemini** kişiselleştirmek isteyen kullanıcılar için mükemmel. CSS bilgisi olan kullanıcılar sınırsız özelleştirme yapabilirken, hazır temalarla basit kullanım da mümkün! 🔔🎨

- 📋 **Gelişmiş Mod Ayarları - Notification Center Styler JSON Konfigürasyonu**
    
    ```json
    {  "theme": "",  "resourceVariables[0].variableKey": "",  "resourceVariables[0].value": "",  "styleConstants[0]": "",  "controlStyles[0].target": "Grid#NotificationCenterGrid",  "controlStyles[0].styles[0]": "Shadow:=",  "controlStyles[1].target": "Grid#CalendarCenterGrid",  "controlStyles[1].styles[0]": "Shadow:=",  "controlStyles[2].target": "Grid#MediaTransportControlsRegion",  "controlStyles[2].styles[0]": "Shadow:=",  "controlStyles[3].target": "Grid#ControlCenterRegion",  "controlStyles[3].styles[0]": "Shadow:=",  "controlStyles[10].target": "Grid#NotificationCenterGrid",  "controlStyles[10].styles[0]": "Background:=<AcrylicBrush TintColor=\"#1F2738\" TintLuminosityOpacity=\"0.8\" TintOpacity=\"0.6\" Opacity=\"0.80\" FallbackColor=\"#2b283f\"/>",  "controlStyles[10].styles[1]": "BorderThickness=0,0,0,0",  "controlStyles[10].styles[2]": "CornerRadius=30",  "controlStyles[15].target": "MenuFlyoutPresenter",  "controlStyles[15].styles[0]": "Background:=<AcrylicBrush TintColor=\"#1F2738\" TintLuminosityOpacity=\"0.8\" TintOpacity=\"0.6\" Opacity=\"0.80\" FallbackColor=\"#2b283f\"/>",  "controlStyles[15].styles[1]": "BorderThickness=0,0,0,0",  "controlStyles[15].styles[2]": "CornerRadius=30",  "controlStyles[15].styles[3]": "Padding=2,4,2,4",  "controlStyles[27].target": "Border#ToastBackgroundBorder2",  "controlStyles[27].styles[0]": "Background:=<AcrylicBrush TintColor=\"#1F2738\" TintLuminosityOpacity=\"0.8\" TintOpacity=\"0.5\" Opacity=\"1\" FallbackColor=\"#2b283f\"/>",  "controlStyles[27].styles[1]": "BorderThickness=0,0,0,0",  "controlStyles[27].styles[2]": "CornerRadius=6",  "controlStyles[27].styles[3]": "Shadow:=",  "controlStyles[31].target": "ActionCenter.FocusSessionControl",  "controlStyles[31].styles[0]": "Height=0"}
    ```
    
    **📝 Açıklama:**
    - `theme`: Hazır tema seçimi
    - `controlStyles[X].target`: Bildirim merkezi bileşen hedefleri
    - `Background:=<AcrylicBrush>`: Acrylic cam efekti ayarları
    - `TintColor`: Ana renk tonu (#1F2738 = koyu mavi-gri)
    - `TintOpacity`: Renk saydamlığı (0.6 = %60)
    - `CornerRadius`: Köşe yuvarlatma (30 = çok yuvarlatılmış)
    - `Shadow:=`: Gölge efektlerini kaldırma
    
    **🎨 Örnek Stil Hedefleri:**
    - `Grid#NotificationCenterGrid`: Ana bildirim paneli
    - `Grid#CalendarCenterGrid`: Takvim bölümü
    - `Grid#MediaTransportControlsRegion`: Medya kontrolleri
    - `Border#ToastBackgroundBorder2`: Bildirim kartları
    - `MenuFlyoutPresenter`: Açılır menüler
    - `ActionCenter.FocusSessionControl`: Focus session kontrolleri
    
    **🎯 Renk Paleti (Dark Glass Tema):**
    - Ana Renk: `#1F2738` (Koyu mavi-gri)
    - Fallback: `#2b283f` (Koyu mor-gri)
    - Saydamlık: 0.6-0.8 arası
    - Köşe: 6-30px yuvarlatma
    
    **🔧 Kullanım:**
    1. Windhawk → Notification Center Styler → Settings
    2. JSON konfigürasyonunu yapıştırın
    3. Renk ve stil değerlerini özelleştirin
    4. Apply ile uygulayın
    

---

### 🚀 Windows 11 Start Menu Styler

**⭐ En Güçlü Start Menu Özelleştirme Modu**

Windows 11’in Start Menu’sunu XAML tabanlı styling sistemi ile tamamen yeniden tasarlamanızı sağlar. [Resmi GitHub styling guide](https://github.com/ramensoftware/windows-11-start-menu-styling-guide/blob/main/README.md#themes) referansında 16 adet hazır tema ve kapsamlı özelleştirme rehberi bulunuyor.

### 🎯 Ana Özellikler

| **Özellik** | **Açıklama** | **Teknik Detay** |
| --- | --- | --- |
| **XAML Styling** | Microsoft’un native teknolojisi | Layout, renkler, boyutlar kontrolü |
| **Ready-Made Themes** | 16 topluluk teması | NoRecommended, Windows10, SideBySide, vb. |
| **Layout Control** | Menu düzenini değiştirme | Pinned Apps, Recommended positioning |
| **Visual Effects** | Acrylic, blur, shadow | Modern Fluent Design efektleri |
| **Search Integration** | Arama menüsü styling | WebView CSS + XAML karışımı |

### 🎨 Resmi Tema Koleksiyonu

[GitHub tema sayfasında](https://github.com/ramensoftware/windows-11-start-menu-styling-guide/blob/main/README.md#themes) bulunan hazır temalar:

| **Tema** | **Açıklama** | **Stil Kategorisi** |
| --- | --- | --- |
| [**NoRecommendedSection**](https://github.com/ramensoftware/windows-11-start-menu-styling-guide/blob/main/Themes/NoRecommendedSection/README.md) | Önerilen bölümü kaldırır | 🧹 Clean & Minimal |
| [**Windows10**](https://github.com/ramensoftware/windows-11-start-menu-styling-guide/blob/main/Themes/Windows10/README.md) | Windows 10 Start Menu deneyimi | 📰 Classic & Nostalgic |
| [**SideBySide**](https://github.com/ramensoftware/windows-11-start-menu-styling-guide/blob/main/Themes/SideBySide/README.md) | Yan yana dual layout | 📊 Productivity Layout |
| [**TranslucentStartMenu**](https://github.com/ramensoftware/windows-11-start-menu-styling-guide/blob/main/Themes/TranslucentStartMenu/README.md) | Şeffaf cam efekti | 🌟 Glass & Transparency |
| [**Fluent2Inspired**](https://github.com/ramensoftware/windows-11-start-menu-styling-guide/blob/main/Themes/Fluent2Inspired/README.md) | Microsoft Fluent Design 2.0 | 🎨 Modern Design |
| [**RosePine**](https://github.com/ramensoftware/windows-11-start-menu-styling-guide/blob/main/Themes/RosePine/README.md) | Aesthetic color palette | 🌹 Beautiful Colors |
| [**Down Aero**](https://github.com/ramensoftware/windows-11-start-menu-styling-guide/blob/main/Themes/Down%20Aero/README.md) | Windows Aero Glass | 💎 Glass Effects |
| [**21996**](https://github.com/ramensoftware/windows-11-start-menu-styling-guide/blob/main/Themes/21996/README.md) | Vintage Win11 build style | 🕰️ Retro Windows |

### ⚙️ Temel Yapılandırma

### Hızlı Tema Kurulumu

```
🔧 Adım Adım:
1. Windhawk → "Windows 11 Start Menu Styler" modunu kur
2. İstediğiniz temayı GitHub'dan seç
3. Tema README'sindeki XAML kodunu kopyala
4. Mod Settings → XAML kodunu yapıştır → Apply
5. Start Menu'yu aç ve değişiklikleri gör!
```

### Manuel Özelleştirme Hedefleri

[Resmi dokümantasyonda](https://github.com/ramensoftware/windows-11-start-menu-styling-guide/blob/main/README.md) bulunan temel hedefler:

| **Hedef** | **XAML Target** | **Kullanım** |
| --- | --- | --- |
| **Arama Kutusu** | `StartDocked.SearchBoxToggleButton` | `Height=0` ile gizle |
| **Pinned Apps** | `StartMenu.PinnedList` | `Margin` ile konumlandır |
| **Recommended** | `Grid#TopLevelSuggestionsContainer` | `Visibility=Collapsed` |
| **User Profile** | `StartDocked.UserTileView` | Profil butonunu gizle |
| **Power Button** | `StartDocked.PowerOptionsView` | Güç butonunu taşı |

### 🎭 Gelişmiş Özelleştirme Teknikleri

### 1. Custom Acrylic Background

```
<!-- Resmi dokümantasyondan acrylic örneği -->
Background:=<AcrylicBrush BackgroundSource="Backdrop"
                          TintColor="Pink"
                          TintOpacity="0.25" />
```

### 2. Color Schemes & Transforms

```
<!-- Accent color integration -->
Background:=<SolidColorBrush Color="{ThemeResource SystemAccentColor}"
                             Opacity="0.8" />

<!-- Transform effects -->
RenderTransform:=<TranslateTransform X="15" Y="-15" />
Transform3D:=<CompositeTransform3D ScaleX="1.5"
                                   TranslateY="-15"
                                   RotationZ="15" />
```

### 3. Gradient & Image Backgrounds

```
<!-- Multi-color gradient -->
Background:=<LinearGradientBrush StartPoint="0,0.5" EndPoint="1,0.5">
    <GradientStop Color="Yellow" Offset="0.0" />
    <GradientStop Color="Red" Offset="0.25" />
    <GradientStop Color="Blue" Offset="0.75" />
    <GradientStop Color="LimeGreen" Offset="1.0" />
</LinearGradientBrush>

<!-- Image background -->
Background:=<ImageBrush Stretch="UniformToFill"
                        ImageSource="https://example.com/bg.jpg" />
```

### 🔍 Search Menu Styling (WebView CSS)

Start Menu’nun arama bölümü WebView kullandığı için CSS ile styling yapılıyor:

### Örnek CSS Özelleştirmeleri

```css
/* Copilot butonunu gizle */#chatButtonRight { display: none !important; }
/* Arama başlıklarının arka planını değiştir */.scope-tile > div { background-color: Black !important; }
/* Arama sonuçlarının arka planı */.suggContainer { background-color: Black !important; }
/* Font değiştirme */h4, .suggContainer, .title { font-family: 'Inter' !important; }
```

### 🛠️ Force Light/Dark Mode

System ayarlarından bağımsız tema zorlaması:

```
RequestedTheme=1  <!-- Light Mode -->
RequestedTheme=2  <!-- Dark Mode -->
```

### 🎯 Pro Kullanım İpuçları

### Semantic Zoom Navigation

```
<!-- Alfabetik navigasyon aktif etme -->
Windows.UI.Xaml.Controls.SemanticZoom#ZoomControl:
IsZoomOutButtonEnabled=True

Windows.UI.Xaml.Controls.Button#ZoomOutButton:
Width=40
Height=40
```

### Performance & Debugging

```
🚀 Best Practices:
- 2D transformations için RenderTransform kullan
- 3D effects için Transform3D tercih et
- TransformGroup ile multiple transforms
- ResourceDictionary kullanarak reusable styles

🔍 Debug Tools:
- UWPSpy ile target finding
- XAML Live Visual Tree
- Property Inspector
```

### 📚 Öğrenme Kaynakları

- [**Ana styling guide**](https://github.com/ramensoftware/windows-11-start-menu-styling-guide/blob/main/README.md) - Kapsamlı dokümantasyon
- [**Tema koleksiyonu**](https://github.com/ramensoftware/windows-11-start-menu-styling-guide/tree/main/Themes) - 16 hazır tema
- [**Taskbar styling**](https://github.com/ramensoftware/windows-11-taskbar-styling-guide) - İlgili projeler
- [**Notification center styling**](https://github.com/ramensoftware/windows-11-notification-center-styling-guide) - Tamamlayıcı modlar

Bu mod, **Windows 11’in Start Menu’sunu** tamamen dönüştürmek isteyen kullanıcılar için en kapsamlı çözüm. Hazır temalarla hızlı başlangıç, XAML bilgisiyle sınırsız özelleştirme! 🚀🎨

- 📋 **Gelişmiş Mod Ayarları - Start Menu Styler JSON Konfigürasyonu**
    
    ```json
    {  "controlStyles[0].target": "Windows.UI.Xaml.Controls.Grid#UndockedRoot",  "controlStyles[0].styles[0]": "Visibility=Visible",  "controlStyles[0].styles[1]": "Width=450",  "controlStyles[0].styles[2]": "Margin=200,-10,0,0",  "controlStyles[1].target": "Windows.UI.Xaml.Controls.Grid#AllAppsRoot",  "controlStyles[1].styles[0]": "Visibility=Visible",  "controlStyles[1].styles[1]": "Width=290",  "controlStyles[1].styles[2]": "Transform3D:=<CompositeTransform3D TranslateX=\"-1100\" />",  "controlStyles[1].styles[3]": "Margin=180,0,-220,0",  "controlStyles[2].target": "Windows.UI.Xaml.Controls.Button#CloseAllAppsButton",  "controlStyles[2].styles[0]": "Visibility=Collapsed",  "controlStyles[3].target": "StartDocked.StartSizingFrame",  "controlStyles[3].styles[0]": "MinWidth=650",  "controlStyles[3].styles[1]": "MaxWidth=650",  "controlStyles[3].styles[2]": "MaxHeight=700",  "controlStyles[4].target": "Windows.UI.Xaml.Controls.Grid#ShowMoreSuggestions",  "controlStyles[4].styles[0]": "Visibility=Collapsed",  "controlStyles[5].target": "Windows.UI.Xaml.Controls.Button#ShowAllAppsButton",  "controlStyles[5].styles[0]": "Visibility=Collapsed",  "theme": "",  "resourceVariables[0].variableKey": "",  "resourceVariables[0].value": "",  "webContentStyles[0].target": "",  "webContentStyles[0].styles[0]": "",  "webContentCustomJs": "",  "disableNewStartMenuLayout": 0,  "styleConstants[0]": ""}
    ```
    
    **📝 Açıklama:**
    - `controlStyles[X].target`: XAML hedef elementi (Start Menu bileşenleri)
    - `controlStyles[X].styles[Y]`: XAML stil özellikleri
    - `webContentStyles`: Arama menüsü için CSS stilleri
    - `webContentCustomJs`: Custom JavaScript kodu
    - `disableNewStartMenuLayout`: Yeni layout’u devre dışı bırakma
    - `theme`: Tema ayarları
    
    **🎯 Örnek Hedefler:**
    - `StartDocked.SearchBoxToggleButton`: Arama kutusu
    - `StartMenu.PinnedList`: Sabitlenmiş uygulamalar
    - `Grid#TopLevelSuggestionsContainer`: Önerilen bölüm
    - `StartDocked.UserTileView`: Kullanıcı profili
    - `StartDocked.PowerOptionsView`: Güç seçenekleri
    
    **🔧 Kullanım:**
    1. Windhawk → Start Menu Styler → Settings
    2. JSON konfigürasyonunu yapıştırın
    3. XAML hedef ve stilleri düzenleyin
    4. Apply ile uygulayın
    

---

### ⚡ Windows 11 Taskbar Styler

**🔥 Taskbar’ı Tamamen Yeniden Tasarlama Modu**

Windows 11’in taskbar’ını XAML tabanlı styling sistemi ile köklü bir şekilde özelleştirmenizi sağlar. [Resmi GitHub styling guide](https://github.com/ramensoftware/windows-11-taskbar-styling-guide/blob/main/README.md#themes) referansında 16 adet hazır tema ve kapsamlı özelleştirme rehberi bulunuyor.

### 🎯 Ana Özellikler

| **Özellik** | **Açıklama** | **Teknik Detay** |
| --- | --- | --- |
| **XAML Styling** | Native Windows teknolojisi | Background, colors, transforms |
| **Ready-Made Themes** | 16 topluluk teması | WinXP, Bubbles, TranslucentTaskbar, vb. |
| **Task List Control** | Buton boyutu ve davranış | Icon size, corner radius, labels |
| **System Tray** | Notification area styling | Icon spacing, clock, network icons |
| **Visual Effects** | Acrylic, WindhawkBlur, gradients | Modern transparency effects |

### 🎨 Resmi Tema Koleksiyonu

[GitHub tema sayfasında](https://github.com/ramensoftware/windows-11-taskbar-styling-guide/blob/main/README.md#themes) bulunan hazır temalar:

| **Tema** | **Açıklama** | **Stil Kategorisi** |
| --- | --- | --- |
| [**WinXP**](https://github.com/ramensoftware/windows-11-taskbar-styling-guide/blob/main/Themes/WinXP/README.md) | Windows XP klasik taskbar | 🕰️ Retro Classic |
| [**TranslucentTaskbar**](https://github.com/ramensoftware/windows-11-taskbar-styling-guide/blob/main/Themes/TranslucentTaskbar/README.md) | Şeffaf cam efekti | 🌟 Glass & Transparency |
| [**Bubbles**](https://github.com/ramensoftware/windows-11-taskbar-styling-guide/blob/main/Themes/Bubbles/README.md) | Bubble-style butonlar | 🫧 Playful Design |
| [**DockLike**](https://github.com/ramensoftware/windows-11-taskbar-styling-guide/blob/main/Themes/DockLike/README.md) | macOS dock benzeri | 🍎 Mac-Inspired |
| [**Windows7**](https://github.com/ramensoftware/windows-11-taskbar-styling-guide/blob/main/Themes/Windows7/README.md) | Windows 7 Aero taskbar | 💎 Aero Glass |
| [**Squircle**](https://github.com/ramensoftware/windows-11-taskbar-styling-guide/blob/main/Themes/Squircle/README.md) | Rounded square design | 🔄 Modern Geometric |
| [**RosePine**](https://github.com/ramensoftware/windows-11-taskbar-styling-guide/blob/main/Themes/RosePine/README.md) | Aesthetic color palette | 🌹 Beautiful Colors |
| [**CleanSlate**](https://github.com/ramensoftware/windows-11-taskbar-styling-guide/blob/main/Themes/CleanSlate/README.md) | Minimal clean design | 🧹 Clean & Minimal |

### ⚙️ Temel Yapılandırma Kategorileri

### 1. General Taskbar Settings

[Resmi dokümantasyonda](https://github.com/ramensoftware/windows-11-taskbar-styling-guide/blob/main/README.md) bulunan temel ayarlar:

| **Hedef** | **XAML Target** | **Kullanım** |
| --- | --- | --- |
| **Taskbar Background** | `Rectangle#BackgroundFill` | `Fill=<color>` background |
| **Taskbar Border** | `Rectangle#BackgroundStroke` | Border styling |
| **Taskbar Size** | Taskbar height and icon size mod | Boyut ayarları |

### 2. Task List Customization

```
<!-- Start button özelleştirme -->
Target: Taskbar.ExperienceToggleButton#LaunchListButton
Style: Background:=<ImageBrush ImageSource="custom-logo.png" />

<!-- Task list buton corner radius -->
Target: Taskbar.TaskListButton
Style: CornerRadius=8

<!-- Running indicator -->
Target: Rectangle#RunningIndicator
Style: Fill=#FFED7014, Height=3, Width=16
```

### 3. System Tray (Notification Area)

```
<!-- Tray icon boyutu -->
Target: SystemTray.ImageIconContent > Grid#ContainerGrid > Image
Style: Width=20, Height=20

<!-- Clock özelleştirme -->
Taskbar Clock Customization mod kullan

<!-- Network/Volume iconlarını gizle -->
Target: SystemTray.OmniButton#ControlCenterButton > ... > ContentPresenter[1]
Style: Visibility=Collapsed
```

### 🎭 Gelişmiş Özelleştirme Teknikleri

### 1. Advanced Background Effects

```
<!-- Acrylic effect -->
Fill:=<AcrylicBrush TintColor="Black" TintOpacity="0.8" />

<!-- WindhawkBlur (özel blur implementation) -->
Fill:=<WindhawkBlur BlurAmount="10" TintColor="#80ff0000" />

<!-- Gradient background -->
Fill:=<LinearGradientBrush StartPoint="0,0.5" EndPoint="1,0.5">
    <GradientStop Color="Yellow" Offset="0.0" />
    <GradientStop Color="Red" Offset="0.25" />
    <GradientStop Color="Blue" Offset="0.75" />
</LinearGradientBrush>

<!-- Image background -->
Fill:=<ImageBrush Stretch="UniformToFill"
                  ImageSource="https://example.com/bg.jpg" />
```

### 2. Transform Effects

```
<!-- 2D Transformations (RenderTransform) -->
RenderTransform:=<TranslateTransform X="15" Y="-15" />
RenderTransform:=<RotateTransform Angle="15" />
RenderTransform:=<ScaleTransform ScaleX="1.5" ScaleY="1.5" />

<!-- 3D Transformations (Transform3D) -->
Transform3D:=<CompositeTransform3D ScaleX="1.5"
                                   TranslateY="-15"
                                   RotationZ="15" />

<!-- Combined transformations -->
RenderTransform:=<TransformGroup>
    <RotateTransform Angle="15" />
    <TranslateTransform X="15" Y="-15" />
</TransformGroup>
```

### 3. Color Schemes & Accent Integration

```
<!-- System accent colors -->
Fill:=<SolidColorBrush Color="{ThemeResource SystemAccentColor}"
                       Opacity="0.8" />

<!-- Accent color variations -->
Fill:=<SolidColorBrush Color="{ThemeResource SystemAccentColorLight2}" />
Fill:=<SolidColorBrush Color="{ThemeResource SystemAccentColorDark1}" />

<!-- Semi-transparent colors -->
Fill=#80FF0000  <!-- 50% transparent red -->
Fill=Transparent  <!-- Fully transparent -->
```

### 🔧 Hızlı Tema Kurulumu

```
🔧 Adım Adım:
1. Windhawk → "Windows 11 Taskbar Styler" modunu kur
2. İstediğiniz temayı GitHub'dan seç
3. Tema README'sindeki XAML kodunu kopyala
4. Mod Settings → XAML kodunu yapıştır → Apply
5. Taskbar değişikliklerini anında görün!
```

### 🎯 Pro Kullanım İpuçları

### Visual States & Hover Effects

```
<!-- Farklı durumlar için farklı stiller -->
Fill@ActiveRunningIndicator=Red
Width@ActiveRunningIndicator=20
Fill@InactiveRunningIndicator=Gray
Fill@RequestingAttentionRunningIndicator=Orange
```

### Performance Best Practices

```
🚀 Optimizasyon İpuçları:
- 2D transformations için RenderTransform kullan
- 3D effects için Transform3D tercih et
- WindhawkBlur, Acrylic'ten daha performanslı
- Single taskbar için en iyi sonuç

🔍 Debug Araçları:
- UWPSpy ile target finding
- Live preview ile real-time test
- Visual states explorer
```

### 📚 İlgili Modlar ve Kaynaklar

- [**Ana taskbar styling guide**](https://github.com/ramensoftware/windows-11-taskbar-styling-guide/blob/main/README.md) - Kapsamlı dokümantasyon
- [**Tema koleksiyonu**](https://github.com/ramensoftware/windows-11-taskbar-styling-guide/tree/main/Themes) - 16 hazır tema
- **Taskbar height and icon size** mod - Boyut ayarları
- **Taskbar Labels for Windows 11** mod - Text label’ları
- **Taskbar Clock Customization** mod - Saat özelleştirme

### ⚠️ Bilinen Limitasyonlar

```
🚨 Dikkat Edilecekler:
- Acrylic background sadece tek taskbar'da çalışır
- Taskbar Background Helper mod gerekebilir
- Windows updates sonrası kontrol edin
- Tema değişiklikleri explorer restart gerektirebilir
```

Bu mod, **Windows 11’in taskbar’ını** tamamen dönüştürmek isteyen kullanıcılar için en kapsamlı çözüm. Retro temalından modern glass efektlerine kadar her tarz mevcut! ⚡🎨

- 📋 **Gelişmiş Mod Ayarları - Taskbar Styler JSON Konfigürasyonu**
    
    ```json
    {  "theme": "TranslucentTaskbar",  "controlStyles[0].target": "",  "controlStyles[0].styles[0]": "",  "resourceVariables[0].variableKey": "",  "resourceVariables[0].value": "",  "styleConstants[0]": ""}
    ```
    
    **📝 Açıklama:**
    - `theme`: Hazır tema seçimi (TranslucentTaskbar, WinXP, Bubbles, vb.)
    - `controlStyles[X].target`: XAML hedef elementi (örn: `Taskbar.TaskListButton`)
    - `controlStyles[X].styles[Y]`: Stil özellikleri (örn: `CornerRadius=8`)
    - `resourceVariables`: Dinamik değişken tanımları
    - `styleConstants`: Sabit değer tanımları
    
    **🔧 Kullanım:**
    1. Windhawk → Taskbar Styler → Settings
    2. JSON konfigürasyonunu yapıştırın
    3. Hedef ve stilleri ihtiyacınıza göre düzenleyin
    4. Apply ile uygulayın
    

---

## 🎛️ Diğer Faydalı Modlar

### ⚡ Taskbar height and icon size

**Windows 11 Taskbar Boyut Kontrolü**
- Taskbar yüksekliğini istediğiniz gibi ayarlayın
- Icon boyutlarını küçültün/büyütün

- Icon kalitesini artırın
- Sadece Windows 11 için

### 🔊 Taskbar Volume Control

**Mouse Wheel ile Ses Kontrolü**
- Taskbar üzerinde mouse wheel ile ses ayarı
- Hızlı ve pratik ses kontrolü
- Klavye kısayollarına gerek yok

### 🕐 Taskbar Clock Customization

**Saat ve Tarih Özelleştirme**
- Özel tarih/saat formatı tanımlayın
- Haber akışı ekleyin
- Font ve renk özelleştirme
- İleri seviye saat özelleştirme

### 🪟 Slick Window Arrangement

**Akıllı Pencere Düzenleme**
- Pencere yerleştirmeyi kolaylaştırır
- Kayma animasyonu ve snapping
- Daha düzgün window management

### 🖱️ Middle click to close on the taskbar

**Orta Tık ile Kapatma**
- Taskbar’da middle click ile programları kapatın
- Yeni instance oluşturmak yerine kapatma
- Hızlı program yönetimi

### 🎨 Modernize Folder Picker Dialog

**Modern Klasör Seçici**
- Eski “Browse For Folder” diyaloğunu değiştirir
- Modern Windows 11 tasarımı
- Daha kullanıcı dostu arayüz

### 🚫 Disable grouping on the taskbar

**Taskbar Gruplama Kapatma**
- Her pencere için ayrı buton oluşturur
- Windows 7 tarzı taskbar davranışı
- Çoklu pencere yönetimi

### 🖤 Classic context menu on Windows 11

**Klasik Sağ Tık Menüsü**
- Windows 10 tarzı context menu
- “Show More Options” gerekmez
- Shift tutmaya gerek yok

### 📸 Taskbar Thumbnail Reorder

**Thumbnail Sıralama**
- Sol mouse butonu ile thumbnail’leri yeniden sıralayın
- Alt+Tab preview’ları organize edin
- Gelişmiş taskbar yönetimi

### 📐 Taskbar tray icon spacing

**Tray Icon Mesafesi**
- System tray iconları arasındaki mesafeyi ayarlayın
- Kompakt veya geniş düzen seçenekleri
- Sadece Windows 11

### 🌙 Dark Mode for Notepad

**Notepad Dark Mode**
- Notepad için eksik olan dark mode
- Gözleri yormayan karanlık tema
- Windows’un standart Notepad’i için

### ⬆️ Taskbar on top for Windows 11

**Üstte Taskbar**
- Windows 11 taskbar’ını ekranın üstüne taşır
- macOS benzeri üst panel deneyimi
- Farklı workflow tercihi

### 🙈 Taskbar auto-hide when maximized

**Akıllı Taskbar Gizleme**
- Sadece maximize edilmiş pencereler var iken gizler
- Normal durumlarda görünür kalır
- Daha akıllı auto-hide davranışı

### 📱 Vertical Taskbar for Windows 11

**Dikey Taskbar**
- Taskbar’ı ekranın sol/sağına taşır
- Dikey panel deneyimi
- Ultrawide monitörler için ideal

### 🌚 Dark mode context menus

**Karanlık Sağ Tık Menüleri**
- Tüm win32 menüler için dark mode
- Sistem genelinde tutarlı karanlık tema
- Win32 uygulamaları dahil

### 🪟 Translucent Windows

**Şeffaf Pencereler**
- Windows 11’de native translucent effects
- Pencere transparanlık efektleri
- Modern cam görünümü

### 🔲 No Focus Rectangle

**Odak Çerçevesi Kaldırma**
- Focus rectangle’ları kaldırır
- Daha temiz arayüz görünümü
- Görsel gürültüyü azaltır

### ⚠️ Turn off change file extension warning

**Dosya Uzantısı Değiştirme Uyarısını Kapat**
- Dosya uzantısı değiştirildiğinde çıkan uyarıyı kaldırır
- Tekrarlayan onay diyaloglarından kurtulun
- Daha hızlı dosya işlemleri

### 🖱️ Click on empty taskbar space

**Boş Taskbar Alanına Tıklama**
- Taskbar’ın boş alanına double/middle click ile özel eylemler
- Desktop gösterme, run dialog açma gibi işlemler
- Hızlı erişim kısayolları

### 🏪 Open With - Remove Microsoft Store Menu Item

**Microsoft Store Menü Öğesini Kaldır**
- “Open with” menüsünden “Search with Microsoft Store” seçeneğini kaldırır
- Daha temiz context menu
- Gereksiz Store önerilerinden kurtulma

### 🧭 Classic Explorer navigation bar

**Klasik Explorer Navigasyon Çubuğu**
- Windows 11 “Moments 4” güncellemesi öncesi navigation bar’ı geri getirir
- Eski Explorer deneyimi
- Klasik breadcrumb navigasyon

### 🎨 Windows 11 File Explorer Styler

**File Explorer Stil Değiştirici**
- Explorer’a özel temalar uygulayın
- Topluluk temaları veya kendi temanızı oluşturun
- Dosya gezgini görsel özelleştirme

### ⚡ Taskbar auto-hide speed

**Taskbar Gizlenme Hızı**
- Auto-hide taskbar’ın hızını ve frame rate’ini özelleştirin
- Daha hızlı gizlenme/görünme animasyonu
- Lag hissini azaltma

### 🔔 Customize Windows notifications placement

**Bildirim Yerleşimini Özelleştir**
- Bildirimleri farklı monitöre veya ekran köşesine taşıyın
- Çok monitör kurulumları için ideal
- Bildirim konumu kontrolü

### ⬅️ Start button always on the left

**Start Butonu Her Zaman Solda**
- Start butonunu taskbar’ın solunda sabitler
- Center taskbar icons olsa bile sol pozisyon
- Windows 11 sadece

### 🖥️ Alt+Tab per monitor

**Monitör Başına Alt+Tab**
- Alt+Tab’ı sadece aktif monitördeki pencereler için çalıştırır
- Çok monitör düzeni için optimize
- Daha verimli pencere değiştirme

### 🔄 Better Taskbar Autohide

**Gelişmiş Taskbar Gizleme**
- Inactive window bildirimi geldiğinde taskbar gizlenmesine izin verir
- Daha akıllı auto-hide davranışı
- Notification handling

### 🚫 Disable Feedback Hub Hotkey

**Feedback Hub Kısayolunu Devre Dışı Bırak**
- Win+F kısayolunu (Feedback Hub) devre dışı bırakır
- Kazara açılma problemini çözer
- Temiz hotkey deneyimi

### 📱 Show all apps by default in start menu

**Start Menüsünde Varsayılan Tüm Uygulamalar**
- Windows 11 start menüsü açıldığında direkt tüm uygulamaları gösterir
- “All apps” butonuna tıklama gerekmez
- Hızlı uygulama erişimi

### 👁️ Always show all taskbar tray icons

**Tüm Tray Iconlarını Her Zaman Göster**
- Eksik Windows seçeneğini geri getirir
- Tüm notification (tray) iconlarını gösterir
- Windows 11 sadece

### 🎨 Taskbar Background Helper

**Taskbar Arkaplan Yardımcısı**
- Şeffaf kısımlar için taskbar arkaplanı ayarlar
- Windows 11 Taskbar Styler ile birlikte kullanım
- Always/sadece maximize pencere durumlarında

### ⭕ Disable rounded corners in Windows 11

**Windows 11’de Yuvarlatılmış Köşeleri Kapat**
- Pencere yuvarlatılmış köşelerini devre dışı bırakır
- Klasik kare köşe görünümü
- Windows 11 için basit mod

### 📁 Remove File Explorer Suffixes

**File Explorer Son Eklerini Kaldır**
- Windows’un eklediği “- File Explorer” son eklerini kaldırır
- Taskbar’da her klasör için ayrı buton
- Temiz taskbar görünümü

### 🌙 Fix Darkmode ListViews

**Dark Mode Liste Görünümlerini Düzelt**
- Dark mode’da ListView’ları düzeltir
- Tam dark theme tutarlılığı
- Windows Explorer iyileştirmesi

### 🔊 Logon, Logoff & Shutdown Sounds Restored

**Giriş, Çıkış ve Kapanma Seslerini Geri Getir**
- Windows’un eski sürümlerindeki sistem seslerini geri getirir
- Nostaljik Windows deneyimi
- Login/logout/shutdown sound effects

### 🖼️ Disable Taskbar Thumbnails

**Taskbar Thumbnail’larını Devre Dışı Bırak**
- Hover’da taskbar thumbnail’larını devre dışı bırakır
- Veya liste ile değiştirir
- Performance iyileştirmesi

### 🎨 UXTheme hook

**UXTheme Kancası**
- Özel temalar uygulamanızı sağlar
- Advanced theming sistemi
- 3. parti tema desteği

### 🎵 CEF/Spotify Tweaks

**CEF/Spotify İyileştirmeleri**
- Spotify için çeşitli iyileştirmeler
- Native frame’ler, şeffaf pencereler ve daha fazlası
- Spotify kullanıcı deneyimi

### 🔄 Cycle taskbar buttons with mouse wheel

**Mouse Wheel ile Taskbar Buton Geçişi**
- Mouse wheel ve/veya klavye kısayolları ile taskbar butonları arasında geçiş
- Hızlı program değiştirme
- Efficiency mod

---

*Windhawk açık kaynak bir projedir ve topluluk katkılarına açıktır. Geliştirme sürecine katılmak için GitHub repository’sini ziyaret edin.*

*⚠️ Dikkat: Windhawk sistem dosyalarında değişiklik yapar. Kullanmadan önce sistem yedeklemesi almanız önerilir.*