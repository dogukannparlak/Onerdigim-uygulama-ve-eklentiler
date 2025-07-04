# wintoys

---

## 🎯 Genel Bakış

### Araç Hakkında

WinToys, Windows işletim sistemi için geliştirilmiş ücretsiz ve kapsamlı bir sistem yönetim aracıdır. Windows’un gizli özelliklerine erişim sağlayan, sistem optimizasyonu ve yönetimi için gerekli tüm araçları tek bir arayüzde toplayan bu uygulama, teknik kullanıcılar ve power user’lar için vazgeçilmez bir yardımcıdır.

### Hedef Kitle

- **Başlangıç Seviyesi**: Temel sistem yönetimi öğrenmek isteyen kullanıcılar
- **Orta Seviye**: IT profesyonelleri ve sistem yöneticileri
- **Gelişmiş Seviye**: Power user’lar ve geliştiriciler

### Ana Özellikler

- ✅ **Sistem Bilgileri**: Detaylı donanım ve yazılım bilgileri
- ✅ **Uygulamalar**: Kurulu programların yönetimi ve kontrolü
- ✅ **Süreçler**: Aktif işlemlerin izlenmesi ve yönetimi
- ✅ **Servisler**: Windows servislerinin kontrolü
- ✅ **Ağ Araçları**: Ağ yapılandırması ve tanılama
- ✅ **Sistem Araçları**: Windows’un gizli araçlarına hızlı erişim
- ✅ **Optimizasyon**: Sistem performansını artırma
- ✅ **Güvenlik**: Sistem güvenliği ve gizlilik ayarları
- ✅ **Temizlik**: Gereksiz dosyaların temizlenmesi

---

# 🚀 Kurulum ve Başlangıç

### Kurulum Yöntemleri

### 1️⃣ Microsoft Store (Önerilen)

1. Microsoft Store’u açın
2. “WinToys” araması yapın
3. **WinToys** uygulamasını seçin
4. **Al** butonuna tıklayın

### 2️⃣ Winget ile Kurulum

```
winget install "WinToys"
```

### 3️⃣ GitHub Releases

1. https://github.com/bogdandonduk/WinToys/releases adresine gidin
2. En son sürümü indirin: `WinToys-x.x.x-Setup.exe`
3. İndirilen dosyayı çalıştırın

### 4️⃣ Taşınabilir Sürüm

1. GitHub’dan taşınabilir sürümü indirin
2. ZIP dosyasını çıkarın
3. `WinToys.exe` dosyasını çalıştırın

### ⚙️ İlk Yapılandırma

WinToys ilk açılışta:
- Yönetici izinleri isteyebilir
- Sistem taraması gerçekleştirir
- Varsayılan ayarları yükler

---

# 🏠 Giriş - Ana Sayfa

### 📊 Sistem Bilgi Kartları

WinToys’un ana sayfası, sistemin temel bilgilerini kart görünümünde sunar:

### Üst Sıra - Donanım Bilgileri

| Kart | Bilgi Türü | Açıklama | Örnek |
| --- | --- | --- | --- |
| **💻 Sistem** | Model/Build | Bilgisayar modeli | 82K2 |
| **🔧 İşlemci** | CPU Modeli | İşlemci türü ve markası | AMD Ryzen 7 5800H with Radeon Graphics |
| **🎮 Ekran Kartı** | GPU Modeli | Grafik kartı bilgisi | NVIDIA GeForce RTX 3060 Laptop GPU |
| **💾 Hafıza** | RAM Miktarı | Toplam bellek kapasitesi | 16 GB |

### Orta Sıra - Sistem Durumu

| Kart | Bilgi Türü | Açıklama | Örnek |
| --- | --- | --- | --- |
| **💿 Depolama** | Disk Kapasitesi | Toplam depolama alanı | 1,37 TB |
| **🪟 Windows** | İşletim Sistemi | Windows sürümü | 11 |
| **⏱️ Çalışma Süresi** | Uptime | Sistemin açık kalma süresi | 11:03:40:38 |
| **⭐ Performans** | Performans Skoru | Sistem performans değerlendirmesi | 9,2/10 |

