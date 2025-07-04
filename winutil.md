# winutil

# Chris Titus Tech Windows Utility

---

## 🎯 Genel Bakış

### Araç Hakkında

Chris Titus Tech Windows Utility (WinUtil), Windows sistemlerini optimize etmek, gereksiz yazılımları kaldırmak ve gizlilik ayarlarını yapılandırmak için geliştirilmiş kapsamlı bir araçtır. Chris Titus Tech tarafından geliştirilen bu araç, Windows kullanıcılarının sistemlerini daha verimli, güvenli ve kullanıcı dostu hale getirmelerine yardımcı olur.

### Temel Özellikler

- ✅ **Otomatik Uygulama Kurulumu**: Popüler yazılımları toplu olarak kurma
- ✅ **Sistem Optimizasyonu**: Performans artırıcı tweaklar
- ✅ **Gizlilik Koruması**: Telemetri ve takip özelliklerini devre dışı bırakma
- ✅ **Bloatware Temizliği**: Gereksiz uygulamaları kaldırma
- ✅ **Özel ISO Oluşturma**: MicroWin ile optimize edilmiş Windows ISO’ları
- ✅ **PowerShell Entegrasyonu**: Gelişmiş komut satırı desteği
    
    

---

## 🚀 Kurulum ve Başlangıç

### Kurulum Yöntemleri

### 1️⃣ PowerShell ile Hızlı Kurulum (Önerilen)

```powershell
irm "https://christitus.com/win" | iex
```

### 2️⃣ Winget ile Kurulum

```
winget install ChrisTitusTech.WinUtil
```

### 3️⃣ Manuel Kurulum

1. GitHub Releases sayfasından en son sürümü indirin: https://github.com/ChrisTitusTech/winutil/releases
2. ZIP dosyasını çıkarın
3. PowerShell ile çalıştırın:

```powershell
.\winutil.ps1
```

### ⚠️ Güvenlik Uyarıları

**⚠️ DİKKAT**: Bu araç sistem dosyalarında değişiklik yapar. Kullanmadan önce:
- Sistem yedeklemesi alın
- Geri yükleme noktası oluşturun
- Önemli dosyalarınızı yedekleyin

### Güvenlik Kontrolü:

- ✅ Geri yükleme noktası oluşturun
- ✅ Önemli dosyalarınızı yedekleyin
- ✅ Sistem özelliklerini not alın

## 💻 Install Sekmesi - Uygulama Yönetimi

Install sekmesi, popüler yazılımları kategoriler halinde gruplandırarak toplu kurulum imkanı sunar.

### 🎛️ Actions (Eylemler)

Install sekmesinin sol panelinde bulunan temel eylem düğmeleri:

| Eylem | Açıklama | Kullanım Senaryosu |
| --- | --- | --- |
| **Install/Upgrade Applications** | Seçili uygulamaları kurar veya günceller | Yeni yazılım kurulumu |
| **Uninstall Applications** | Seçili uygulamaları kaldırır | Sistem temizliği |
| **Upgrade all Applications** | Tüm kurulu uygulamaları günceller | Sistem bakımı |

### Kullanım Örneği:

### 📦 Package Manager

WinUtil iki farklı paket yöneticisi desteği sunar:

| Package Manager | Açıklama | Avantajlar | Dezavantajlar |
| --- | --- | --- | --- |
| **Winget** (Varsayılan) | Microsoft’un resmi paket yöneticisi | ✅ Resmi destek✅ Güvenilir✅ Hızlı | ⚠️ Daha az uygulama |
| **Chocolatey** | Topluluk tabanlı paket yöneticisi | ✅ Geniş uygulama desteği✅ Uzun geçmiş | ⚠️ 3. parti⚠️ Güvenlik riski |

### ✅ Selection (Seçim Yönetimi)

Uygulama seçimini yönetmek için araçlar:

| Özellik | Açıklama | Kullanım Amacı |
| --- | --- | --- |
| **Clear Selection** | Tüm seçimleri temizle | Yeni seçim başlatma |
| **Get Installed** | Kurulu uygulamaları listele | Mevcut durumu görme |
| **Selected Apps: 0** | Seçili uygulama sayısı | İlerleme takibi |

