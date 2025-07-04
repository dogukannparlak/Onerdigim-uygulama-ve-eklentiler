# Stremio

## 🎬 Bölüm 1: Stremio’ya Giriş: Modern Medya Merkezi Kavramı

### 1.1. Stremio Nedir? Bir Medya Toplayıcısı Olarak Tanımı ve Felsefesi

Stremio, 2015 yılında Bulgar girişim Stremio Ltd. tarafından geliştirilen, çağdaş bir **medya toplama platformu** (media aggregator) olarak konumlanmıştır. Temel misyonu, Netflix, Amazon Prime Video, YouTube, Twitch gibi birden çok platformda dağınık halde bulunan video içeriklerini tek bir birleşik arayüz altında organize etmek ve erişilebilir kılmaktır.

### Felsefi Yaklaşım: “Toplayıcı” Modelinin Gücü

Stremio’nun stratejik yaklaşımı, içeriği kendi sunucularında barındırma yerine, mevcut kaynakları **toplama** (aggregation) prensibine dayanır. Bu felsefe, modern medya tüketimindeki temel problemi çözer: **platform parçalanması**. Kullanıcılar artık farklı hizmetler arasında sürekli geçiş yapmak zorunda kalmadan, tek bir arayüzden tüm içerik evrenine erişebilir.

### İş Modeli ve Konumlandırma

```
Stremio'nun Stratejik Konumlandırması:
├── Resmi Statü: Yasal İçerik Düzenleyici
├── Fiili Kullanım: Kapsamlı Medya Erişim Platformu
├── Gelir Modeli: AdEx kardeş şirketi üzerinden reklam
└── Yasal Strateji: "Makul İnkar Edilebilirlik" Çerçevesi
```

### 1.2. Açık Kaynak Yapısı ve Topluluk Odaklı Geliştirme

**Açık Kaynak Felsefesi**: Stremio’nun web versiyonu tamamen açık kaynaklıdır ve GitHub üzerinden herkesin incelemesine açıktır. Bu şeffaflık iki kritik avantaj sağlar:

1. **Güvenlik Şeffaflığı**: Kodun kamu denetimine açık olması, potansiyel güvenlik açıklarının topluluk tarafından tespit edilmesini sağlar
2. **Topluluk Odaklı Büyüme**: Platform gelişimi merkezi kontrolden çıkarak, kullanıcı ihtiyaçları doğrultusunda organik olarak şekillenir

### Topluluk Ekosisteminin Dinamikleri

Platform’ın asıl gücü, **topluluk tarafından geliştirilen eklentiler**de yatmaktadır. Bu ekosistem, Stremio’yu statik bir uygulamadan dinamik ve sürekli evrilen bir hizmet platformuna dönüştürür.

## 🔧 Bölüm 2: Kurulum, Arayüz ve Temel Kullanım

### 2.1. Geniş Platform Desteği ve Kurulum Stratejisi

### Desteklenen Platformlar

| Platform | Durum | Eklenti Desteği | Özellik Durumu |
| --- | --- | --- | --- |
| **Windows** | ✅ Tam Destek | ✅ Tam | Tüm özellikler |
| **macOS** | ✅ Tam Destek | ✅ Tam | Tüm özellikler |
| **Linux** | ✅ Tam Destek | ✅ Tam | Tüm özellikler |
| **Android** | ✅ Tam Destek | ✅ Tam | Tam işlevsellik |
| **Android TV** | ✅ Tam Destek | ✅ Tam | Ev sinema deneyimi |
| **iOS** | ⚠️ Sınırlı | ❌ Yok | Temel işlevler |
| **Web** | ✅ Tam Destek | ✅ Tam | Tarayıcı tabanlı |

### iOS Kısıtlaması: Stratejik Bir Sorun

iOS’taki eklenti desteği eksikliği, platform için kritik bir handikaptır. Bu durum, iOS kullanıcılarını Chromecast veya Apple TV üzerinden yayın yapmaya zorlar, bu da entegre deneyimi bozar.

### 2.2. Hesap Yönetimi: Cihazlar Arası Senkronizasyonun Stratejik Önemi

### Bulut Tabanlı Senkronizasyon Modeli

```
Senkronize Edilen Veriler:
├── 🎭 Kişisel Kütüphane
├── 📺 İzleme Geçmişi ("Kaldığın Yerden Devam")
├── ⭐ Favori İçerikler
├── 🔌 Eklenti Yapılandırması
├── ⚙️ Kullanıcı Tercihleri
└── 📅 Takvim Verileri
```

