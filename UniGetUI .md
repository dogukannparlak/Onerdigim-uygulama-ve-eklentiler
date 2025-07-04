# UniGetUI

# Paket Yöneticileri için Grafik Arayüz

## 🎯 Genel Bakış

### Araç Hakkında

UniGetUI (eski adıyla WingetUI), Windows’ta birden çok paket yöneticisini tek bir grafik arayüzden yönetmenizi sağlayan ücretsiz ve açık kaynak kodlu bir uygulamadır. “Paket yöneticilerinin paket yöneticisi” olarak tanımlanabilecek bu araç, komut satırı bilgisi gerektirmeden yazılım kurulum, güncelleme ve kaldırma işlemlerini kolaylaştırır.

### Desteklenen Paket Yöneticileri

| Paket Yöneticisi | Tür | Paket Sayısı | Açıklama |
| --- | --- | --- | --- |
| **🪟 Winget** | Microsoft Resmi | 10,000+ | Windows Package Manager |
| **🍫 Chocolatey** | Topluluk | 8,000+ | Windows için popüler paket yöneticisi |
| **🥄 Scoop** | Hafif | 3,000+ | Komut satırı araçları odaklı |
| **📱 npm** | JavaScript | 2,000,000+ | Node.js paket yöneticisi |
| **🐍 pip** | Python | 400,000+ | Python paket yöneticisi |
| **💎 .NET Tool** | Microsoft | 5,000+ | .NET geliştirici araçları |

### Ana Özellikler

- ✅ **Birleşik Arayüz**: Tüm paket yöneticilerini tek yerden kontrol
- ✅ **Batch İşlemler**: Çoklu paket kurulum/güncelleme
- ✅ **Otomatik Güncellemeler**: Zamanlanmış güncelleme kontrolü
- ✅ **Gelişmiş Arama**: Tüm repolar arasında arama
- ✅ **Export/Import**: Paket listelerini yedekleme
- ✅ **Tema Desteği**: Açık/koyu tema seçenekleri
- ✅ **30+ Dil Desteği**: Türkçe dahil çoklu dil desteği
- ✅ **Komut Satırı**: CLI parametreleri desteği

## 🚀 Kurulum ve Başlangıç

### Kurulum Yöntemleri

### 1️⃣ Microsoft Store (Önerilen)

```
🏪 Microsoft Store:
1. Microsoft Store'u açın
2. "UniGetUI" araması yapın
3. Martí Climent tarafından geliştirilen uygulamayı seçin
4. "Al" butonuna tıklayın
```

### 2️⃣ Winget ile Kurulum

```powershell
# Winget ile kurulum
winget install MartiCliment.UniGetUI
# Kaynak güncellemesi sonrası
winget source update
winget install MartiCliment.UniGetUI
```

### 3️⃣ GitHub Releases (Manuel)

```
📥 GitHub Releases:
1. https://github.com/marticliment/UniGetUI/releases
2. En son sürümü seçin (v3.2.0+)
3. "UniGetUI.Installer.exe" dosyasını indirin
4. Yönetici olarak çalıştırın
```

### 4️⃣ Chocolatey ile Kurulum

```powershell
# Chocolatey kurulumuchoco install unigetui
# Güncellemechoco upgrade unigetui
```

### 5️⃣ Scoop ile Kurulum

```powershell
# Bucket eklemescoop bucket add extras
# UniGetUI kurulumuscoop install unigetui
```

### ⚙️ İlk Yapılandırma

### İlk Açılış Adımları

```
🚀 İlk Kurulum:
1. UniGetUI'yi başlatın
2. Yönetici izinlerini onaylayın
3. Paket yöneticilerinin algılanmasını bekleyin
4. Dil ayarını Türkçe olarak seçin
5. Güncellemeleri kontrol edin
```

### Paket Yöneticilerini Etkinleştirme