**Tipik kullanım adımları:**
1. Kategori seç (Browsers, Development, etc.)
2. İstenen uygulamaları işaretle
3. “Selected Apps” sayısını kontrol et
4. Package Manager seç
5. Kurulum eylemini başlat

### 🔄 Toplu İşlem Özellikleri

### Kurulum Stratejileri:

| Strateji | Açıklama | Öneri |
| --- | --- | --- |
| **Kategori Bazlı** | Tüm kategoriyi seç | Yeni sistem kurulumu |
| **Seçici Kurulum** | Sadece gerekli uygulamalar | Mevcut sistem optimizasyonu |
| **Güncelleme Odaklı** | “Upgrade all Applications” | Düzenli bakım |

## ⚙️ Tweaks Sekmesi - Sistem Optimizasyonu

Tweaks sekmesi, Windows sisteminin davranışını değiştiren çeşitli ayarları içerir. İki ana buton ile tweakları uygulayabilir veya geri alabilirsiniz.

### 🔧 Essential Tweaks (Temel Düzenlemeler)

### Sistem Güvenliği ve Koruma:

| Tweak | Açıklama | Fayda | Risk |
| --- | --- | --- | --- |
| **Create Restore Point** | Sistem geri yükleme noktası oluşturur | Güvenlik backup’ı | 🟢 Yok |
| **Delete Temporary Files** | Geçici dosyaları ve cache’leri temizler | Disk alanı kazanımı | 🟢 Yok |

### Gizlilik ve Veri Koruması:

| Tweak | Açıklama | Etki | Öneri |
| --- | --- | --- | --- |
| **Disable Consumer Features** | Microsoft Store önerilerini kapatır | Reklam temizliği | ✅ Önerilen |
| **Disable Telemetry** | Microsoft’a veri gönderimi durdurur | Gizlilik artışı | ✅ Önerilen |
| **Disable Activity History** | Aktivite takibi kapatır | Gizlilik koruması | ✅ Önerilen |

### Dosya Sistemi ve Gezgin:

| Tweak | Açıklama | Kullanım |
| --- | --- | --- |
| **Disable Explorer Automatic Folder Discovery** | Otomatik klasör keşfini kapatır | Performans |
| **Disable Location Tracking** | Konum takibini devre dışı bırakır | Gizlilik |
| **Disable Storage Sense** | Otomatik disk temizliği kapatır | Manuel kontrol |

### Oyun ve Multimedya:

| Tweak | Açıklama | Hedef Grup |
| --- | --- | --- |
| **Disable GameDVR** | Xbox oyun kaydedicisini kapatır | Gamers |
| **Disable Hibernation** | Hibernate modunu devre dışı bırakır | Disk alanı |
| **Disable Homegroup** | Ev grubu özelliğini kapatır | Ağ optimizasyonu |

### Güvenlik ve Ağ:

| Tweak | Açıklama | Önem |
| --- | --- | --- |
| **Disable Wifi Sense** | WiFi şifre paylaşımını kapatır | Güvenlik |
| **Enable End Task With Right Click** | Sağ tık ile görev sonlandırma | Kullanılabilirlik |
| **Run Disk Cleanup** | Disk temizliği çalıştır | Performans |

### Terminal ve Sistem:

| Tweak | Açıklama | Hedef |
| --- | --- | --- |
| **Change Windows Terminal default: PowerShell 5 > PowerShell 7** | Modern PowerShell varsayılan yap | Geliştiriciler |
| **Disable PowerShell 7 Telemetry** | PowerShell telemetrisini kapat | Gizlilik |
| **Disable Recall** | AI recall özelliğini kapat | Gizlilik |

### Özel Ayarlar:

| Tweak | Açıklama | Kullanım Amacı |
| --- | --- | --- |
| **Set Hibernation as default (good for laptops)** | Laptop’lar için hibernate varsayılan | Enerji tasarrufu |
| **Set Services to Manual** | Servisleri manuel başlatma yap | Sistem kontrolü |
| **Debloat Edge** | Microsoft Edge’i temizle | Performans |

### ⚠️ Advanced Tweaks - CAUTION (Gelişmiş - Dikkat)

**⚠️ UYARI**: Bu bölümdeki tweaklar sistem kararlılığını ciddi şekilde etkileyebilir!

### Adobe İlgili Tweaklar:

| Tweak | Açıklama | Risk Seviyesi | Geri Alma |
| --- | --- | --- | --- |
| **Adobe Network Block** | Adobe’nin ağ erişimini engeller | 🔴 Yüksek | Firewall kuralları |
| **Adobe Debloat** | Adobe uygulamalarını kaldırır | 🔴 Yüksek | Manuel yeniden kurulum |

### Ağ ve İnternet:

| Tweak | Açıklama | Potansiyel Sorun | Çözüm |
| --- | --- | --- | --- |
| **Disable IPv6** | IPv6 protokolünü kapatır | Modern ağ sorunları | Ağ adaptörü ayarları |
| **Prefer IPv4 over IPv6** | IPv4’ü öncelikli yap | Uyumluluk sorunları | Registry düzenleme |

### Sistem Servisleri:

| Tweak | Açıklama | Etki | Uyarı |
| --- | --- | --- | --- |
| **Disable Teredo** | Teredo tunnel’ını kapat | Ağ değişiklikleri | 🟡 Orta risk |
| **Disable Background Apps** | Arka plan uygulamalarını kapat | Sistem performansı | 🟡 Uygulama sorunları |
| **Disable Fullscreen Optimizations** | Tam ekran optimizasyonlarını kapat | Oyun performansı | 🟡 Görsel sorunlar |

### Microsoft Servisleri:

| Tweak | Açıklama | Sonuç | Risk |
| --- | --- | --- | --- |
| **Disable Microsoft Copilot** | AI asistanını devre dışı bırak | Özellik kaybı | 🟡 Orta |
| **Disable Intel MM (vPro LMS)** | Intel Management Engine kapat | Donanım özellikleri | 🔴 Yüksek |
| **Disable Notification Tray/Calendar** | Bildirim merkezini kapat | Sistem bildirimleri | 🟡 Orta |

### Windows Özellikleri:

| Tweak | Açıklama | Etki | Geri Alma |
| --- | --- | --- | --- |
| **Disable Windows Platform Binary Table (WPBT)** | WPBT’yi devre dışı bırak | Sistem başlatma | BIOS ayarları |
| **Set Display for Performance** | Ekranı performans için optimize et | Görsel kalite | Görünüm ayarları |
| **Set Classic Right-Click Menu** | Klasik sağ tık menüsü | Kullanıcı deneyimi | Registry |
| **Set Time to UTC (Dual Boot)** | Dual boot için UTC zamanı | Çift sistem | Saat ayarları |

### Uygulama Kaldırma (ÇOK RİSKLİ):

| Tweak | Açıklama | Risk | Sonuç |
| --- | --- | --- | --- |
| **Remove ALL MS Store Apps - NOT RECOMMENDED** | Tüm Store uygulamalarını kaldır | 🔴 ÇOK YÜKSEK | Sistem kararsızlığı |
| **Remove Microsoft Edge** | Edge tarayıcısını kaldır | 🔴 Yüksek | Web görüntüleme sorunları |
| **Remove Home and Gallery from explorer** | Gezgin’den öğeleri kaldır | 🟡 Orta | Eksik özellikler |
| **Remove OneDrive** | OneDrive’ı tamamen kaldır | 🟡 Orta | Bulut eşitleme kaybı |
| **Block Razer Software Installs** | Razer yazılım kurulumunu engelle | 🟡 Orta | Donanım desteği |

### 🎨 Customize Preferences (Özelleştirme Tercihleri)

### Görünüm ve Tema:

| Özellik | Açıklama | Görsel Etki |
| --- | --- | --- |
| **Dark Theme for Windows** | ✅ Sistem geneli koyu tema | Modern görünüm |
| **Bing Search in Start Menu** | ✅ Başlangıç menüsünde Bing arama | İnternet arama |
| **NumLock on Startup** | ⚪ Başlangıçta NumLock açık | Sayısal tuş takımı |
| **Verbose Messages During Logon** | ⚪ Oturum açmada detaylı mesajlar | Sistem bilgisi |

### Başlangıç Menüsü:

| Özellik | Açıklama | Kullanıcı Deneyimi |
| --- | --- | --- |
| **Recommendations in Start Menu** | ✅ Başlangıç menüsünde öneriler | Kişiselleştirme |
| **Remove Settings Home Page** | ⚪ Ayarlar ana sayfasını kaldır | Sadelik |

### Pencere Yönetimi:

| Özellik | Açıklama | Kullanım |
| --- | --- | --- |
| **Snap Window** | ✅ Pencere yapıştırma | Çoklu pencere |
| **Snap Assist Flyout** | ✅ Yapıştırma yardımcısı | Verimlilik |
| **Snap Assist Suggestion** | ✅ Yapıştırma önerileri | Otomatik düzenleme |

### Fare ve Klavye:

| Özellik | Açıklama | Erişilebilirlik |
| --- | --- | --- |
| **Mouse Acceleration** | ✅ Fare ivmesi | Hareket düzgünlüğü |
| **Sticky Keys** | ✅ Yapışkan tuşlar | Erişim kolaylığı |

### Dosya ve Sistem:

| Özellik | Açıklama | Kullanıcı Kontrolü |
| --- | --- | --- |
| **Show Hidden Files** | ⚪ Gizli dosyaları göster | Gelişmiş kullanım |
| **Show File Extensions** | ✅ Dosya uzantılarını göster | Güvenlik |

### Görev Çubuğu:

| Özellik | Açıklama | Görünüm |
| --- | --- | --- |
| **Search Button in Taskbar** | ⚪ Görev çubuğunda arama | Ekran alanı |
| **Task View Button in Taskbar** | ✅ Görev görünümü düğmesi | Sanal masaüstler |
| **Center Taskbar Items** | ✅ Görev çubuğu ortalama | Modern tasarım |
| **Widgets Button in Taskbar** | ✅ Widget düğmesi | Hızlı bilgi |

### Ayrıntılı Ayarlar:

| Özellik | Açıklama | Teknik Detay |
| --- | --- | --- |
| **Detailed BSoD** | ⚪ Detaylı mavi ekran | Hata ayıklama |

### 🎮 Tweaks Uygulama ve Kontrol

### Eylem Düğmeleri:

| Düğme | Açıklama | Kullanım |
| --- | --- | --- |
| **Run Tweaks** | Seçili tweakları uygular | Ana uygulama düğmesi |
| **Undo Selected Tweaks** | Seçili tweakları geri alır | Hata durumunda geri alma |

### Güvenli Kullanım Önerileri:

1. **Öncesinde:** Her zaman geri yükleme noktası oluşturun
2. **Seçim:** Sadece ihtiyaç duyduğunuz tweakları seçin
3. **Test:** Tweakları küçük gruplar halinde uygulayın
4. **Gözlem:** Her grup sonrası sistemi test edin
5. **Geri alma:** Sorun yaşarsanız “Undo Selected Tweaks” kullanın

### Risk Kategorileri:

| Seviye | İşaret | Açıklama | Önerilen Eylem |
| --- | --- | --- | --- |
| 🟢 **Güvenli** | Essential Tweaks çoğunluğu | Sistem kararlılığını etkilemez | Güvenle uygulayın |
| 🟡 **Orta Risk** | Bazı sistem değişiklikleri | Küçük sorunlara neden olabilir | Dikkatli uygulayın |
| 🔴 **Yüksek Risk** | Advanced Tweaks | Sistem kararsızlığına yol açabilir | Sadece deneyimli kullanıcılar |
| ⚫ **Kritik** | Store Apps kaldırma | Sistem işlevselliğini bozabilir | Önerilmez |

## 🔧 Config Sekmesi - Gelişmiş Yapılandırma

Config sekmesi, Windows’un gelişmiş yapılandırma seçeneklerini, sistem onarım araçlarını ve klasik kontrol panellerine erişimi sağlar.

### 🎯 Features (Windows Özellikleri)

### Temel .NET Framework Desteği:

| Özellik | Açıklama | Kullanım Amacı | Gereksinim |
| --- | --- | --- | --- |
| **All .Net Framework (2, 3.4)** | Eski .NET Framework sürümlerini etkinleştirir | Legacy uygulamalar için | Windows özelliği |

### Sanallaştırma Teknolojileri:

| Özellik | Açıklama | Hedef Kitle | Sistem Etkisi |
| --- | --- | --- | --- |
| **Hyper-V Virtualization** | Microsoft’un yerleşik sanallaştırma çözümü | Geliştiriciler, IT uzmanları | Yüksek CPU/RAM kullanımı |
| **Windows Subsystem for Linux** | Linux alt sistemini Windows’ta çalıştır | Geliştirici ortamları | Orta sistem etkisi |
| **Windows Sandbox** | İzole Windows ortamı | Güvenli test için | Hyper-V gerektirir |