Bu **“tak-çalıştır”** yaklaşımı, Stremio’yu Kodi gibi rakiplerinden ayıran temel farklılaştırıcıdır. Kullanıcı bir cihazda eklenti kurduğunda, bu ayarlar hesabına kaydedilir ve diğer tüm cihazlara otomatik yansır.

### 2.3. Kullanıcı Arayüzü Anatomisi: Sezgisel ve İşlevsel Tasarım

### Üç Ana Bölüm Mimarisi

**1. Pano (Board) - Kişiselleştirilmiş İçerik Akışı**
- Devam eden dizilerin yeni bölümleri
- İzlemeye devam edilen filmler
- Kişiselleştirilmiş öneriler
- Yakında çıkacak içerikler

**2. Keşfet (Discover) - İçerik Keşif Merkezi**
- Popülerlik, tür, IMDb puanı filtreleri
- Dinamik kategori listeleri
- Trend analizi ve öneriler
- Gelişmiş arama algoritmaları

**3. Kütüphane (Library) - Kişisel Koleksiyon Yönetimi**
- İzleme listeleri
- Favori işaretlemeler
- İzleme geçmişi takibi
- Kişisel notlar ve değerlendirmeler

## 🔌 Bölüm 3: Eklenti Ekosistemi: Platformun Kalbi

### 3.1. Eklenti Mimarisinin Teknik Analizi

### Sunucu Taraflı vs İstemci Taraflı Mimari

**Stremio’nun Sunucu Taraflı Yaklaşımı:**

```
Kullanıcı → Stremio App → Eklenti Sunucusu → İçerik Kaynağı
```

**Avantajları:**
- ✅ **Güvenlik**: Kullanıcı cihazında kod çalıştırılmaz
- ✅ **Basitlik**: Tek tıkla eklenti kurulumu
- ✅ **Senkronizasyon**: Bulut tabanlı yapılandırma
- ✅ **Güncelleme**: Otomatik eklenti güncellemeleri

**Dezavantajları:**
- ❌ **Kırılganlık**: Tek başarısızlık noktası riski
- ❌ **Bağımlılık**: Üçüncü taraf sunucu istikrarına bağımlılık
- ❌ **Kontrol**: Sınırlı yerel kontrol imkanı

### 3.2. Eklenti Kategorileri: Resmi vs Topluluk

### Resmi Eklentiler - Güvenli Temel

| Eklenti | İşlev | Kaynak | Yasal Durum |
| --- | --- | --- | --- |
| **YouTube** | Video akışı | Google | ✅ Tamamen yasal |
| **Twitch** | Canlı oyun yayınları | Amazon | ✅ Tamamen yasal |
| **WatchHub** | İçerik bulma | Çeşitli yasal platformlar | ✅ Tamamen yasal |
| **OpenSubtitles** | Altyazı sağlama | OpenSubtitles.org | ✅ Tamamen yasal |
| **FilmOn** | Canlı TV | FilmOn Networks | ✅ Tamamen yasal |

### Topluluk Eklentileri - Güçlü Ama Riskli

| Eklenti | Popülerlik | Risk Seviyesi | Kullanım Alanı |
| --- | --- | --- | --- |
| **Torrentio** | ⭐⭐⭐⭐⭐ | 🟡 Orta | Torrent kaynaklı içerik |
| **Cyberflix Catalog** | ⭐⭐⭐ | 🟡 Orta | Film/dizi katalogları |
| **USA TV** | ⭐⭐⭐ | 🟡 Orta | Canlı TV kanalları |

## ⚡ Bölüm 4: Olmazsa Olmaz Eklentiler ve Gelişmiş Yapılandırmalar

### 4.1. Torrentio: Stremio Deneyiminin Belkemiği

### Torrentio’nun Stratejik Önemi

Torrentio, neredeyse tüm ileri düzey kullanıcılar için **Stremio deneyiminin bel kemiğini** oluşturur. Bu eklenti olmadan Stremio, potansiyelinin sadece küçük bir kısmını gerçekleştirebilir.

### Yapılandırma Süreci

```
Torrentio Kurulum Aşamaları:
1. https://torrentio.strem.fun/configure adresine git
2. Torrent sağlayıcılarını seç (YTS, 1337x, RARBG, etc.)
3. Kalite filtrelerini ayarla (4K, 1080p, 720p)
4. CAM/Screener gibi düşük kaliteyi filtrele
5. Real-Debrid API anahtarını entegre et (opsiyonel)
6. Konfigürasyonu Stremio'ya yükle
```

### Torrent Sağlayıcı Seçimi Stratejisi