| Paket Yöneticisi | Otomatik Algılama | Manuel Kurulum |
| --- | --- | --- |
| **Winget** | ✅ Windows 11’de varsayılan | `winget --version` |
| **Chocolatey** | ⚠️ Kontrol gerekli | `choco install chocolatey` |
| **Scoop** | ⚠️ Kontrol gerekli | `iwr get.scoop.sh` |
| **npm** | ⚠️ Node.js gerekli | Node.js kurulumu |
| **pip** | ⚠️ Python gerekli | Python kurulumu |

## ⚙️ Ayarlar - Settings

### 🎨 Genel Ayarlar

### Arayüz Özelleştirme

```
🎨 Görünüm Ayarları:
├── 🌙 Tema: Koyu/Açık/Sistem
├── 🌍 Dil: Türkçe (30+ dil mevcut)
├── 🔤 Yazı Tipi: Segoe UI (varsayılan)
├── 📏 Yazı Boyutu: Orta (Küçük/Orta/Büyük)
├── 🎨 Aksan Rengi: Mavi (özelleştirilebilir)
└── 📱 Pencere Boyutu: Kaydet/Geri yükle
```

### Davranış Ayarları

| Ayar | Seçenekler | Açıklama |
| --- | --- | --- |
| **Başlangıç** | Windows ile başlat | Otomatik başlatma |
| **Sistem Tepsisi** | Simge durumuna küçült | Arka plan çalışması |
| **Güncellemeler** | Otomatik kontrol | Periyodik kontrol |
| **Bildirimler** | Etkin/Kapalı | Popup bildirimleri |
| **Onay İstemleri** | Her işlem için | Güvenlik onayı |

### 📦 Paket Yöneticisi Ayarları

### Winget Konfigürasyonu

```
🪟 Winget Ayarları:
├── 📍 Kurulum Konumu: Varsayılan
├── 🔇 Sessiz Kurulum: Etkin
├── 🔄 Güncelleme Kontrolü: Günlük
├── 📊 Kaynak Önceliği: msstore > winget
├── 🛡️ Güvenlik: Imzalı paketler
└── 📜 Log Seviyesi: Bilgi
```

### Chocolatey Konfigürasyonu

```
🍫 Chocolatey Ayarları:
├── 📍 Cache Konumu: C:\ProgramData\chocolatey
├── 🔐 Global Onaylar: Kapalı
├── ⏰ Komut Timeout: 2700 saniye
├── 🔄 Güncelleme Kontrolü: Haftalık
├── 🛡️ Checksum Kontrolü: Etkin
└── 📊 İstatistik Paylaşımı: Kapalı
```

### Scoop Konfigürasyonu

```
🥄 Scoop Ayarları:
├── 📍 Kurulum Dizini: ~/scoop
├── 🌐 Global Kurulumlar: Kapalı
├── 🔄 Cache Temizleme: Otomatik
├── 📊 Bucket Güncellemesi: Günlük
├── 🔗 Shim Oluşturma: Etkin
└── 📜 Aria2 İndirici: Etkin
```

### 🔔 Bildirim Ayarları

### Bildirim Türleri

| Bildirim | Açıklama |
| --- | --- |
| **Kurulum Tamamlandı** | Paket kurulumu bitti |
| **Güncelleme Mevcut** | Yeni sürüm bulundu |
| **Hata Oluştu** | İşlem başarısız |
| **Batch İşlem** | Toplu işlem durumu |
| **Başlangıç** | Uygulama başladı |

### 🛡️ Güvenlik Ayarları

### Güvenlik Politikaları

```
🔒 Güvenlik Ayarları:
├── 🛡️ UAC Yükseltme: Gerektiğinde
├── 📝 Dijital İmza: Kontrol et
├── 🔍 Hash Doğrulama: Etkin
├── 🚫 Güvenilmeyen Kaynaklar: Engelle
├── 📊 Telemetri: Temel
└── 🔄 Otomatik Yedekleme: Haftalık
```

### 📁 Gelişmiş Ayarlar

### Export/Import Seçenekleri