### Medya ve Oyun Desteği:

| Özellik | Açıklama | Hedef | Uyumluluk |
| --- | --- | --- | --- |
| **Legacy Media (WMP, DirectPlay)** | Eski medya ve oyun desteği | Retro oyunlar, eski uygulamalar | Windows 95/XP uygulamaları |

### Ağ Dosya Sistemleri:

| Özellik | Açıklama | Kullanım Alanı | Teknik Detay |
| --- | --- | --- | --- |
| **NFS - Network File System** | UNIX/Linux dosya paylaşım protokolü | Cross-platform ağ | Enterprise ortamlar |

### Arama ve Kayıt Defteri:

| Özellik | Açıklama | Etki | Yeniden Başlatma |
| --- | --- | --- | --- |
| **Enable Search Box Web Suggestions in Registry** | Web önerilerini etkinleştir | Arama deneyimi | Explorer restart gerekli |
| **Disable Search Box Web Suggestions in Registry** | Web önerilerini devre dışı bırak | Gizlilik | Explorer restart gerekli |

### Sistem Bakım ve Kurtarma:

| Özellik | Açıklama | Zamanlama | Fayda |
| --- | --- | --- | --- |
| **Enable Daily Registry Backup Task 12:30am** | Günlük otomatik registry yedekleme | Gece 00:30 | Sistem güvenliği |
| **Enable Legacy F8 Boot Recovery** | Klasik F8 boot menüsünü etkinleştir | Boot sırasında | Gelişmiş başlatma seçenekleri |
| **Disable Legacy F8 Boot Recovery** | Klasik F8 boot menüsünü kapat | Hızlı boot için | Modern startup |

### Özellik Yükleme Düğmesi:

| Düğme | Açıklama | Kullanım |
| --- | --- | --- |
| **Install Features** | Seçili özellikleri sisteme yükler | Tüm seçimler sonrası |

### 🛠️ Fixes (Sistem Onarım Araçları)

### Kullanıcı Hesap Yönetimi:

| Araç | Açıklama | Kullanım Senaryosu | Komut |
| --- | --- | --- | --- |
| **Set Up Autologin** | Otomatik oturum açma ayarla | Kişisel bilgisayarlar | `netplwiz` |

### Sistem Bileşeni Onarımları:

| Araç | Açıklama | Sorun Türü | İşlem Süresi |
| --- | --- | --- | --- |
| **Reset Windows Update** | Windows Update servisini sıfırla | Güncelleme takılmaları | 2-5 dakika |
| **Reset Network** | Ağ yapılandırmasını sıfırla | İnternet bağlantı sorunları | 1-3 dakika |
| **System Corruption Scan** | Sistem dosyası bütünlüğü kontrolü | Dosya bozulmaları | 10-30 dakika |

### Uygulama Yöneticisi Onarımları:

| Araç | Açıklama | Çözüm | Yeniden Kurulum |
| --- | --- | --- | --- |
| **WinGet Reinstall** | Windows Package Manager’ı yeniden yükle | WinGet sorunları | Otomatik |

### Üçüncü Parti Temizlik:

| Araç | Açıklama | Hedef | Etki |
| --- | --- | --- | --- |
| **Remove Adobe Creative Cloud** | Adobe Creative Cloud’u tamamen kaldır | Sistem temizliği | Kalıntı temizleme |

### 🖥️ Legacy Windows Panels (Klasik Kontrol Panelleri)

### Ana Sistem Panelleri:

| Panel | Açıklama | Erişim Komutu | Kullanım Amacı |
| --- | --- | --- | --- |
| **Control Panel** | Klasik Windows kontrol paneli | `control` | Sistem ayarları |
| **God Mode** | Tüm sistem ayarlarına tek erişim | Özel GUID | Gelişmiş yönetim |
| **System Properties** | Sistem bilgileri ve ayarları | `sysdm.cpl` | Donanım/performans |

### Ağ ve Bağlantı Panelleri:

| Panel | Açıklama | Erişim | Yönetim |
| --- | --- | --- | --- |
| **Network Connections** | Ağ adaptörleri ve bağlantılar | `ncpa.cpl` | Ağ yapılandırması |