### 📈 Canlı İstatistik Kartları

### Alt Panel - Gerçek Zamanlı Veriler

📊 Sistem İstatistikleri:

├── 📱 Uygulamalar: 183 adet kurulu

├── ⚙️ İşlemler: 299 aktif süreç

├── 🔧 Hizmetler: 146 Windows servisi

└── 🧹 Alan Temizlendi: 710.49 MB

### Performans Göstergeleri

| Metrik | Anlık Değer | Açıklama |
| --- | --- | --- |
| **🔧 İşlemci** | %20 | CPU kullanım yüzdesi |
| **🎮 Ekran Kartı** | %43 | GPU kullanım yüzdesi |
| **💾 Hafıza** | %80 | RAM kullanım yüzdesi |
| **🌐 Ağ** | 199,56 GB | Toplam ağ trafiği |

### Ağ Aktivitesi

🌐 Ağ Aktivitesi:

├── Download Hızı: ↓ 1.2 KB/s

├── Upload Hızı: ↑ 0 B/s

└── Toplam Veri: 199,56 GB

---

# 📱 Uygulamalar

## 🔍 Uygulama Arayüzü ve Navigasyon

### Ana Arayüz Elemanları

WinToys Uygulamalar sekmesi şu bileşenlerden oluşur:

| Bileşen | Konum | İşlev | Kullanım |
| --- | --- | --- | --- |
| **🔍 Arama Çubuğu** | Üst sol | “Uygulama bul” | Hızlı uygulama arama |
| **📊 Uygulama Sayacı** | Üst orta | “183 uygulamalar” | Toplam kurulu uygulama sayısı |
| **🔽 Filtre/Sıralama** | Üst sağ | Dropdown menüler | Liste özelleştirme |
| **📋 Uygulama Listesi** | Ana alan | Detaylı liste | Tüm uygulamaları görüntüle |

## 🎨 Renk Kodlama Sistemi

### Uygulama Türü Göstergeleri

WinToys, uygulamaları türlerine göre renk kodlaması ile ayırt eder:

| Renk | Tür | Açıklama | Örnekler |
| --- | --- | --- | --- |
| 🟡 **Sarı** | Win32 Uygulamaları | Klasik masaüstü programları | 7-Zip, Chrome, Photoshop |
| 🔵 **Mavi** | Microsoft Store Apps | UWP/Modern uygulamalar | Amazon Games, Apple TV, Ayarlar |

### Uygulama Liste Görünümü

📱 Gerçek Uygulama Listesi Formatı:

```
🟡 7-Zip 24.09 (x64) 5.59 MB ⋯
   24.9.0.0 | Igor Pavlov 17.09.2024

🔵 Amazon Games 451 MB ⋯
   3.0.9495.3 | Amazon.com Services, Inc. 16.03.2025

🔵 AMD Radeon Software 612.79 MB ⋯
   10.23.19011.0 | Advanced Micro Devices 19.06.2025
```

## ⚙️ Uygulama Detay Bilgileri

### Her Uygulama İçin Gösterilen Bilgiler

| Bilgi | Açıklama | Örnek | Konum |
| --- | --- | --- | --- |
| **📱 Uygulama Adı** | Program başlığı | “7-Zip 24.09 (x64)” | Sol üst |
| **🏷️ Sürüm** | Versiyon numarası | “24.9.0.0” | Alt satır sol |
| **🏢 Geliştirici** | Yapımcı şirket | “Igor Pavlov” | Alt satır orta |
| **💾 Boyut** | Disk kullanımı | “5.59 MB” | Sağ üst |
| **📅 Kurulum Tarihi** | Yüklenme tarihi | “17.09.2024” | Sağ alt |
| **⋯ Eylem Menüsü** | Üç nokta butonu | Sağ tık menüsü | En sağ |

## 🎛️ Uygulama Eylemleri

### Sağ Tık Menü Seçenekleri

Uygulamaların yanındaki “⋯” butonuna tıklayarak erişilebilen eylemler:

| Eylem | Simge | Açıklama | Kullanım |
| --- | --- | --- | --- |
| **⚡ Kapat** | 🔌 | Uygulamayı sonlandır | Açık programları kapat |
| **📁 Gözat** | 📂 | Dosya konumunu aç | Kurulum klasörüne git |
| **🔍 Arama** | 🔎 | Web’de ara | Uygulama hakkında bilgi |
| **🔄 Sıfırla** | ↻ | Uygulama verilerini sıfırla | Sorun giderme |
| **🗑️ Kaldır** | ❌ | Uygulamayı kaldır | Tam kaldırma |

---

# ⚙️ Hizmetler

## 🔍 Hizmetler Arayüzü

### Ana Arayüz Bileşenleri

WinToys Hizmetler sekmesi Windows servislerini yönetmek için kapsamlı araçlar sunar:

| Bileşen | Konum | İşlev | Kullanım |
| --- | --- | --- | --- |
| **🔍 Arama Çubuğu** | Üst sol | “Arama hizmetleri” | Hizmet ara |
| **📊 Hizmet Sayacı** | Üst orta | “146 hizmetler” | Toplam hizmet sayısı |
| **🔽 Filtre Menüsü** | Üst sağ | Kategorik filtreler | Hizmet türü seçimi |
| **📋 Hizmet Listesi** | Ana alan | Detaylı hizmet bilgileri | Tam görünüm |

## 🎨 Hizmet Durum Göstergeleri

### Görsel Durum Çizgileri

| Renk | Durum | Açıklama | Örnek Hizmetler |
| --- | --- | --- | --- |
| 🟢 **Yeşil Çizgi** | Çalışıyor | Aktif olarak çalışan hizmetler | AMD Crash Defender Service |
| ⚫ **Çizgi Yok** | Durdurulmuş | Pasif/durdurulmuş hizmetler | Ağ Bağlantısı Aracısı |
| 🔵 **Mavi Vurgu** | Seçili | Aktif olarak seçilen hizmet | - |

### Hizmet Bilgi Formatı

📋 Gerçek Hizmet Liste Formatı:

```
🟢 AMD Crash Defender Service    Çalışıyor  Otomatik  ⋯
   C:\WINDOWS\System32\DriverStore\...amdfedr.exe

   Ağ Bağlantısı Aracısı         Çalışıyor  Elle      ⋯
   C:\WINDOWS\System32\svchost.exe
```

## 🗂️ Filtre ve Kategori Sistemi

### Hizmet Filtreleri

Sağ üst köşedeki filtre menüsü ile hizmetleri kategorilere ayırabilirsiniz:

| Filtre | Açıklama | Kullanım |
| --- | --- | --- |
| **Tümü** | Tüm hizmetleri göster | Genel görünüm |
| **Kullanışsız** | Gereksiz hizmetler | Optimizasyon için |
| **Microsoft** | Microsoft hizmetleri | Sistem hizmetleri |
| **Üçüncü taraf** | 3. parti hizmetler | Kurulu program hizmetleri |
| **Durum** | Durum bazlı filtre | Çalışan/durmuş |
| **Mod** | Başlangıç türü | Otomatik/Manuel |

## 🎛️ Hizmet Yönetim Eylemleri

### Sağ Tık Menü Seçenekleri

Her hizmetin yanındaki “⋯” menüsünden erişilebilen eylemler:

| Eylem | Simge | Açıklama | Kullanım |
| --- | --- | --- | --- |
| **▶️ Başlat** | ▶️ | Durdurulmuş hizmeti başlat | Hizmet başlatma |
| **⏹️ Durdur** | ⏹️ | Çalışan hizmeti durdur | Sorun giderme |
| **🔄 Yeniden Başlat** | 🔄 | Hizmeti yeniden başlat | Yenileme |
| **📁 Gözat** | 📁 | Hizmet dosya konumu | Dosya analizi |
| **🔍 Arama** | 🔍 | Web’de hizmet ara | Bilgi alma |
| **⚙️ Mod** | ⚙️ | Başlangıç türü değiştir | Otomasyonu ayarla |

# 🚀 Performans

WinToys Performans sekmesi, sisteminizi maksimum verimlilik için optimize etmenizi sağlayan kapsamlı ayarlar sunar:

## 🔋 Güç ve Performans Yönetimi

| Ayar | Açıklama |
| --- | --- |
| **⚡ Nihai performans güç planı** | Bileşenlerin maksimum performans için ihtiyaç
duydukları tüm gücü tüketmelerine olanak tanır |
| **🎮 HAGS (Donanım Hızlandırmalı GPU)** | Ekran kartının görevleri daha verimli bir şekilde tahsis hti)
etmesini sağlayarak işlemci gecikmesini ve kullanım
yükünü azaltır |
| **🛡️ VBS (Sanallaştırma Tabanlı Güvenlik)** | Güvenlik açıklarına ve kötü amaçlı kullanımlara karşı
korumayı artırmak için yalıtılmış bir sanal bellek bölgesi
oluşturur |

📊 Başlangıç Uygulamaları

- Yenile: Listeyi güncelle
- Yeni başlangıç uygulaması ekle: Manuel uygulama ekleme
- Yenisi eklenince bildir: Otomatik uyarı sistemi

## 🔧 Sistem Optimizasyon Ayarları

### Uygulama ve Süreç Yönetimi

| Ayar | Açıklama |
| --- | --- |
| **🔄 Uygulamaları yeniden başlat** | Yeniden başlatılabilir uygulamaları otomatik kaydet ve tekrar oturum açınızda bunları yeniden başlatır |
| **⚙️ Arka plan uygulamaları** | Uygulamaların arka planda çalışmasına izin verir |
| **📋 Etkinlik geçmişi** | Kullandığınız uygulama ve hizmetleri, açtığınız dosyaları ve gezindiğiniz web sitelerini takip eder |

## 🎨 Görsel  Ayarlar

| Ayar | Açıklama |
| --- | --- |
| **🎭 En iyi performans için görsel efektleri ayarlayın** | Windows kullanıcı arayüzü ile ilgili ayarlar |
| **💎 Saydamlık** | Şeffaflık efektleri |

## 🎮 Oyun Ayarları

| Ayar | Açıklama |
| --- | --- |
| **🎯 Oyun modu** | Belirli oyunlarda kare hızını artırabilecek ayarlar |
| **🪟 Pencereli mod iyileştirme seçenekleri** | Pencereli oyunlarda performans iyileştirmeleri |
| **📹 Arka planda kayıt** | Arka plan oyun kaydı özelliği |
| **💾 Diskten Hızlı Getirme** | Disk’ten verileri hızlı okuma |

## 🔍 Sistem Hizmetleri Optimizasyonu

### Arka Plan Hizmetleri

| Hizmet | Açıklama |
| --- | --- |
| **🔍 Arama indeksleme** | Daha hızlı arama sonuçları sağlayarak indekslemenin arka planda çalışmasına izin verir |
| **📦 Teslim İyileştirme** | İndirilen Windows güncellemelerini yerel ağınızda veya internetten diğer cihazlarla paylaşır |
| **🌐 Ağ bağdaştırıcısı yerleşik işlemci** | Bazı ağ işlemlerini işlemcinizden ağ bağdaştırıcının yerleşik işlemcisine aktarır |

---

# 🏥 Sağlık

## ⚡ Sistem Performans ve Hızlandırma

### Önyükleme ve Güç Yönetimi

| Ayar | Açıklama |
| --- | --- |
| **🚀 Hızlı başlatmayı** | Cihazın kapatıldıktan sonra daha hızlı açılmasını sağlayarak önyükleme süresini  azaltır |
| **😴 Hazırda bekletme** | Açık uygulamalarınız da dahil olmak üzere işletim sisteminin durumunu diskte hiberfil.sys adlı bir dosyaya kaydeder |

## 🧹 Temizlik

### Manuel Temizlik Seçenekleri

WinToys’un Temizlik bölümü çeşitli sistem alanlarını temizlemenizi sağlar:

| Temizlik Türü | Açıklama |
| --- | --- |
| **🗑️ Gereksiz** | Geçici dosyalar, çöp kutusu, cache |
| **📁 Dosya Gezgini** | Dosya gezgini geçmişi ve önbellekleri |
| **🏪 Microsoft Store** | Store uygulamaları cache’i |
| **🌐 DNS** | DNS önbelleğini temizle |
| **🗑️ Sistem Geri Yükleme** | Eski geri yükleme noktalarını sil |