```
📤 Dışa/İçe Aktarma:
├── 📋 Paket Listesi: JSON/XML/CSV
├── ⚙️ Ayarlar: Yedekle/Geri yükle
├── 📊 Geçmiş: Tam/Özet
├── 🔧 Konfigürasyon: Taşınabilir
└── 📦 Batch Kurulum: Script oluştur
```

## 🎯 Paket Yöneticileri Detayları

### 🪟 Windows Package Manager (Winget)

### Özellikler ve Avantajlar

```
🪟 Winget Avantajları:
├── 🏢 Microsoft Resmi Desteği
├── 🔒 Güvenlik ve Güvenilirlik
├── 🚀 Windows 11'de Varsayılan
├── 📊 Büyük Paket Deposu (10K+)
├── 🔄 Otomatik Güncellemeler
└── 🛡️ Dijital İmza Kontrolü
```

### 🍫 Chocolatey

### Özellikler ve Avantajlar

```
🍫 Chocolatey Avantajları:
├── 📦 Geniş Paket Yelpazesi (8K+)
├── 🛠️ PowerShell Entegrasyonu
├── 🔧 Dependency Yönetimi
├── 🏢 Kurumsal Çözümler
├── 📊 Community Desteği
└── 🔄 Batch İşlemler
```

### Chocolatey Komutları

```powershell
# Temel Chocolatey komutları
                
# Kurulu paketleri listele
choco list    
      
# Paket ara
choco search paket_adi 

# Paket kur
choco install paket_adi  
          
# Tümünü güncelle
choco upgrade all  
   
# Paket kaldır
choco uninstall paket_adi 
```

### 🥄 Scoop

### Özellikler ve Avantajlar

```
🥄 Scoop Avantajları:
├── 🚀 Hızlı ve Hafif
├── 📂 Portable Uygulamalar
├── 🔧 Geliştirici Odaklı
├── 📝 Basit JSON Manifest
├── 🏠 User-level Kurulumlar
└── 🔗 Symlink Desteği
```

### Scoop Bucket’ları

| Bucket | Açıklama | Paket Örnekleri |
| --- | --- | --- |
| **main** | Temel araçlar | git, python, nodejs |
| **extras** | GUI uygulamaları | chrome, vscode, discord |
| **versions** | Çoklu sürümler | python27, java8, nodejs14 |
| **games** | Oyunlar | steam, minecraft, unity |

### 📱 npm (Node Package Manager)

### Özellikler ve Avantajlar

```
📱 npm Avantajları:
├── 🌍 En Büyük Paket Deposu (2M+)
├── 🚀 JavaScript Ekosistemi
├── 🔧 Geliştirici Araçları
├── 📦 Dependency Management
├── 🔄 Semantic Versioning
└── 🌐 Global/Local Kurulumlar
```

### 🐍 pip (Python Package Manager)

### Özellikler ve Avantajlar

```
🐍 pip Avantajları:
├── 🧮 Python Paketleri (400K+)
├── 🔬 Bilimsel Kütüphaneler
├── 🤖 Machine Learning
├── 🌐 Web Frameworks
├── 🔧 Automation Tools
└── 📊 Data Science
```

## 💡 İpuçları ve Püf Noktaları

### 🚀 Hızlı Kullanım İpuçları

**Klavye Kısayolları**

```
⌨️ Önemli Kısayollar:
├── Ctrl + F: Arama yap
├── Ctrl + R: Listeyi yenile
├── Ctrl + A: Tümünü seç
├── Ctrl + Shift + U: Tümünü güncelle
├── Ctrl + E: Dışa aktar
├── F5: Sayfayı yenile
├── Ctrl + Q: Uygulamayı kapat
└── Ctrl + , : Ayarları aç
```

**Batch İşlemler**

```
🔄 Toplu İşlem İpuçları:
├── Ctrl + Sol Tık: Çoklu seçim
├── Shift + Sol Tık: Aralık seçimi
├── Ctrl + A: Tümünü seç
├── Sağ Tık: Bağlam menüsü
└── Ara çubuğu: Hızlı filtre
```