### Güç ve Donanım Panelleri:

| Panel | Açıklama | Kontrol | Hedef |
| --- | --- | --- | --- |
| **Power Panel** | Güç yönetimi ve pil ayarları | `powercfg.cpl` | Enerji optimizasyonu |
| **Printer Panel** | Yazıcı kurulumu ve yönetimi | Yazıcı ayarları | Donanım yönetimi |

### Bölgesel ve Ses Panelleri:

| Panel | Açıklama | Yapılandırma | Kişiselleştirme |
| --- | --- | --- | --- |
| **Region** | Bölge, dil ve tarih/saat formatları | Yerelleştirme | Uluslararası kullanım |
| **Sound Settings** | Ses aygıtları ve ses efektleri | `mmsys.cpl` | Ses yapılandırması |

### Kullanıcı Yönetimi:

| Panel | Açıklama | Yönetim | Güvenlik |
| --- | --- | --- | --- |
| **User Accounts** | Kullanıcı hesapları ve parola ayarları | `netplwiz` | Erişim kontrolü |

### 💻 PowerShell Profile (CTT Özel Profili)

### PowerShell Profil Yönetimi:

| Eylem | Açıklama | İçerik | Fayda |
| --- | --- | --- | --- |
| **Install CTT PowerShell Profile** | Chris Titus Tech’in özel PowerShell profilini yükle | Özel komutlar, temalar | Gelişmiş terminal deneyimi |
| **Uninstall CTT PowerShell Profile** | CTT PowerShell profilini kaldır | Varsayılan ayarlara dön | Sistem temizliği |

### CTT Profil Özellikleri:

**Dahil Edilen Özellikler:**
- ✅ **Gelişmiş Komut Tamamlama:** Tab ile otomatik tamamlama
- ✅ **Sözdizimi Vurgulama:** Renkli komut görünümü
- ✅ **Git Entegrasyonu:** Git durumu gösterimi
- ✅ **Özel Alias’lar:** Kısaltılmış komutlar
- ✅ **Modern Tema:** Görsel iyileştirmeler
- ✅ **Performans Optimizasyonu:** Hızlı başlatma

**Eklenen Alias Örnekleri:**
- `ll` → `Get-ChildItem` (Dosya listesi)
- `la` → `Get-ChildItem -Force` (Gizli dosyalarla)
- `..` → `Set-Location ..` (Üst dizin)
- `cls` → `Clear-Host` (Ekran temizle)

### 🌐 Remote Access (Uzaktan Erişim)

### OpenSSH Server Kurulumu:

| Özellik | Açıklama | Güvenlik Seviyesi | Yapılandırma |
| --- | --- | --- | --- |
| **Enable OpenSSH Server** | Windows’ta SSH sunucusunu etkinleştir | Yüksek güvenlik | Otomatik yapılandırma |

### SSH Sunucu Özellikleri:

**Temel Özellikler:**
- 🔐 **Güvenli Bağlantı:** SSH protokolü ile şifreli erişim
- 🖥️ **Komut Satırı Erişimi:** Uzaktan PowerShell/CMD kullanımı
- 📁 **Dosya Transferi:** SCP/SFTP desteği
- 🔑 **Anahtar Tabanlı Kimlik Doğrulama:** Gelişmiş güvenlik

**Güvenlik Yapılandırması:**
- Port 22 (varsayılan) veya özel port
- Güvenlik duvarı kuralı otomatik ekleme
- Başarısız girişim sınırlandırması
- IP kısıtlama seçenekleri

**Kullanım Senaryoları:**
- 💼 **Uzaktan Yönetim:** Server ve workstation yönetimi
- 🔧 **Geliştirme:** Remote development environment
- 📊 **Monitoring:** Sistem izleme ve log analizi
- 🛠️ **Bakım:** Uzaktan sistem bakımı

### SSH İstemci Araçları:

**Windows Uyumlu SSH İstemcileri:**
- **Windows Terminal:** Modern terminal ile SSH
- **PuTTY:** Klasik SSH istemcisi
- **WSL/Linux:** Linux alt sistemi üzerinden
- **PowerShell:** Yerleşik SSH istemcisi

### 🔧 Config Sekmesi Kullanım Rehberi

### Özellik Kurulum Sırası:

1. **Öncelik:** Gerekli Windows özelliklerini seçin
2. **Kurulum:** “Install Features” butonuna tıklayın
3. **Bekleme:** Sistem yeniden başlatma gerekebilir
4. **Test:** Kurulu özellikleri test edin

### Sistem Onarım Adımları:

1. **Tanı:** Sorunu belirleyin
2. **Yedek:** Geri yükleme noktası oluşturun
3. **Onarım:** İlgili Fix aracını çalıştırın
4. **Doğrulama:** Sorunun çözüldüğünü kontrol edin

### Güvenlik Önerileri:

- ⚠️ **OpenSSH:** Sadece güvenli ağlarda etkinleştirin
- 🔐 **God Mode:** Deneyimli kullanıcılar için
- 🛡️ **Registry Backup:** Mutlaka aktif tutun
- 🔄 **System Corruption Scan:** Düzenli çalıştırın

## 🛠️ Yaygın Sorunlar ve Çözümleri

### Sorun 1: PowerShell Execution Policy Hatası

```powershell
# Çözüm
Set-ExecutionPolicy -ExecutionPolicy RemoteSigned -Scope CurrentUser

# Geçici çözüm 
PowerShell -ExecutionPolicy Bypass -File .\winutil.ps1
```

### Sorun 2: Internet Connection Required Hatası

```powershell
# Manuel download
Invoke-WebRequest -Uri "https://github.com/ChrisTitusTech/winutil/releases/latest/download/winutil.ps1" -OutFile "winutil.ps1"
```

### Sorun 3: Tweakları Geri Alma

| Tweak | Geri Alma Yöntemi |
| --- | --- |
| **Disable Telemetry** | `Settings > Privacy > Diagnostics & feedback` |
| **Remove MS Store Apps** | `PowerShell: Get-AppxPackage -AllUsers` |
| **Disable Windows Defender** | `Windows Security > Virus & threat protection` |

## 🔄 Sistem Geri Yükleme

### Geri Yükleme Noktasından Döndürme:

```powershell
# Geri yükleme noktaları listele
Get-ComputerRestorePoint

# Geri yükleme başlat
Restore-Computer -RestorePoint 1
```

### Manuel Geri Yükleme:

1. **Sistem Özellikleri** > **Sistem Koruması**
2. **Sistem Geri Yükleme** > **Sonraki**
3. Geri yükleme noktası seçin
4. **Son** > **Evet**

## 🛡️ Güvenlik ve Geri Alma

### 🔒 Güvenlik En İyi Uygulamaları

### Kurulum Öncesi:

```powershell
# Sistem bilgilerini kaydet
Get-ComputerInfo | Out-File "system_info_backup.txt"

# Geri yükleme noktası oluştur
Checkpoint-Computer -Description "WinUtil Before Changes"

# Uygulama listesini kaydet
Get-AppxPackage | Select Name, Version | Export-Csv "installed_apps_backup.csv"
```

### Kurulum Sonrası:

```powershell
# Sistem kararlılığını test et
sfc /scannow

# Event log kontrol et
Get-EventLog -LogName System -EntryType Error -Newest 10

# Performans etkisini ölç
Get-Counter "\Processor(_Total)\% Processor Time"
```

### 🔄 Geri Alma Prosedürleri

### Hızlı Geri Alma Komutları:

```powershell
# Windows Store apps geri yükle
Get-AppxPackage -AllUsers | Foreach {Add-AppxPackage -DisableDevelopmentMode -Register "$($_.InstallLocation)\AppXManifest.xml"}

# Telemetry yeniden etkinleştir
reg add "HKLM\SOFTWARE\Microsoft\Windows\CurrentVersion\Policies\DataCollection" /v AllowTelemetry /t REG_DWORD /d 3 /f

# Windows Defender yeniden etkinleştir
Set-MpPreference -DisableRealtimeMonitoring $false
```

### ⚠️ Risk Değerlendirmesi

| Risk Seviyesi | Tweaklar | Geri Alma Kolaylığı |
| --- | --- | --- |
| 🟢 **Düşük** | Tema, dosya görünümü, temporary files | Kolay |
| 🟡 **Orta** | Telemetry, startup programs | Orta |
| 🔴 **Yüksek** | Store apps removal, system services | Zor |

---

### GitHub Repository:

- 📂 **Source Code**: https://github.com/ChrisTitusTech/winutil