### Otomatik Sistem Bakımı

| Özellik | Açıklama |
| --- | --- |
| **⚡ Sürücü İyileştirme** | Cihazınızın daha verimli çalışmasına yardımcı olur |
| **🧹 Akıllı Depolama** | Bazı geçici sistem dosyalarını otomatik olarak temizler |

## **🔋 Pil Raporu**

### **Kapsamlı Pil Durumu Analizi**

WinToys'un Sağlık bölümü, dizüstü bilgisayarlar için detaylı pil analizi yapabilir. **"Pil raporu oluştur"** butonu ile PowerShell komutu çalıştırarak kapsamlı bir HTML raporu oluşturur.

### **Pil Raporu Örneği**

**⚠️ Not:** Aşağıdaki veriler örnek amaçlıdır. Gerçek verileriniz farklı olacaktır.

**📊 Pil Genel Bilgileri:**

```
🔋 Pil Model: L20D4PC0
🏭 Üretici: Sunwoda
🔢 Seri No: 6000
⚗️ Kimya: Li-Ion (Lityum İyon)
📅 Rapor Tarihi: 2025-06-24 01:54:21

```

**📈 Kapasite Durumu:**

| Metrik | Örnek Değer |
| --- | --- |
| **🎯 Tasarım Kapasitesi** | 60.000 mWh |
| **⚡ Tam Şarj Kapasitesi** | 49.720 mWh |
| **🔄 Şarj Döngüsü** | 420 döngü |
| **📉 Kapasite Kaybı** | 10.280 mWh |

### **Pil Sağlık Değerlendirmesi**

| Sağlık Durumu | Kapasite Oranı | Açıklama |
| --- | --- | --- |
| **🟢 Mükemmel** | %90-100 | Yeni pil performansı |
| **🟢 İyi** | %80-89 | Sağlıklı çalışma durumu |
| **🟡 Orta** | %60-79 | Belirgin kapasite azalması |
| **🔴 Zayıf** | %40-59 | Pil değişimi yaklaşıyor |
| **🔴 Kritik** | <%40 | Acil pil değişimi |

### **Örnek Kullanım Analizi (Son 7 Gün)**

**⚡ Pil Kullanım Seansları:**

```
📅 2025-06-20: 1:09 dakika kullanım → %1 enerji tüketimi (640 mWh)
📅 2025-06-23: 1:19:51 kullanım → %63 enerji tüketimi (31.280 mWh)
📅 2025-06-23: 1:13:33 kullanım → %76 enerji tüketimi (37.700 mWh)

```

**📊 Pil Performans Örneği:**

- **🔋 Aktif Kullanım**: 2:19:35 saat (örnek tahmin)
- **⏱️ Tasarım Hedefi**: 2:48:27 saat (yeni pil)
- **📉 Performans Farkı**: %17 azalma
- **🎯 Günlük Ortalama**: 45 dakika pil kullanımı

## **🔧 Onar**

WinToys'un Onar sekmesi kapsamlı sistem onarım araçları sunar:

🛠️ Sistem Tanılama Araçları:

**🔧 DISM (Deployment Image Servicing and Management)**

- Bozuk sistem dosyalarını veya bileşenlerini değiştirmek için kullanılan yerel Windows görüntüsünü, sağlıklı indirmiş olan yedek olarak kontrol eder ve onarır
- ⚠️ İnternet bağlantısı gerektirir

**🔍 SFC (System File Checker)**

- Tüm korunan sistem dosyalarını tarar ve DISM tarafından sunulan önbelleğe alınmış bir kopya kullanarak bozuk olanları değiştirir

**💾 CHKDSK (Check Disk)**

- Depolama cihazınızı kontrol eder ve onarır (bozuk sektörler, okuma/yazma hataları, dosya sistemi)
- ⚠️ C bölümü Windows tarafından kullanılırken kontrol edilemediğinden, işlem bir sonraki yeniden başlatma için programlanacaktır