| Sağlayıcı | Güçlü Yönler | Zayıf Yönler | Önerilen Kullanım |
| --- | --- | --- | --- |
| **YTS** | 4K kalite, düşük boyut | Sadece filmler | Film odaklı kullanım |
| **1337x** | Geniş içerik yelpazesi | Değişken kalite | Genel amaçlı |
| **RARBG** | Yüksek kalite, güvenilir | Sınırlı içerik | Kalite odaklı |
| **EZTV** | TV dizilerine odaklı | Sadece diziler | Dizi takibi |

### 4.2. Trakt Entegrasyonu: Kişiselleştirilmiş İzleme Yönetimi

### Trakt’ın Ekosistem Değeri

```
Trakt Ekosistemi:
├── 📊 İzleme İstatistikleri
├── 📝 Kişisel Notlar ve Puanlar
├── 👥 Sosyal Medya Özellikleri
├── 📅 Takvim Entegrasyonu
├── 🔄 Platform Arası Senkronizasyon
└── 🎯 Kişiselleştirilmiş Öneriler
```

### Scrobbling: Otomatik İzleme Takibi

Trakt eklentisi kurulduğunda, Stremio’daki tüm izleme aktivitesi otomatik olarak Trakt hesabınızla senkronize olur. Bu “scrobbling” özelliği:
- İzlenen bölümleri otomatik işaretler
- İzleme süresini kaydeder
- Kişisel istatistikler oluşturur
- Sosyal paylaşım imkanı sunar

## ⚖️ Bölüm 5: Yasal, Güvenlik ve Gizlilik Analizi

### 6.1. Yasal Durum Analizi: Karmaşık Bir Manzara

### Yasal Çerçeve Ayrıştırması

```
Yasal Sorumluluk Katmanları:
├── 🟢 Stremio Uygulaması → %100 Yasal
├── 🟡 Resmi Eklentiler → %100 Yasal
├── 🟠 Topluluk Eklentileri → Gri Alan
├── 🔴 Kullanılan İçerik → Kullanıcı Sorumluluğu
└── ⚫ Dağıtım/Ticari Kullanım → Ciddi Risk
```

### Ülke Bazlı Risk Değerlendirmesi

| Ülke/Bölge | Risk Seviyesi | Yasal Durum | Öneri |
| --- | --- | --- | --- |
| **ABD** | 🔴 Yüksek | DMCA uyarıları | VPN zorunlu |
| **Almanya** | 🔴 Yüksek | Yüksek para cezaları | VPN zorunlu |
| **İngiltere** | 🟡 Orta | ISP engellemeleri | VPN önerilen |
| **Fransa** | 🟡 Orta | HADOPI sistemi | VPN önerilen |
| **Türkiye** | 🟡 Orta-Düşük | Gri alan | VPN önerilen |
| **Hollanda** | 🟢 Düşük | Bireysel kullanım tolere | İsteğe bağlı |

### 6.2. VPN Kullanımının Kritik Önemi

### VPN Seçim Kriterleri

```
Stremio için İdeal VPN Özellikleri:
├── 🚫 No-Log Politikası
├── 🌍 Geniş Sunucu Ağı
├── ⚡ Yüksek Hız (25+ Mbps)
├── 🔒 Strong Encryption (AES-256)
├── 🛡️ Kill Switch Özelliği
├── 💰 Uygun Fiyat
└── 📱 Multi-platform Desteği
```

### 6.3. Güvenlik Risk Değerlendirmesi

### Potansiyel Güvenlik Tehditleri

```
Risk Matrisi:
├── 🔴 Yüksek Risk: Bilinmeyen eklentiler
├── 🟡 Orta Risk: Popüler topluluk eklentileri
├── 🟢 Düşük Risk: Resmi eklentiler
└── ⚪ Minimal Risk: Sadece yerel medya
```

### Güvenlik En İyi Uygulamaları

1. **Güvenilir Kaynaklardan Eklenti Kurulumu**
2. **Düzenli Güvenlik Güncellemeleri**
3. **Endpoint Protection Kullanımı**
4. **Network Monitoring**
5. **DNS Filtreleme**

### 6.4. Gizlilik Politikası İncelemesi

### Stremio’nun Veri Toplama Politikası

```
Toplanan Veriler:
✅ E-posta adresi (hesap yönetimi)
✅ Kütüphane verileri (senkronizasyon)
✅ Uygulama kullanım istatistikleri (anonim)
❌ İzleme geçmişi detayları
❌ Eklenti kullanım logları
❌ IP adresi kayıtları
❌ Kişisel kimlik bilgileri
```