### 🔧 Sorun Giderme İpuçları

### Yaygın Sorunlar ve Çözümler

```
🛠️ Sorun Giderme:
├── Yavaş Arama:
│   └── Cache'i temizle + Yeniden indeksle
├── Kurulum Hatası:
│   └── Yönetici modunda çalıştır
├── Güncelleme Problemi:
│   └── Kaynakları yenile + UAC kontrol
├── Ağ Hatası:
│   └── Proxy ayarları + Güvenlik duvarı
└── Memory Leak:
    └── Uygulamayı yeniden başlat
```

## 🔧 Sorun Giderme

### 🚨 Yaygın Sorunlar

### Kurulum ve Başlatma Sorunları

```
❌ Kurulum Sorunları:
├── Problem: "UniGetUI başlamıyor"
│   ├── Çözüm 1: .NET 8.0 kurulumunu kontrol et
│   ├── Çözüm 2: Windows güncellemelerini yap
│   └── Çözüm 3: Yönetici olarak çalıştır
|
|
├── Problem: "Paket yöneticisi algılanmıyor"
│   ├── Çözüm 1: PATH değişkenini kontrol et
│   ├── Çözüm 2: Yeniden başlat
│   └── Çözüm 3: Manuel kurulum yap
|
|
└── Problem: "Erişim reddedildi"
    ├── Çözüm 1: UAC ayarlarını kontrol et
    ├── Çözüm 2: Antivirus istisnası ekle
    └── Çözüm 3: Windows Defender kontrol et
```

### Ağ ve Bağlantı Sorunları

| Sorun | Belirtiler | Çözüm |
| --- | --- | --- |
| **Proxy Sorunu** | Paketler yüklenmiyor | Proxy ayarlarını yapılandır |
| **DNS Hatası** | Repolara erişim yok | DNS ayarlarını değiştir |
| **Firewall Engeli** | Bağlantı zaman aşımı | UniGetUI’yi güvenlik duvarından geçir |
| **SSL Sertifika** | Güvenlik uyarıları | Sertifika deposunu güncelle |

### 🔍 Tanılama Araçları

### Sistem Kontrolü

```powershell
# Winget tanılama
winget --info
winget source list
winget validate
# Chocolatey tanılama
choco doctor
choco feature list
choco config list
# Scoop tanılama
scoop checkup
scoop status
scoop config
```

### 🛠️ Gelişmiş Çözümler

### Temiz Kurulum

```
🔧 Temiz Kurulum Adımları:
1. UniGetUI'yi kaldır
2. %appdata%\UniGetUI klasörünü sil
3. %localappdata%\UniGetUI klasörünü sil
4. Registry'den kalıntıları temizle
5. Sistemi yeniden başlat
6. UniGetUI'yi yeniden kur
```

## ❓ Sıkça Sorulan Sorular

### Genel Sorular

**S: UniGetUI ücretsiz mi?**
A: Evet, UniGetUI tamamen ücretsiz ve açık kaynak kodludur. MIT lisansı altında dağıtılmaktadır.

**S: Hangi Windows sürümlerinde çalışır?**
A: Windows 10 1903 ve sonrası tüm sürümlerde çalışır. Windows 11’de en iyi performansı verir.

**S: Paket yöneticilerini ayrı ayrı kurmam gerekiyor mu?**
A: Evet, UniGetUI sadece mevcut paket yöneticilerini yönetir. Önce istediğiniz paket yöneticilerini kurmalısınız.

### Güvenlik Soruları

**S: UniGetUI paketlerin güvenliğini nasıl garanti ediyor?**
A: UniGetUI, paket yöneticilerinin kendi güvenlik kontrollerini kullanır. Winget için dijital imza, Chocolatey için checksum kontrolü yapar.

**S: Antivirüs UniGetUI’yi virüs olarak gösteriyor, ne yapmalıyım?**
A: Bu yaygın bir durumdur. UniGetUI’yi antivirüs beyaz listesine ekleyin. Uygulama açık kaynak kodludur ve güvenlidir.