💡 **Not**: Bu araçların hiçbiri mevcut sorunları çözmezse yeni bir Windows yüklemesi önerilir.

### 🔋 Donanım Tanılama

### Sistem Bileşeni Kontrolleri

| Test Türü | Açıklama |
| --- | --- |
| **🧠 Bellek teşhis** | Muhtemel hafıza sorunları için cihazınızı kontrol edin |
| **🔌 Uyku hapi** | Zamanlanmış görevlerin cihazınızı rastgele uyandırmasını tespit edin ve durdurun |
| **🎮 Grafik sürücüsü** | Ekranınızda donma veya titreme gibi tuhaf sorunlar varsa sürücüyü yeniden başlatın |
| ⏳Simge önbelleği | Simgeleriniz veya küçük resimleriniz boş, bulanık veya
bozuksa önbelleği yeniden oluşturun |

## 🔄 Güncelleme Yönetimi

# 🔧 İnce Ayarlar

WinToys’un İnce Ayarlar sekmesi, Windows’un derinlerinde bulunan gelişmiş yapılandırma seçeneklerini kullanıcı dostu bir arayüzle sunar. Bu bölüm 6 ana kategoriye ayrılmıştır:

## 🖥️ Masaüstü (Desktop)

### Masaüstü Simge ve Görünüm Yönetimi

WinToys’un Masaüstü bölümü, masaüstü deneyiminizi özelleştirmek için kapsamlı seçenekler sunar:

| Ayar | Açıklama |
| --- | --- |
| **💻 Bu Bilgisayar** | Masaüstünde bu bilgisayar ikonun görünmesini sağlar |
| **🗑️ Geri Dönüşüm Kutusu** | Silinen dosyaların geçici depolandığı masaüstü simgesi |
| **📄 Araçlar** | Sistem araçlarına hızlı erişim masaüstü simgesi |
| **🔗 Kısayol oku** | Kısayol simgelerindeki ok işaretlerini gizler/gösterir |
| **🏷️ Simge etiketleri için gölgeler** | Masaüstü simge metinlerinin altında gölge efekti ekler  |
| **🖥️ Masaüstünü Göster** | Sağ alt köşeye basılınca masaüsütüne dönülmesini sağlar/kapatır |
| **📁 Başlık çubuğu pencereleri salla** | Pencere başlığını salladığınızda diğer pencereleri minimize eder (Aero Shake) |
| **🖱️ Klasik içerik menüsü** | Eski Windows sağ tık menü stilini kullanır |
| **🖼️** Duvar Kağıdı Kalitesi | Slider ile masaüstü arka plan görüntünüzün kalitesini ayarlayabilirsiniz. |

## 📱 Başlat Menüsü (Start Menu)

### Başlat Menüsü Gizlilik ve Performans Kontrolü

WinToys’un Başlat Menüsü bölümü, arama davranışı ve veri paylaşımını tam kontrol etmenizi sağlar:

| Ayar | Açıklama |
| --- | --- |
| **🌐 Arama yaparken web sonuçlarını dahil et** | Bing arama motorunu kullanarak internet sonuçlarını başlat menüsünde gösterir |
| **📦 Otomatik yükleme önerileri** | Microsoft Store’dan uygulama önerilerini başlat menüsünde görüntüler |
| **👤 Hesap bildirimleri** | Microsoft hesabınızla ilgili bildirimleri ve önerileri gösterir |
| **💤 Güç menüsünde hazırda bekletme modunu göster** | Güç seçeneklerinde uyku/hibernation modunu görüntüler |

## 📁 Dosya Gezgini (File Explorer)

### Dosya Gezgini Görünüm ve İşlevsellik Kontrolü

WinToys’un Dosya Gezgini bölümü, dosya yönetimi deneyiminizi tam olarak özelleştirmenizi sağlar:

| Ayar | Açıklama | Fayda |
| --- | --- | --- |
| **📄 Dosya uzantısını göster** | Dosya uzantılarını görünür hale getirerek .pdf, .exe, .md gibi uzantıları dosya adlarının sonunda görmenizi sağlar.” | Güvenlik artışı, dosya türü tanıma |
| **👁️ Gizli öğeleri ve sistem öğelerini göster** | Windows tarafından gizlenen sistem dosyalarını ve klasörlerini görüntüler | Gelişmiş sistem kontrolü |
| **📂 Çıkarma işlemi tamamlandıktan sonra dosyaları göster** | Arşiv çıkarma işlemi bittikten sonra hedef klasörü otomatik açar | Kullanılabilirlik artışı |
| **🎨 Klasik Arayüz** | Eski Windows Dosya Gezgini görünümünü kullanır | Nostalji, bazı durumlarda hız |
| **📋 Dosyalar için önizleme bölmesini göster** | Seçili dosyanın önizlemesini sağ panelde gösterir | Hızlı dosya görüntüleme |
| **🗑️ Gezinti bölmesinde geri dönüşüm kutusunu göster** | Sol panelde çöp kutusu kısayolu görüntüler | Hızlı çöp kutusu erişimi |
| **🏠 Giriş** | Dosya Gezgini açılış sayfasını “Seçtiğiniz” yere“Giriş” yapar | Hızlı erişim dosyaları |
| **🖼️ Galeri** | Görsel dosyalar için gelişmiş galeri görünümü | Resim/video yönetimi |
| **☑️ Öğeleri seçmek için onay kutularını kullanın** | Dosya seçimi için onay kutuları ekler | Çoklu seçim kolaylığı |
| **🔄 Sağlayıcı bildirimlerini eşitle** | Bulut depolama senkronizasyon bildirimleri | Senkronizasyon durumu takibi |
| ↗️Şununla Aç  | Dosya Gezgini başlatıldığında açılacak varsayılan konumu seçin: Bu Bilgisayar, Giriş veya İndirilenler. | İstenilen bölüme hızlı erişim |

## 🛡️ Gizlilik (Privacy)

### Kapsamlı Gizlilik ve Telemetri Kontrolü

WinToys’un Gizlilik bölümü, Windows’un veri toplama ve paylaşma davranışını detaylı şekilde kontrol etmenizi sağlar:

| Ayar | Açıklama |
| --- | --- |
| **👤 Konum** | Microsoftun konum verilerinize erişimi |
| **📡 Telemetri** | Microsoft’a tanılama ve kullanım verisi gönderimi |
| **📊 Müşteri Deneyimini Geliştirme Programı** | Windows Customer Experience Improvement Program |
| **📈 Uygulama telemetrisi** | Uygulamaların kullanım verisi toplama |
| **🚀 Uygulama izlemeyi başlat** | Başlangıç uygulamalarının izlenmesi |
| **✍️ Çizim oluşturmayı ve yazmayı geliştirin** | El yazısı ve klavye öğrenme |
| **📝 Çizim oluşturmayı ve yazmayı kişiselleştirin** | Kişisel yazım verisi toplama |
| **❌ Hata raporlama** | Windows Error Reporting servisi |
| **📷 Kilit ekranında kamera** | Kilit ekranı kamera erişimi |
| **📸 Kamera açma/kapama göstergesi** | Kamera kullanım bildirimi |
| **💬 Çevrimiçi konuşma tanıma** | Online speech recognition |

## 📢 Reklamlar (Advertisements)

Ürünleri veya yeni özellikleri tanıtan içeriği görüntüleyebilecek reklamlarla ilgili ayarları değiştirin

