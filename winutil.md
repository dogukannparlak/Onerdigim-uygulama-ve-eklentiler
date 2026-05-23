# 🛠️ WinUtil

> **Kısa Açıklama:** Windows'ta toplu uygulama kurulumu, sistem tweak'leri, onarım araçları ve güncelleme politikalarını tek arayüzden yöneten ücretsiz PowerShell aracı.

2026.x · Windows 10/11 · MIT / ücretsiz · Sistem yönetimi

---

## 📌 Genel Bakış

WinUtil (Chris Titus Tech Windows Utility), popüler programları toplu kurmanı, Windows gizlilik ve performans ayarlarını tek tıkla uygulamanı, sistem onarım araçlarına erişmeni ve Windows Update politikasını yapılandırmanı sağlar. Grafik arayüz sunar; arka planda PowerShell, WinGet veya Chocolatey kullanır.

Bu rehberde 4 ana sekme anlatılır: **Install**, **Tweaks**, **Config**, **Updates**.

> ⚠️ WinUtil sistem genelinde değişiklik yapar. **Yönetici olarak** çalıştırman gerekir. Tweaks uygulamadan önce geri yükleme noktası oluşturman önerilir.

> En güncel bilgi için [resmi GitHub deposunu](https://github.com/ChrisTitusTech/winutil) ve [winutil.christitus.com](https://winutil.christitus.com) dokümantasyonunu kontrol et. Arayüz ve madde listesi sürüme göre değişebilir.

---

## ✨ Öne Çıkan Özellikler

- **Install** — Kategorilere ayrılmış yüzlerce uygulamayı toplu kur, kaldır veya güncelle
- **Tweaks** — Gizlilik, performans ve arayüz ayarlarını hazır profillerle veya tek tek uygula
- **Config** — Windows özelliklerini aç/kapat, sistem onarımı çalıştır, klasik panellere kısayol
- **Updates** — Windows Update politikasını varsayılan, dengeli veya kapalı moda al

---

## 📥 İndirme ve Kurulum

### Yöntem 1: PowerShell — Önerilen

1. Başlat menüsünde **Terminal** veya **PowerShell** ara
2. Sağ tık → **Yönetici olarak çalıştır**
3. Aşağıdaki komutu yapıştır:

```powershell
irm "https://christitus.com/win" | iex
```

Script indirilir ve WinUtil arayüzü açılır. Her çalıştırmada güncel sürüm çekilir; internet bağlantısı gerekir.

### Yöntem 2: WinGet

```powershell
winget install ChrisTitusTech.WinUtil
```

Kurulumdan sonra WinUtil'i yönetici PowerShell'den başlat.

### Yöntem 3: GitHub Releases

1. [github.com/ChrisTitusTech/winutil/releases](https://github.com/ChrisTitusTech/winutil/releases) adresine git
2. `winutil.ps1` dosyasını indir
3. Yönetici PowerShell'de çalıştır:

```powershell
.\winutil.ps1
```

---

## ⚙️ İlk Kullanım

1. **Yönetici izni:** WinUtil sistem dosyalarına dokunur; normal kullanıcı hesabıyla tam çalışmaz
2. **Geri yükleme noktası:** Tweaks sekmesinde **Restore Point - Create** ile veya Windows Ayarları → Sistem → Kurtarma üzerinden oluştur
3. **Sekme seç:** İhtiyacına göre Install, Tweaks, Config veya Updates sekmesine geç

> 💡 Emin değilsen önce **Install** ile uygulama kur, ardından Tweaks'te **Standard** hazır seçimini incele; hepsini birden uygulama.

---

## 🖥️ Ortak Arayüz

Üst çubukta tüm sekmelerde şunlar bulunur:


| Öğe                                     | Ne işe yarar                                   |
| --------------------------------------- | ---------------------------------------------- |
| **Install / Tweaks / Config / Updates** | Ana sekmeler arası geçiş                       |
| **Arama kutusu**                        | Uygulama veya tweak adı ara                    |
| **Tema (ay/güneş)**                     | Arayüz koyu/açık mod                           |
| **Bildirim / Ayarlar / Kapat**          | Bildirimler, WinUtil ayarları, pencereyi kapat |


---

# 📦 Install

Popüler yazılımları kategoriler halinde listeler; işaretlediklerini toplu kurar, kaldırır veya günceller.

## Sol panel — Actions


| Düğme / öğe                        | Ne işe yarar                                                                            |
| ---------------------------------- | --------------------------------------------------------------------------------------- |
| **Install/Upgrade Applications**   | Seçili uygulamaları kurar veya günceller                                                |
| **Uninstall Applications**         | Seçili uygulamaları kaldırır                                                            |
| **Upgrade all Applications**       | Desteklenen tüm kurulu uygulamaları günceller                                           |
| **Package Manager**                | **WinGet** (varsayılan, Microsoft resmi) veya **Chocolatey** (daha geniş paket listesi) |
| **Highlight FOSS**                 | Açık kaynak uygulamaları yeşil renkle vurgular                                          |
| **Clear Selection**                | Tüm işaretleri temizler                                                                 |
| **Collapse/Expand All Categories** | Kategorileri toplu açar veya kapatır                                                    |
| **Selected Apps**                  | Kaç uygulama seçili olduğunu gösterir                                                   |
| **Show Installed Apps**            | Sistemde kurulu olanları otomatik işaretler                                             |


## Kategoriler

Uygulamalar şu kategorilere ayrılır; her kategoride onlarca program bulunur:


| Kategori             | Örnek türler                                |
| -------------------- | ------------------------------------------- |
| **Browsers**         | Chrome, Firefox, Brave, Edge...             |
| **Communications**   | Discord, Slack, Telegram, Zoom...           |
| **Development**      | VS Code, Git, Python, Node.js...            |
| **Games**            | Steam, Epic Games, GOG Galaxy...            |
| **Microsoft Tools**  | PowerShell, PowerToys, Windows Terminal...  |
| **Multimedia Tools** | VLC, OBS, GIMP, Audacity...                 |
| **Pro Tools**        | Wireshark, PuTTY, WinSCP, Nmap...           |
| **Selfhosted Tools** | Plex, Nextcloud Desktop...                  |
| **Utilities**        | 7-Zip, Bitwarden, Rufus, CrystalDiskMark... |


Tam liste arayüzde görünür; sürüme göre uygulama eklenip çıkarılabilir.

## Nasıl kullanılır?

1. **Install** sekmesine git
2. Kategorilerden ihtiyacın olan uygulamaları işaretle
3. **Package Manager** olarak WinGet veya Chocolatey seç
4. **Install/Upgrade Applications** düğmesine tıkla
5. Kurulum ilerlemesini pencerede takip et

> 💡 **WinGet** Microsoft'un resmi paket yöneticisidir; çoğu kullanıcı için yeterlidir. **Chocolatey** daha fazla paket sunar ancak üçüncü taraf bir ekosistemdir. Kurulum hatası alırsan diğer paket yöneticisini dene.

---

# ⚙️ Tweaks

Windows gizlilik, performans ve arayüz ayarlarını toplu veya tek tek uygular. Değişiklikler kayıt defteri, servisler veya uygulama kaldırma yoluyla yapılır.

## Kullanım akışı

1. **Recommended Selections** ile başla:
  - **Standard** — Yaygın gizlilik ve temizlik tweak'leri
  - **Minimal** — Daha az müdahale
  - **Clear** — Tüm seçimleri temizle
  - **Get Installed Tweaks** — Daha önce uygulanmış tweak'leri işaretle
2. Listeden ekstra maddeleri işaretle veya **Customize Preferences** toggle'larını ayarla
3. **Run Tweaks** ile uygula
4. Sorun olursa aynı maddeleri seçip **Undo Selected Tweaks** ile geri al

> ⚠️ Bu sekmedeki ayarlar sistemi ciddi şekilde değiştirir. Emin değilsen **Standard** veya **Minimal** ile başla. Her maddenin üzerine gelince İngilizce açıklama tooltip'i görünür.

## Ek araçlar


| Öğe                      | Ne işe yarar                                                                                               |
| ------------------------ | ---------------------------------------------------------------------------------------------------------- |
| **O&O ShutUp10++ - Run** | Üçüncü taraf gizlilik aracı O&O ShutUp10++'ı indirip çalıştırır                                            |
| **DNS - Set to:**        | Sistem DNS'ini seçilen sağlayıcıya ayarlar (Default DHCP, Google, Cloudflare, Quad9, OpenDNS, AdGuard vb.) |


## Performance Plans


| Düğme                                      | Ne işe yarar                                           |
| ------------------------------------------ | ------------------------------------------------------ |
| **Ultimate Performance Profile - Enable**  | Gizli "Ultimate Performance" güç planını etkinleştirir |
| **Ultimate Performance Profile - Disable** | Ultimate Performance planını kaldırır                  |


---

## Essential Tweaks

Genellikle güvenli kabul edilen temel düzenlemeler. Yine de geri yükleme noktası oluşturman önerilir.


| Madde                                                    | Ne işe yarar                                                                    | Not                                                              |
| -------------------------------------------------------- | ------------------------------------------------------------------------------- | ---------------------------------------------------------------- |
| **Restore Point - Create**                               | WinUtil değişikliklerinden önce sistem geri yükleme noktası oluşturur           | Tweaks uygulamadan önce bunu seç                                 |
| **Temporary Files - Remove**                             | Kullanıcı ve sistem TEMP klasörlerini temizler                                  |                                                                  |
| **Disk Cleanup - Run**                                   | C: sürücüsünde Disk Temizleme çalıştırır; eski Windows güncellemelerini siler   |                                                                  |
| **Telemetry - Disable**                                  | Microsoft telemetri ve tanılama veri gönderimini kapatır                        |                                                                  |
| **Activity History - Disable**                           | Son belgeler, pano ve çalıştır geçmişi takibini kapatır                         |                                                                  |
| **ConsumerFeatures - Disable**                           | Windows'un otomatik oyun ve Store uygulaması yüklemesini engeller               | Phone Link gibi bazı varsayılan uygulamalara erişim kapanabilir  |
| **Location Tracking - Disable**                          | Konum takibini ve ilgili servisi devre dışı bırakır                             |                                                                  |
| **Unwanted Pre-Installed Apps - Remove**                 | Bing News, Clipchamp, Solitaire, Teams gibi önceden yüklü uygulamaları kaldırır |                                                                  |
| **Widgets - Remove**                                     | Görev çubuğundaki Widget'ları ve ilgili paketleri kaldırır                      |                                                                  |
| **End Task With Right Click - Enable**                   | Görev çubuğunda sağ tık → Görevi sonlandır seçeneğini açar                      |                                                                  |
| **Services - Set to Manual**                             | Bazı servisleri manuel başlatmaya alır; svchost süreç sayısını azaltabilir      |                                                                  |
| **PowerShell 7 Telemetry - Disable**                     | PowerShell 7 telemetri ortam değişkenini kapatır                                |                                                                  |
| **Windows Platform Binary Table (WPBT) - Disable**       | Üretici yazılımının önyüklemede çalışmasını engeller                            | Güvenlik odaklı                                                  |
| **BitLocker - Disable**                                  | BitLocker disk şifrelemesini kapatır                                            | Şifreleme kullanıyorsan seçme                                    |
| **Hibernation - Disable**                                | Hazırda bekletmeyi kapatır; hiberfil.sys dosyasını kaldırır                     | Disk alanı kazandırır                                            |
| **Microsoft Store Recommended Search Results - Disable** | Başlat aramasında Store uygulama önerilerini gizler                             |                                                                  |
| **Start Menu Previous Layout - Enable**                  | Windows 11 25H2 sonrası yeni Başlat menüsü yerine eski düzeni geri getirir      | ViVeTool indirir; yeniden başlatma gerekir                       |
| **File Explorer Automatic Folder Discovery - Disable**   | Explorer'ın klasör tipini otomatik tahmin etmesini kapatır                      | Klasör gruplamasını devre dışı bırakır; oturumu kapat/aç gerekir |


---

## Advanced Tweaks — CAUTION

Sistem davranışını belirgin şekilde değiştirir. Ne yaptığını bilmeden uygulama.


| Madde                                              | Ne işe yarar                                                              | Not                                                    |
| -------------------------------------------------- | ------------------------------------------------------------------------- | ------------------------------------------------------ |
| **Microsoft Edge - Debloat**                       | Edge telemetri, popup ve gereksiz özelliklerini kapatır                   | Edge kalır, sadeleşir                                  |
| **Microsoft Edge - Remove**                        | Edge kaldırma kısıtlamasını kaldırıp Edge'i siler                         | Bazı Windows özellikleri Edge'e bağımlı olabilir       |
| **Microsoft OneDrive - Remove**                    | OneDrive'ı kaldırır ve senkron servisini kapatır                          | Bulut yedekleme kaybolur                               |
| **Xbox & Gaming Components - Remove**              | Xbox uygulaması, Game Bar ve ilgili bileşenleri kaldırır                  | Oyun kaydı ve Xbox özellikleri gider                   |
| **Windows AI - Disable**                           | Copilot, Recall ve diğer Windows AI paketlerini kaldırır veya kapatır     | AI özellikleri tamamen gider                           |
| **File Explorer Home and Gallery - Disable**       | Explorer'dan Giriş ve Galeri'yi kaldırır; varsayılan "Bu bilgisayar" olur |                                                        |
| **Visual Effects - Set to Best Performance**       | Görsel efektleri minimuma indirir; performans öncelikli                   | Arayüz sadeleşir                                       |
| **Storage Sense - Disable**                        | Otomatik disk temizliğini (Storage Sense) kapatır                         | Manuel temizlik gerekir                                |
| **Background Apps - Disable**                      | Store uygulamalarının arka planda çalışmasını engeller                    | Bildirim/bildirim gecikmesi olabilir                   |
| **Fullscreen Optimizations - Disable**             | Tam ekran optimizasyonlarını kapatır                                      | Exclusive fullscreen'de renk yönetimi devre dışı kalır |
| **System Tray Notifications & Calendar - Disable** | Bildirim merkezi ve takvim dahil tüm bildirimleri kapatır                 |                                                        |
| **Right-Click Menu Previous Layout - Enable**      | Windows 11 sade sağ tık menüsü yerine klasik menüyü getirir               | Explorer yeniden başlar                                |
| **Brave Browser - Debloat**                        | Brave Rewards, Leo AI, cüzdan ve VPN gibi özellikleri kapatır             | Brave kuruluysa geçerli                                |
| **Adobe URL Block List - Enable**                  | hosts dosyasına Adobe aktivasyon/telemetri sunucularını ekler             | hosts dosyası yedeklenir                               |
| **Razer Software Auto-Install - Disable**          | Razer yazılımının otomatik kurulumunu engeller                            | Donanım sürücüsü olmadan da çalışır                    |
| **RDP Unsigned File Warnings - Disable**           | İmzasız RDP dosyası uyarılarını kapatır                                   | Güvenlik riski artabilir                               |
| **IPv6 - Disable**                                 | IPv6 protokolünü tamamen kapatır                                          | Modern ağlarda sorun çıkarabilir                       |
| **IPv6 - Set IPv4 as Preferred**                   | IPv4'ü IPv6'ya göre önceliklendirir                                       | IPv6'yi tamamen kapatmaz                               |
| **Teredo - Disable**                               | Teredo tünelleme protokolünü kapatır                                      | Bazı oyunlarda bağlantı sorunu olabilir                |
| **Date & Time - Set Time to UTC**                  | Sistem saatini UTC'ye ayarlar                                             | Çift önyükleme (Windows + Linux) için                  |
| **O&O ShutUp10++ - Run**                           | Harici gizlilik aracını başlatır                                          | Ayrı pencere açılır                                    |
| **DNS - Set to:**                                  | Seçilen DNS sağlayıcısını tüm ağ adaptörlerine uygular                    | Default DHCP ile geri alınabilir                       |


---

## Customize Preferences

Toggle anahtarları: **açık** = madde adındaki özellik etkin, **kapalı** = devre dışı. Run Tweaks ile birlikte uygulanır.


| Toggle                             | Açıkken ne olur                                          | Not                                                |
| ---------------------------------- | -------------------------------------------------------- | -------------------------------------------------- |
| **Dark Theme for Windows**         | Sistem geneli koyu tema                                  |                                                    |
| **File Explorer File Extensions**  | Dosya uzantıları görünür (.txt, .exe)                    |                                                    |
| **File Explorer Hidden Files**     | Gizli dosya ve klasörler listelenir                      |                                                    |
| **Start Menu Bing Search**         | Başlat aramasına Bing web sonuçları dahil edilir         |                                                    |
| **Start Menu Recommendations**     | Başlat menüsünde öneriler gösterilir                     | Kapalıyken Kilit ekranı Spotlight da etkilenebilir |
| **Settings Home Page**             | Ayarlar uygulamasında ana sayfa görünür                  |                                                    |
| **Taskbar Centered Icons**         | Görev çubuğu simgeleri ortada (Win11)                    | Kapalı = solda                                     |
| **Taskbar Search Icon**            | Görev çubuğunda arama simgesi                            |                                                    |
| **Taskbar Task View Icon**         | Görev çubuğunda Görev Görünümü düğmesi                   |                                                    |
| **System Tray Battery Percentage** | Pil simgesinin yanında yüzde gösterilir                  | Laptop                                             |
| **Mouse Acceleration**             | Fare imleci hızına göre ivmelenir                        | FPS oyunlarında genelde kapalı tercih edilir       |
| **Num Lock on Startup**            | Bilgisayar açıldığında Num Lock açık                     |                                                    |
| **Sticky Keys**                    | Yapışkan tuşlar erişilebilirlik özelliği açık            |                                                    |
| **Game Mode**                      | Windows oyun için kaynak önceliği verir                  | Ses/video prodüksiyonunda kapatılabilir            |
| **Cross-Device Resume**            | Telefon ve PC arası aktivite devam ettirme (Win11 24H2+) |                                                    |
| **BSoD Verbose Mode**              | Mavi ekranda ayrıntılı hata bilgisi                      |                                                    |
| **Logon Verbose Mode**             | Oturum açarken ayrıntılı durum mesajları                 |                                                    |
| **Logon Screen Acrylic Blur**      | Giriş ekranında bulanık arka plan efekti                 |                                                    |
| **Scrollbars Always Visible**      | Kaydırma çubukları her zaman görünür                     |                                                    |
| **Multiplane Overlay**             | Multiplane Overlay grafik katmanı                        | Ekran kartı sorunlarında kapatılabilir             |
| **S0 Sleep Network Connectivity**  | Modern bekleme modunda ağ bağlantısı                     |                                                    |
| **S3 Sleep**                       | Modern Standby yerine klasik S3 uyku modu                | Donanıma bağlı                                     |
| **Microsoft Outlook New Version**  | Yeni Outlook arayüzü ve geçiş seçeneği                   | Kapalı = klasik Outlook                            |
| **Enable Long Paths**              | 260 karakterden uzun dosya yollarına izin verir          |                                                    |


---

# 🔧 Config

Windows özelliklerini aç/kapat, sistem onarımı çalıştır ve klasik yönetim panellerine kısayol eriş.

## Features

İşaretle → **Run Features** ile uygula. Bazı özellikler yeniden başlatma gerektirir.


| Özellik                                                | Ne işe yarar                                        |
| ------------------------------------------------------ | --------------------------------------------------- |
| **.NET Framework (Versions 2, 3, 4) - Enable**         | Eski .NET uygulamaları için framework desteği       |
| **Hyper-V - Enable**                                   | Sanal makine desteği (Windows Pro/Enterprise)       |
| **Windows Subsystem for Linux (WSL) - Enable**         | Linux alt sistemi                                   |
| **Windows Sandbox - Enable**                           | Tek seferlik izole Windows ortamı (Hyper-V gerekir) |
| **Legacy Media Components (WMP, DirectPlay) - Enable** | Windows Media Player ve DirectPlay                  |
| **Network File System (NFS) - Enable**                 | NFS ağ dosya paylaşımı                              |
| **Registry Backup (Daily Task 12:30am) - Enable**      | Her gece 00:30'da otomatik registry yedek görevi    |
| **Legacy F8 Boot Recovery - Enable**                   | Önyüklemede F8 gelişmiş seçenekler menüsü           |
| **Legacy F8 Boot Recovery - Disable**                  | F8 menüsünü kapatır; daha hızlı önyükleme           |


## Fixes

Tek tıkla sistem onarımı. Sorun yaşamadan rastgele çalıştırma.


| Düğme                            | Ne işe yarar                                                           |
| -------------------------------- | ---------------------------------------------------------------------- |
| **AutoLogon - Run**              | Otomatik oturum açma yapılandırmasını açar                             |
| **Network - Reset**              | Ağ yapılandırmasını sıfırlar                                           |
| **NTP Server - Enable**          | Windows Time servisini etkinleştirir                                   |
| **System Corruption Scan - Run** | SFC ve DISM ile sistem dosyası bütünlüğü kontrolü (10–30 dk sürebilir) |
| **Windows Update - Reset**       | Windows Update servislerini ve önbelleğini sıfırlar                    |
| **WinGet - Reinstall**           | Windows Package Manager'ı yeniden kurar                                |


## Legacy Windows Panels

İlgili Windows aracını doğrudan açar:

Computer Management · Control Panel · Network Connections · Power Panel · Printer Panel · Region · Sound Settings · System Properties · Time and Date · Windows Restore

## PowerShell Profile (PowerShell 7+ Only)


| Düğme                                | Ne işe yarar                                                     |
| ------------------------------------ | ---------------------------------------------------------------- |
| **CTT PowerShell Profile - Install** | Chris Titus Tech'in özelleştirilmiş PowerShell 7 profilini kurar |
| **CTT PowerShell Profile - Remove**  | CTT profilini kaldırır; varsayılana döner                        |


## Remote Access


| Düğme                       | Ne işe yarar                                |
| --------------------------- | ------------------------------------------- |
| **OpenSSH Server - Enable** | Windows'ta SSH sunucusunu kurar ve başlatır |


> ⚠️ SSH sunucusunu yalnızca güvenilir ağlarda aç. Güçlü parola veya anahtar tabanlı kimlik doğrulama kullan.

---

# 🔄 Updates

Windows Update politikasını üç hazır profilden biriyle yapılandırır.

## Default Settings

Windows Update'i fabrika varsayılanına döndürür. WinUtil'in daha önce uyguladığı güncelleme politikalarını ve ilgili Group Policy ayarlarını siler.

**Kim için:** Güncelleme ayarlarını eski haline almak isteyenler.

## Security Settings

Dengeli güvenlik profili (Windows **Pro** gerekir — Group Policy kullanır):

- **Feature update** gecikmesi: 365 gün — büyük Windows sürüm güncellemeleri ertelenir
- **Güvenlik güncellemesi** gecikmesi: 4 gün — kritik yamalar kısa süre bekletilir
- **Sürücü güncellemeleri** Windows Update üzerinden engellenir — manuel sürücü tercihini korur

**Kim için:** Kararlı sistem isteyen, yine de güvenlik yamalarını almak isteyen Pro kullanıcılar.

> 💡 Windows **Home** sürümünde Group Policy olmadığı için bu profilin bir kısmı uygulanmayabilir.

## Disable All Updates — Önerilmez

Tüm Windows güncellemelerini tamamen kapatır. Güvenlik yamaları da gelmez; sistem savunmasız kalır.

**Kim için:** Yalnızca internete bağlı olmayan, izole sistemler. Günlük kullanım bilgisayarında seçme.

---

## ⚠️ Bilinen Sorunlar ve Çözümleri


| Sorun                                  | Çözüm                                                                                                               |
| -------------------------------------- | ------------------------------------------------------------------------------------------------------------------- |
| Execution Policy hatası                | `Set-ExecutionPolicy RemoteSigned -Scope CurrentUser` veya `PowerShell -ExecutionPolicy Bypass -File .\winutil.ps1` |
| Script indirilemiyor / internet hatası | [GitHub Releases](https://github.com/ChrisTitusTech/winutil/releases)'ten `winutil.ps1` indirip manuel çalıştır     |
| Tweak sonrası sistem bozuldu           | Tweaks'te **Undo Selected Tweaks** veya Windows **Sistem Geri Yükleme**                                             |
| WinGet kurulum hatası                  | Config → **WinGet - Reinstall**                                                                                     |


---

## 🔗 Faydalı Bağlantılar

- 📂 [GitHub — ChrisTitusTech/winutil](https://github.com/ChrisTitusTech/winutil)
- 📖 [Resmi Dokümantasyon](https://winutil.christitus.com)
- 🚀 [Hızlı başlatma komutu](https://christitus.com/win)

## 📝 Notlar

> WinUtil'de bu rehberde anlatılan 4 sekme vardır: Install, Tweaks, Config, Updates. Tweaks sekmesinde 50'den fazla madde bulunur; emin olmadığın Advanced maddelere dokunma. Her maddenin üzerine gelince kısa İngilizce açıklama görünür. Değişiklik yapmadan önce **Restore Point - Create** seçmeyi unutma.

---

## ⚠️ Sorumluluk Reddi

Bu repository yalnızca bilgilendirme amaçlıdır. Burada önerilen uygulamalar ve eklentiler:

- **Kendi sorumluluğunuzda kullanın**: Uygulamaların sisteminizde neden olabileceği herhangi bir sorun, veri kaybı veya sistem hasarından sorumlu değiliz
- **Resmi kaynaklardan indirin**: Mutlaka uygulamaları resmi web sitelerinden veya güvenilir kaynaklardan indirin
- **Güncellik garantisi yoktur**: Uygulama bilgileri zaman içinde güncelliğini yitirebilir
- **Virüs/malware kontrolü yapın**: İndirdiğiniz dosyaları güvenlik yazılımınızla tarayın
- **Sistem yedeklemesi alın**: Önemli verilerinizi yedeklemeden yeni yazılım kurmayın
- **Lisans koşullarına dikkat edin**: Her uygulamanın kendi lisans koşulları vardır
- **Kişisel veri güvenliği**: Uygulamaların gizlilik politikalarını inceleyin

**Kullanım öncesi mutlaka araştırma yapın ve bu uygulamaları kendi riskinizle kullanın.**

---

*Son güncelleme: 2026-05-23*