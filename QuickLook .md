# QuickLook

# QuickLook: Windows’ta macOS Hızı

## 🔍 Genel Bakış

QuickLook, macOS’un ikonik “Quick Look” özelliğini Windows işletim sistemine taşıyan devrim niteliğinde bir dosya önizleme aracıdır. Paddy Xu tarafından geliştirilen bu açık kaynaklı uygulama, tek bir tuş vuruşuyla (Space) herhangi bir dosyanın içeriğini anında görüntüleme imkanı sunarak, Windows kullanıcılarının verimliliğini dramatik şekilde artırmaktadır.

### 🎯 Geliştirme Felsefesi

QuickLook’un yaratılış hikayesi, bir geliştiricinin macOS’tan Windows’a geçiş yaparken hissettiği eksiklikten doğmuştur. macOS’un en beğenilen özelliklerinden biri olan Quick Look’un Windows’ta bulunmaması, dosya yönetimi konusunda ciddi bir verimlilik kaybına neden olmaktaydı. Bu boşluğu doldurmak amacıyla başlayan proje, kısa sürede Windows ekosisteminin vazgeçilmez araçlarından biri haline gelmiştir.

---

## **📥 İndirme ve Kurulum**

### **🔗 Ana Uygulama İndirme Bağlantıları**

| İndirme Türü | Bağlantı | Açıklama |
| --- | --- | --- |
| **GitHub MSI (ÖNERİLEN)** | 🔗 [GitHub Releases](https://github.com/QL-Win/QuickLook/releases/latest) | Tam özellikli, en kararlı sürüm |
| **Microsoft Store** | 🔗 [Microsoft Store](https://www.microsoft.com/store/apps/9NV4BS3L1H4S) | Kolay kurulum, sınırlı özellikler |
| **Portable ZIP** | 🔗 [GitHub Releases](https://github.com/QL-Win/QuickLook/releases/latest) | Kurulum gerektirmez |
| **Scoop Paket Yöneticisi** | `scoop bucket add extras && scoop install extras/quicklook` | Komut satırı kurulum |
| **Nightly Builds** | 🔗 [AppVeyor](https://ci.appveyor.com/project/xupefei/quicklook) | En yeni düzeltmeler |

### **🔌 Popüler Plugin İndirme Bağlantıları**

| Plugin | Direkt İndirme | Açıklama |
| --- | --- | --- |
| **OfficeViewer** | 🔗 [.qlplugin](https://github.com/QL-Win/QuickLook.Plugin.OfficeViewer/releases/latest) | Office dosyaları (Office kurulumsuz) |
| **OfficeViewer-Native** | 🔗 [.qlplugin](https://github.com/QL-Win/QuickLook.Plugin.OfficeViewer-Native/releases/latest) | Office dosyaları (Office gerekli) |
| **EpubViewer** | 🔗 [.qlplugin](https://github.com/QL-Win/QuickLook.Plugin.EpubViewer/releases/latest) | E-kitap önizleme |
| **PdfViewer-Native** | 🔗 [.qlplugin](https://github.com/QL-Win/QuickLook.Plugin.PdfViewer-Native/releases/latest) | WebView2 tabanlı PDF görüntüleme |
| **FolderViewer** | 🔗 [.qlplugin](https://github.com/QL-Win/QuickLook.Plugin.FolderViewer/releases/latest) | Klasör içerik listesi |
| **ApkViewer** | 🔗 [.qlplugin](https://github.com/QL-Win/QuickLook.ApkReader/releases/latest) | Android APK bilgileri |
| **FontViewer** | 🔗 [.qlplugin](https://github.com/QL-Win/QuickLook.Plugin.FontViewer/releases/latest) | Font dosyaları (Win11'de dikkatli) |
| **FitsViewer** | 🔗 [.qlplugin](https://github.com/QL-Win/QuickLook.Plugin.FitsViewer/releases/latest) | Astronomi FITS formatı |

📋 **Tüm Plugin'ler**: [QL-Win Organization](https://github.com/QL-Win) sayfasında tam liste

---

## **🚀 Hızlı Başlangıç Rehberi**

### **1️⃣ Ana Uygulamayı Kurun**

```bash
# Önerilen: GitHub MSI sürümü
https://github.com/QL-Win/QuickLook/releases/latest

# Alternatif: Scoop ile
scoop install extras/quicklook

```

### **2️⃣ Temel Plugin'leri Kurun**

```bash
# 🏢 Office dosyaları için (seçeneklerden birini)
OfficeViewer: https://github.com/QL-Win/QuickLook.Plugin.OfficeViewer/releases/latest
OfficeViewer-Native: https://github.com/QL-Win/QuickLook.Plugin.OfficeViewer-Native/releases/latest

# 📚 E-kitaplar için
EpubViewer: https://github.com/QL-Win/QuickLook.Plugin.EpubViewer/releases/latest

# 📁 Klasör içerikleri için
FolderViewer: https://github.com/QL-Win/QuickLook.Plugin.FolderViewer/releases/latest

# 🔤 Font dosyaları için
FontViewer: https://github.com/QL-Win/QuickLook.Plugin.FontViewer/releases/latest

```

### **3️⃣ Kullanmaya Başlayın**

1. Herhangi bir dosyayı seçin
2. **Space** tuşuna basın
3. Önizlemeyi kapatmak için tekrar **Space** veya **Esc**

## ⚡ Çalışma Mantığı ve Kullanım

### Temel Kullanım Akışı

1. **Dosya Seçimi**: Herhangi bir dosyayı seçin (Masaüstü, File Explorer, Aç/Kaydet dialogları)
2. **Önizleme**: Space tuşuna basın
3. **İnceleme**: Dosya içeriğini anında görüntüleme
4. **Navigasyon**: Ok tuşları ile diğer dosyalara geçiş
5. **Kapama**: Space, Esc tuşu veya X butonuyla kapatma

### 🎮 Klavye Kısayolları

| Kısayol | İşlev | Açıklama |
| --- | --- | --- |
| **Space** | Göster/Gizle | Önizleme penceresini aç/kapat |
| **Esc** | Gizle | Önizleme penceresini kapat |
| **Enter** | Aç/Çalıştır | Dosyayı varsayılan uygulamayla aç |
| **↑ ↓ ← →** | Navigasyon | Diğer dosyalara geçiş |
| **Mouse Wheel** | Yakınlaştır/Uzaklaştır | Görüntüler için zoom |
| **Ctrl + Wheel** | PDF Zoom | PDF dosyaları için zoom |
| **Wheel** | Ses Kontrolü | Video dosyalarında ses seviyesi |

---

## 📁 Desteklenen Dosya Formatları

### 🖼️ Görüntü Formatları

- **Temel Formatlar**: PNG, JPG/JPEG, BMP, GIF, TIFF
- **RAW Formatlar**: CR2, NEF, ARW, DNG (Plugin ile)
- **Vektör Formatlar**: SVG, AI (Plugin ile)
- **Özel Formatlar**: PSD, XCF, WebP

### 📄 Belge Formatları

- **PDF**: Yerleşik yüksek kaliteli görüntüleme
- **Microsoft Office**: Word (DOC/DOCX), Excel (XLS/XLSX), PowerPoint (PPT/PPTX)
- **Metin Dosyaları**: TXT, RTF, HTML, XML, JSON
- **Markup**: Markdown (MD), LaTeX

### 🎬 Medya Formatları

- **Video**: MP4, AVI, MKV, WMV, MOV, M2TS, WEBM
- **Ses**: MP3, WAV, FLAC, OGG, AAC, WMA
- **Codec Desteği**: FFmpeg tabanlı geniş codec desteği

### 🗜️ Arşiv Formatları

- **Sıkıştırma**: ZIP, RAR, 7Z, TAR, GZ, BZ2
- **İçerik Önizleme**: Arşiv içeriğini açmadan görüntüleme
- **Çoklu Format**: Nested arşivler desteği

### 💻 Geliştirici Dosyaları

- **Kaynak Kod**: C, C++, C#, Java, Python, JavaScript, TypeScript
- **Web**: HTML, CSS, SCSS, LESS
- **Konfigürasyon**: JSON, YAML, XML, INI
- **Sözdizimi Vurgulama**: 50+ programlama dili

## **🔌 Plugin Ekosistemi**

### **Resmi Plugin'ler ve Kritik Bağımlılıklar**

QuickLook'un gerçek gücü plugin ekosisteminde yatmasına rağmen, en popüler plugin'lerde önemli lisanslama karmaşıklıkları bulunmaktadır.

| Plugin Adı | Temel İşlev | Desteklenen Dosya Türleri | Bağımlılıklar ve Lisans | İndirme Bağlantısı | Analist Notu |
| --- | --- | --- | --- | --- | --- |
| **OfficeViewer** | Office kurulumu gerektirmeden Office dosyalarını önizler | .docx, .xlsx, .pptx | Ticari Syncfusion bileşenlerine dayanır; eklenti MIT lisanslıdır | 🔗 [GitHub Releases](https://github.com/QL-Win/QuickLook.Plugin.OfficeViewer/releases) | MS Office kurulu değilse bu seçeneği tercih edin. Görüntüleme doğruluğu Native sürümden daha düşük olabilir |
| **OfficeViewer-Native** | Yerel MS Office veya WPS Office kurulumunu kullanarak Office dosyalarını önizler | .docx, .xlsx, .pptx | Yerel MS Office/WPS Office kurulumu gerektirir; MIT lisanslıdır | 🔗 [GitHub Releases](https://github.com/QL-Win/QuickLook.Plugin.OfficeViewer-Native/releases) | MS Office kuruluysa en iyi görüntüleme doğruluğu için önerilir |
| **PdfViewer-Native** | WebView2 tabanlı PDF görüntüleme | PDF, AI dosyaları | Microsoft WebView2 gerektirir | 🔗 [GitHub Releases](https://github.com/QL-Win/QuickLook.Plugin.PdfViewer-Native/releases) | Yerleşik PDF viewer'a alternatif |
| **EpubViewer** | EPUB formatındaki e-kitapları önizler ve okunmasını sağlar | .epub | Bağımsız; MIT lisanslıdır | 🔗 [GitHub Releases](https://github.com/QL-Win/QuickLook.Plugin.EpubViewer/releases) | Dijital kitaplıkları yöneten kullanıcılar için vazgeçilmez |
| **FitsViewer** | Astronomide kullanılan FITS görüntü formatını önizler | .fits, .fit | Bağımsız; LGPL-2.1 lisanslıdır | 🔗 [GitHub Releases](https://github.com/QL-Win/QuickLook.Plugin.FitsViewer/releases) | Astronomi ile ilgilenenler için son derece niş ve değerli |
| **FolderViewer** | Klasörlerin içeriğini bir liste olarak önizler | Klasörler | Bağımsız | 🔗 [GitHub Releases](https://github.com/QL-Win/QuickLook.Plugin.FolderViewer/releases) | Varsayılan klasör meta verilerine ek olarak dosya listesini gösterir |
| **ApkViewer** | Android APK dosyalarının meta bilgilerini önizler | .apk | Bağımsız | 🔗 [GitHub Releases](https://github.com/QL-Win/QuickLook.ApkReader/releases) | APK simgesi, sürüm, izinler gibi bilgileri gösterir |
| **FontViewer** | Font dosyalarını önizler | .ttf, .otf, .woff | Bağımsız | 🔗 [GitHub Releases](https://github.com/QL-Win/QuickLook.Plugin.FontViewer/releases) | ⚠️ Windows 11'de kararlılık sorunları bildirildi |
| **VideoViewer** | Video dosyaları için gelişmiş önizleme | Çoğu video formatı | FFmpeg | 🔗 [GitHub Releases](https://github.com/QL-Win/QuickLook.Plugin.VideoViewer/releases) | Thumbnail oluşturma ve meta veri gösterimi |

### Plugin Kurulum Süreci

1. **İndirme**: `.qlplugin` formatında plugin dosyasını indirin
2. **Kurulum**: QuickLook çalışırken dosyayı seçip Space tuşuna basın
3. **Onay**: “Install” butonuna tıklayın
4. **Yeniden Başlatma**: QuickLook’u yeniden başlatın

## **📦 Plugin Kurulum Süreci**

### **Hızlı Kurulum Adımları**

1. **İndirme**: Yukarıdaki tablodaki bağlantılardan `.qlplugin` dosyasını indirin
2. **Kurulum**: QuickLook çalışırken dosyayı seçip **Space** tuşuna basın
3. **Onay**: Açılan önizleme penceresinde "**Install**" butonuna tıklayın
4. **Yeniden Başlatma**: QuickLook'u sistem tepsisinden yeniden başlatın

### **🔧 Alternatif Kurulum Yöntemleri**

**Manuel Kurulum:**

```
# Plugin klasörüne kopyalama
copy "plugin.qlplugin" "%APPDATA%\QuickLook\QuickLook.Plugin.{PluginName}\"

```

**Plugin Listesi Kontrolü:**

- Sistem tepsisi → QuickLook → "Plugin Manager" → Kurulu plugin'leri görüntüle

### **💡 Pro Tips**

- **Toplu Kurulum**: Birden fazla `.qlplugin` dosyasını seçip Space tuşuyla toplu kurulum yapabilirsiniz
- **Plugin Güncelleme**: Yeni sürüm çıktığında eski plugin üzerine kurulum yapın
- **Sorun Giderme**: Plugin çalışmıyorsa `%APPDATA%\QuickLook\` klasöründen ilgili plugin klasörünü silin

---

## **🎨 Arayüz ve Deneyim**

### Fluent Design Language

QuickLook, Microsoft’un modern Fluent Design dil öğelerini benimser:
- **Acrylic Effects**: Şeffaf ve bulanık arka plan efektleri
- **Smooth Animations**: Akıcı geçiş animasyonları
- **Adaptive Layout**: İçeriğe göre otomatik boyutlandırma
- **Context Awareness**: Dosya türüne göre optimize edilmiş arayüz

### 📱 Dokunmatik Ekran Desteği

- **Gesture Navigation**: Parmak hareketleri ile gezinme
- **Pinch to Zoom**: Yakınlaştırma/uzaklaştırma
- **Touch Scrolling**: Dokunmatik kaydırma
- **Modern UI Elements**: Dokunmatik kullanım için optimize edilmiş butonlar

### 🔍 HiDPI ve 4K Desteği

- **Automatic Scaling**: Otomatik DPI ölçeklendirme
- **Sharp Rendering**: Yüksek çözünürlüklü görüntü rendering
- **Multi-Monitor**: Çoklu monitör konfigürasyonları
- **Adaptive Quality**: Performans optimizasyon algoritmaları
    
    ### QuickLook’un Güçlü Yönleri
    
    - ✅ **Açık Kaynak Güvenilirliği**: Tam kod şeffaflığı
    - ✅ **Zengin Plugin Ekosistemi**: Sürekli genişleyen format desteği
    - ✅ **Aktif Geliştirme**: Düzenli güncellemeler ve yeni özellikler
    - ✅ **Topluluk Desteği**: Geniş kullanıcı ve geliştirici topluluğu
    - ✅ **Ücretsiz Kullanım**: Hiçbir lisans ücreti yok
    
    ### Sınırlılıklar ve Çözüm Önerileri
    
    - ❌ **Office Plugin Karmaşıklığı**: Harici plugin kurulumu gerekiyor
        - 💡 **Çözüm**: OfficeViewer plugin’ini kurun
    - ❌ **Büyük Dosya Performansı**: 100MB+ dosyalarda yavaşlama
        - 💡 **Çözüm**: MaxPreviewSize ayarını düşürün
    - ❌ **Bazı Exotic Formatlar**: Çok nadir formatlarda destek yok
        - 💡 **Çözüm**: Topluluk plugin’lerini kontrol edin

## 🐛 Sorun Giderme ve SSS

### 🚨 Windows 11 Kritik Sorunları

### Windows 11 Performans ve Görüntüleme Hataları

**Rapor Edilen Sorunlar:**
- Şiddetli gecikme ve donmalar
- Hatalı açılan önizleme pencereleri
- İmleç takılması
- Şeffaflık efektlerinde görüntüleme kusurları
- Microsoft Store sürümünde arka plan servisinin durması

**Kök Neden:** Windows 11’in değişen görüntüleme API’leri, özellikle bozuk `SetWindowCompositionAttribute` fonksiyonu.

**Geçici Çözümler:**

```
# %APPDATA%\QuickLook\user_config.ini dosyasına ekleyin
[Appearance]
UseTransparency=false
EnableAcrylicEffect=false
```

**Kalıcı Çözüm:** GitHub’dan Nightly build kurun veya en güncel kararlı sürüme geçin.

### ⚠️ Yaygın Sorunlar ve Çözümleri

### 1. QuickLook Başlamıyor

**Belirtiler**: Uygulama açılmıyor, sistem tepsisinde görünmüyor

**Teşhis Adımları:**

```powershell
# .NET Framework kontrol
Get-ItemProperty "HKLM:\SOFTWARE\Microsoft\NET Framework Setup\NDP\v4\Full\" -Name Release

# Windows Defender istisna ekleme
Add-MpPreference -ExclusionPath "C:\Program Files\QuickLook"
```

**Çözümler:**
- **Yönetici hakları**: Admin olarak çalıştırın
- **.NET Framework**: 4.7.2+ sürümünü kurun
- **Güvenlik yazılımı**: İstisna listesine ekleyin
- **Store sürümü sorunu**: GitHub MSI sürümüne geçin

### 2. Güvenlik Uyarısı: “Truva Atı” False Positive

**Durum:** Windows Defender “Fuery.B!cl” Truva atı uyarısı

**Açıklama:**
- Bu bir yanlış pozitiftir (2020’de yaşandı)
- `SetWindowsHookEx` fonksiyonu nedeniyle tetiklenir
- Aç/Kaydet dialog entegrasyonu için gereklidir

**Çözüm:**

```
# Windows Defender istisna ekleme
powershell Add-MpPreference -ExclusionProcess "QuickLook.exe"
powershell Add-MpPreference -ExclusionProcess "Wow64HookHelper.exe"
```

### 3. Çoklu Monitör DPI Sorunları

**Belirtiler**: Yanlış monitörde devasa boyutlarda açılan pencere

**Çözüm:**

```
# user_config.ini
[Display]
DPIAware=true
PerMonitorDPI=true
```

### 4. Space Tuşu Çalışmıyor

**Belirtiler**: Space tuşuna basılıyor ama önizleme açılmıyor

**Teşhis ve Çözüm:**
- **Focus kontrolü**: File Explorer’a tıklayıp odağı verin
- **Hotkey çakışması**: Başka uygulama Space tuşunu ele geçirmiş olabilir
- **Alternatif yöntem**: Sağ tık menüsünden “QuickLook” kullanın
- **Everything uygulaması**: Search box focus’tayken çakışma yaşanabilir

### 5. Plugin Kararlılık Sorunları

**Belirtiler**: Belirli dosya türlerinde çökmeler

**Yaygın Problemler:**
- **FontViewer**: Windows 11’de kararsız
- **RAW görüntüler**: Dikey RAW dosyalarında sorun
- **Office plugin**: Syncfusion bağımlılığı nedeniyle hata

**Çözümler:**

```bash
# Plugin temizleme
%APPDATA%\QuickLook\QuickLook.Plugin.{PluginName}
# Plugin klasörünü silin ve yeniden kurun
```

### ❓ Sık Sorulan Sorular

**S: QuickLook ücretsiz mi?**
C: Evet, tamamen ücretsiz ve açık kaynaklı. GPL-3.0 lisansı altında dağıtılıyor.

**S: Windows 11’de çalışıyor mu?**
C: Evet, Windows 7’den Windows 11’e kadar tüm sürümlerde çalışıyor.

**S: Office dosyalarını görmek için Microsoft Office gerekli mi?**
C: Hayır, OfficeViewer plugin’i ile Office kurulmadan da görüntüleyebilirsiniz.

**S: Kendi plugin’imi nasıl geliştirebilirim?**
C: GitHub wiki’deki “Plugin Development Guide”ı takip edebilirsiniz.

**S: Kurumsal ortamda kullanabilir miyim?**
C: Evet, MSI installer ile toplu kurulum yapabilirsiniz.

---

---

**🔗 Ana İndirme Sayfası**: [QuickLook GitHub](https://github.com/QL-Win/QuickLook/releases)

**🔌 Tüm Plugin'ler**: [QL-Win Organization](https://github.com/QL-Win)

*"QuickLook - Windows'ta macOS hızını yaşayın, tek tuş ile her şeyi önizleyin."*