| **Öğe** | **Açıklama** |
| --- | --- |
| **Kişiye Özel Deneyimler** | Microsoft’un ürünleri kullanım alışkanlıklarınıza göre kişiselleştirilmiş öneriler sunmasını sağlar. |
| **Reklam Kimliği** | Uygulamaların size özel reklamlar gösterebilmesi için kullanılan benzersiz kimliği etkinleştirir veya devre dışı bırakır. |
| **Ayarlarda Önerilen İçerik** | Ayarlar menüsünde Microsoft’un önerdiği içeriklerin (ipuçları, ürünler vb.) gösterilip gösterilmeyeceğini belirler. |
| **Ayarlarda Ana Sayfa** | Ayarlar uygulaması açıldığında varsayılan olarak ana sayfanın gösterilip gösterilmeyeceğini belirler. |
| **Önerilen Bildirimler** | Windows’un öneri, güncelleme ve tavsiye bildirimlerini gösterip göstermeyeceğini ayarlamanızı sağlar. |
| **Kilit Ekranıyla İlgili Eğlenceli İçerikler, İpuçları ve Püf Noktaları** | Kilit ekranında haberler, ipuçları veya önerilen içeriklerin gösterilip gösterilmeyeceğini ayarlamanızı sağlar. |
| **Windows İpuçları ve Önerileri** | Windows kullanımı hakkında yardımcı olabilecek öneri ve ipuçlarının gösterilmesini sağlar. |
| **Windows’a Hoş Geldiniz Deneyimi** | Yeni güncellemeler veya hesap oturumları sonrası tanıtım içeriklerinin gösterilmesini sağlar. |
| **Cihazınızın Kurulumunu Tamamlayın** | Yeni bir cihaz kurulumunda yapılması gereken ek adımlar için hatırlatmalar sağlar. |

## ⚙️ Sistem (System)

### Gelişmiş Sistem Davranışı ve Performans Ayarları

WinToys’un Sistem bölümü, Windows’un temel işleyişini optimize etmek için kritik ayarlar sunar: İşinizi kolaylaştırabilecek sistemle ilgili ayarları değiştirin

| Ayar | Açıklama |
| --- | --- |
| **🕒 Saniye cinsinden saat** | Görev çubuğu saatinde saniye gösterimini ekler |
| **📵 Görevi sonlandır** | Sağ tık menüsüne “Görevi Sonlandır” seçeneği ekler |
| **📋 Pano geçmişi** | Windows+V ile clipboard geçmişi erişimi |
| **📸 Ekran Yazdırma tuşuyla ekran görüntüsü alma** | Print Screen tuşu ile ekran görüntüsü almanızı sağlar |
| **🐭 Fare hızlandırma** | Mouse acceleration/pointer precision ayarı |
| **🔔 Geri Bildirim Hatırlatmaları** | Windows feedback reminder bildirimleri |
| **🔄 Alt+Tab İçeriği** | Alt+Tab’da hangi içeriklerin gösterileceği |
| **📅 Dijital Pazarlar Yasası** | EU Digital Markets Act compliance ayarları |

### Sistem Ayarları Detaylı Analizi

### Prodüktivite Artırıcı Ayarlar

1. **📋 Pano geçmişi**:
    - **Fayda**: Son 25 kopyalanan öğeye erişim
    - **Kullanım**: Windows+V kısayolu
2. **📸 Print Screen → Snipping Tool**:
    - **Fayda**: Modern ekran görüntüsü deneyimi
    - **Özellikler**: Düzenleme, annotation, otomatik kaydetme
3. **📵 Görevi sonlandır**:
    - **Fayda**: Donmuş uygulamaları hızla kapatma
    - **Kullanım**: Sağ tık → “Görevi Sonlandır”

## 🔐 Yetkili Kullanıcı

### ⚠️ Güvenlik Açığı Riski Oluşturabilecek Gelişmiş Ayarlar

WinToys’un Yetkili Kullanıcı bölümü, sistem güvenliğini etkileyebilecek kritik ayarlar içerir. Bu ayarlar sadece deneyimli kullanıcılar tarafından dikkatli şekilde kullanılmalıdır:

| Ayar | Açıklama | Kullanım Amacı |
| --- | --- | --- |
| **⚠️ God Mode(Tanrı Modu)** | Tüm Windows ayarlarına erişim sağlayan  | Gelişmiş sistem yönetimi |
| **👨‍💻 Geliştirici Modu** | Windows Geliştirici Modu aktivasyonu | Uygulama geliştirme, yan yükleme |
| **👤 Kullanıcı Hesabı Denetimi** | UAC (User Account Control) seviyesi | Sistem güvenlik kontrolü |
| **🛡️ Kullanıcı seçimi koruma sürücüsü** | Windows Defender Credential Guard | Kimlik bilgisi koruması |