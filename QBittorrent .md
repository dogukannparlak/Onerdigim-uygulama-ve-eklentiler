# QBittorrent

## 🎯 Genel Bakış

### BitTorrent Nedir?

**BitTorrent**, dosya paylaşımı için kullanılan peer-to-peer (P2P) bir protokoldür. Geleneksel indirme yöntemlerinden farklı olarak, dosyaları merkezi bir sunucudan değil, ağdaki diğer kullanıcılardan (peer) parçalar halinde alır.

### Nasıl Çalışır?

| Kavram | Açıklama | Örnek |
| --- | --- | --- |
| **Torrent Dosyası** | Dosya bilgilerini içeren küçük dosya | `Ubuntu-22.04.torrent` |
| **Magnet Link** | Torrent bilgisinin URL formatı | `magnet:?xt=urn:btih:...` |
| **Tracker** | Peer’ları buluşturan sunucu | `tracker.ubuntu.com` |
| **Seeder** | Dosyanın tamamına sahip kullanıcı | Upload yapan kişi |
| **Leecher** | Dosyayı indiren kullanıcı | Download yapan kişi |
| **Peer** | Ağdaki her kullanıcı | Seeder + Leecher |
| **Swarm** | Aynı dosyayı paylaşan peer grubu | Ubuntu ISO swarm’ı |

### BitTorrent’in Avantajları

✅ **Dağıtık Sistem**: Tek sunucuya bağımlılık yok
✅ **Hız Artışı**: Çoklu kaynaklardan indirme
✅ **Bandwidth Tasarrufu**: Merkezi sunucu yükü yok
✅ **Dayanıklılık**: Bir peer çıksa sistem devam eder
✅ **Ölçeklenebilirlik**: Daha çok peer = daha hızlı indirme

### BitTorrent’in Dezavantajları

❌ **Upload Gereksinimi**: Paylaşmak zorundasınız
❌ **Gizlilik**: IP adresiniz görünür
❌ **Hukuki Riskler**: Telif hakkı ihlalleri
❌ **Slow Start**: Az peer varsa yavaş başlar

### Torrent Dosya Türleri

### .torrent Dosyaları

```
- Dosya adı ve boyut bilgileri
- Parça (piece) hash değerleri
- Tracker URL'leri
- Yaratılma tarihi
- Açıklama metni
```

### Magnet Linkler

```
magnet:?xt=urn:btih:HASH
&dn=DOSYA_ADI
&tr=TRACKER_URL
&xl=DOSYA_BOYUTU
```

### QBittorrent Hakkında

QBittorrent, Qt framework’ü ve libtorrent kütüphanesi üzerine inşa edilmiş ücretsiz ve açık kaynaklı bir BitTorrent client’ıdır. µTorrent’e alternatif olarak geliştirilmiş olan QBittorrent, reklamsız deneyim, güçlü arama motoru ve WebUI desteği ile öne çıkar.

### Temel Özellikler

- ✅ **Tamamen Ücretsiz**: Hiç reklam, malware veya spyware içermez
- ✅ **Platformlar Arası**: Windows, Linux, macOS, FreeBSD desteği
- ✅ **WebUI Desteği**: Uzaktan erişim ve yönetim
- ✅ **Entegre Arama**: Çoklu torrent sitelerinde arama
- ✅ **RSS Desteği**: Otomatik indirme filtreleri
- ✅ **IPv6 Desteği**: Modern ağ protokolleri
- ✅ **Şifreleme**: Güvenli peer bağlantıları
- ✅ **UPnP/NAT-PMP**: Otomatik port yönlendirme

## 🚀 Kurulum ve Başlangıç

### Kurulum Yöntemleri

### 1️⃣ Windows Kurulumu

**Resmi İndirme**:
1. https://www.qbittorrent.org/download adresine gidin
2. Windows versiyonunu seçin:
- **QBittorrent v5.1.1** (Qt6 + libtorrent 1.2.x)
- **QBittorrent v5.1.1 (qt6 lt20)** (Qt6 + libtorrent 2.0.x)
3. İndirilen `.exe` dosyasını çalıştırın
4. Kurulum talimatlarını takip edin

**Winget ile Kurulum**:

```bash
winget install qBittorrent.qBittorrent
```

**Chocolatey ile Kurulum**:

```bash
choco install qbittorrent
```

### 2️⃣ Linux Kurulumu

**Ubuntu/Debian**:

```bash
sudo apt update
sudo apt install qbittorrent
```

**Fedora**:

```bash
sudo dnf install qbittorrent
```

**Arch Linux**:

```bash
sudo pacman -S qbittorrent
```

**AppImage (Taşınabilir)**:
1. https://www.qbittorrent.org/download adresinden AppImage indirin
2. İzinleri ayarlayın: `chmod +x qbittorrent-*.AppImage`
3. Çalıştırın: `./qbittorrent-*.AppImage`

### 3️⃣ macOS Kurulumu

**Resmi DMG**:
1. https://www.qbittorrent.org/download adresinden macOS versiyonunu indirin
2. DMG dosyasını açın ve uygulamayı Applications klasörüne sürükleyin
3. **Sistem Ayarları** > **Güvenlik** den uygulamayı onaylayın

**Homebrew**:

```bash
brew install qbittorrent
```

### ⚙️ İlk Yapılandırma

### Temel Ayarlar

1. **Dil Seçimi**: Tools → Options → Behaviour → Interface Language
2. **İndirme Klasörü**: Tools → Options → Downloads → Default Save Path

## 💻 Temel İşlemler

### 🔄 Torrent Çalışma Mantığı

### İndirme Süreci Adım Adım

1. **Torrent/Magnet Ekleme** → QBittorrent dosya bilgilerini alır
2. **Tracker İletişimi** → Peer listesi istenir
3. **Peer Bağlantısı** → Diğer kullanıcılara bağlanılır
4. **Piece İndirme** → Dosya parçalar halinde indirilir
5. **Hash Doğrulama** → İndirilen parçalar kontrol edilir
6. **Dosya Tamamlama** → Parçalar birleştirilerek dosya oluşur

### Torrent Yaşam Döngüsü

| Aşama | Durum | Açıklama | Süre |
| --- | --- | --- | --- |
| **Metadata** | Downloading Metadata | Torrent bilgileri alınıyor | 1-30 saniye |
| **Queued** | Queued | Sırada bekliyor | Değişken |
| **Downloading** | Downloading | Aktif indirme | Dakikalar-Saatler |
| **Completed** | Completed | İndirme tamamlandı | Anlık |
| **Seeding** | Seeding | Paylaşım yapıyor | Sürekli |

### Dosya Parçalama (Piece System)

```
Büyük Dosya (1 GB)
├── Piece 1 (4 MB) ← Peer A'dan
├── Piece 2 (4 MB) ← Peer B'den
├── Piece 3 (4 MB) ← Peer C'den
├── ...
└── Piece 256 (4 MB) ← Peer Z'den

Her piece SHA-1 hash ile doğrulanır
```

### Ratio Sistemi

| Oran | Açıklama | Anlam |
| --- | --- | --- |
| **< 0.5** | Az paylaşım | Leech durumu |
| **0.5 - 1.0** | Orta paylaşım | Normal kullanım |
| **1.0 - 2.0** | İyi paylaşım | Toplumsal katkı |
| **> 2.0** | Mükemmel paylaşım | Süper seeder |

### 📥 Torrent İndirme

### Torrent Dosyası Ekleme

| Yöntem | Kısayol | Açıklama |
| --- | --- | --- |
| **Dosya Menüsü** | `Ctrl + O` | File → Add Torrent File |
| **Sürükle-Bırak** | - | Torrent dosyasını pencereye sürükle |
| **Çift Tıklama** | - | .torrent dosyasına çift tıkla |

### Magnet Link Ekleme

| Yöntem | Kısayol | Açıklama |
| --- | --- | --- |
| **URL Ekleme** | `Ctrl + Shift + O` | File → Add Torrent Link |
| **Pano İçeriği** | `Ctrl + V` | Magnet linkini otomatik algıla |

### Toplu İndirme

1. **Download from URLs** dialoqunu açın (`Ctrl + Shift + O`)
2. Her satıra bir magnet link/URL ekleyin
3. **Category** ve **Download path** ayarlayın
4. **Download** butonuna tıklayın

### 📊 Transfer Listesi Yönetimi

### Kolonlar ve Sıralama

| Kolon | Açıklama | Faydalı |
| --- | --- | --- |
| **#** | Kuyruk sırası | Öncelik yönetimi |
| **Name** | Torrent adı | Arama ve tanıma |
| **Size** | Toplam boyut | Disk alanı planlaması |
| **Progress** | İndirme ilerlemesi | Durum takibi |
| **Status** | Mevcut durum | Sorun tespiti |
| **Seeds** | Seeder sayısı | Hız tahmini |
| **Peers** | Peer sayısı | Bağlantı durumu |
| **Down Speed** | İndirme hızı | Performans |
| **Up Speed** | Yükleme hızı | Paylaşım |
| **ETA** | Tahmini süre | Planlama |

### Durumlar ve Anlamları

| Durum | Açıklama | Eylem |
| --- | --- | --- |
| **Downloading** | Aktif indirme | Normal |
| **Seeding** | Paylaşım yapıyor | Normal |
| **Paused** | Durakladı | Manuel başlat |
| **Queued** | Kuyrukta bekliyor | Sırayı kontrol et |
| **Checking** | Dosyaları kontrol ediyor | Bekle |
| **Error** | Hata durumu | Sorun çöz |
| **Missing Files** | Dosyalar bulunamıyor | Konum değiştir |

### 🗂️ Kategori Yönetimi

### Kategori Oluşturma

1. Transfer listesinde sağ tık → **New Category**
2. **Kategori adı** girin
3. **Save path** belirleyin (isteğe bağlı)
4. **OK** ile kaydedin

### Otomatik Kategori Yönetimi

| Özellik | Açıklama | Kullanım |
| --- | --- | --- |
| **Auto TMM** | Otomatik Torrent Yönetimi | Kategori bazlı organizasyon |
| **Default Save Path** | Varsayılan kayıt yolu | Kategori özel klasörler |
| **Incomplete Path** | Yarım dosya yolu | Geçici indirme klasörü |

## ⚙️ Gelişmiş Özellikler

### 🔄 Kuyruk Yönetimi

### Kuyruk Ayarları

| Ayar | Varsayılan | Açıklama |
| --- | --- | --- |
| **Max active downloads** | 3 | Eş zamanlı indirme |
| **Max active uploads** | 3 | Eş zamanlı yükleme |
| **Max active torrents** | 5 | Toplam aktif torrent |

### Öncelik Seviyeleri

| Öncelik | Açıklama | Kullanım |
| --- | --- | --- |
| **Maximum** | En yüksek öncelik | Acil dosyalar |
| **High** | Yüksek öncelik | Önemli dosyalar |
| **Normal** | Normal öncelik | Standart kullanım |
| **Low** | Düşük öncelik | Arka plan |
| **Do not download** | İndirme | Gereksiz dosyalar |

### 📡 Tracker Yönetimi

### Tracker Ekleme/Düzenleme

1. Torrent’i seçin → **Trackers** sekmesi
2. Sağ tık → **Add a URL** / **Edit URL**
3. Tracker URL’sini girin
4. **OK** ile kaydedin

### Tracker Durumları

| Durum | Açıklama | Çözüm |
| --- | --- | --- |
| **Working** | Normal çalışıyor | - |
| **Updating** | Güncelleniyor | Bekle |
| **Not contacted yet** | Henüz bağlanmadı | Bekle |
| **Tracker error** | Hata var | URL’yi kontrol et |

### 🎯 Hız Limitleri

### Global Hız Limitleri

1. **Tools** → **Options** → **Speed**
2. Upload/Download limitlerini ayarlayın
3. **Alternative Rate Limits** için zaman programı yapın

| Ayar | Açıklama | Önerilen |
| --- | --- | --- |
| **Global Download Speed** | Toplam indirme hızı | Bandın %80’i |
| **Global Upload Speed** | Toplam yükleme hızı | Bandın %80’i |
| **Alternative Speed** | Alternatif hızlar | Gündüz saatleri |

### Torrent Bazlı Limitler

1. Torrent’i seçin → sağ tık → **Set download limit**
2. Özel hız değeri girin
3. **0** = limitsiz, **1** = global limit kullan

## 📡 RSS Özellikleri

### 🔧 RSS Kurulumu

### RSS Besleme Ekleme

1. **View** → **RSS Reader** (F3)
2. **RSS** sekmesinde **New subscription**
3. RSS URL’sini girin (örn: torrent sitesi RSS’i)
4. **Feed name** verin
5. **OK** ile ekleyin

### RSS Konfigürasyonu

| Ayar | Açıklama | Önerilen |
| --- | --- | --- |
| **Auto downloading** | Otomatik indirme | Kurallara göre |
| **Max articles** | Maksimum makale | 50-100 |
| **Refresh interval** | Yenileme sıklığı | 15-30 dakika |

### 📋 RSS Kuralları

### Otomatik İndirme Kuralı

1. **RSS** → **New rule** (veya F4)
2. **Rule name** girin
3. **Must Contain** alanına anahtar kelimeler ekleyin
4. **Must Not Contain** ile istenmeyen terimleri hariç tutun
5. **Category** ve **Save to** ayarlayın

### Kural Örnekleri

| Kural Tipi | Must Contain | Must Not Contain | Kullanım |
| --- | --- | --- | --- |
| **TV Dizisi** | `ShowName S\d+E\d+` | `cam, ts, screener` | Bölüm takibi |
| **Film Kalitesi** | `1080p, BluRay` | `cam, ts, webrip` | Yüksek kalite |
| **Dil Filtresi** | `turkish, tr` | `dubbed, altyazi` | Dil tercihi |

### Regex Filtreleri

```
# Sezon/bölüm formatı
.*[Ss](\d+)[Ee](\d+).*

# Kalite filtreleri
.*(1080p|720p|BluRay|WEB-DL).*

# Tarih formatı
.*(\d{4}.\d{2}.\d{2}).*
```

### 📈 RSS İzleme

### Feed Durumları

| Durum | Açıklama | Eylem |
| --- | --- | --- |
| **Unread** | Okunmamış makaleler | İncele |
| **Downloading** | İndiriliyor | Bekle |
| **Downloaded** | İndirildi | Arşivle |
| **Error** | Hata | Kuralı kontrol et |

## 🔒 Güvenlik ve Gizlilik

### ⚖️ Yasal ve Etik Kullanım

### BitTorrent’in Yasal Kullanım Alanları

✅ **Açık Kaynak Yazılımlar**
- Linux dağıtımları (Ubuntu, Fedora, etc.)
- Açık kaynak uygulamalar
- Ücretsiz oyunlar ve demo’lar

✅ **Yasal İçerik Dağıtımı**
- Creative Commons lisanslı içerik
- Kendi oluşturduğunuz içerik
- Telif hakkı süresi geçmiş eserler

✅ **Kurumsal Kullanım**
- Yazılım güncellemeleri (Windows Update gibi)
- Büyük dosya dağıtımı
- Backup ve senkronizasyon

### Yasal Riskler ve Sorumlulukar

⚠️ **DİKKAT EDİLMESİ GEREKENLER**:

| Risk | Açıklama | Önlem |
| --- | --- | --- |
| **Telif Hakkı İhlali** | Korumalı içerik indirme | Sadece yasal içerik kullan |
| **ISP Uyarıları** | İnternet sağlayıcı bildirimi | VPN kullan |
| **Hukuki Süreç** | Dava açılması | Yasal sınırlarda kal |
| **Malware Riski** | Zararlı dosyalar | Antivirus kullan |

### Güvenli Torrent Kullanım Kuralları

1. **Kaynağı Doğrula**: Sadece güvenilir sitelerden indir
2. **Dosyaları Tara**: İndirdiğin dosyaları antivirüs ile tara
3. **IP’ni Gizle**: VPN veya proxy kullan
4. **Ratio’yu Koru**: Paylaşım yap ama sınırlarda
5. **Özel Tracker’lar**: Kapalı topluluk tracker’larını tercih et

### 🛡️ Temel Güvenlik

### Kimlik Gizleme

| Özellik | Açıklama | Önerilen |
| --- | --- | --- |
| **Anonymous Mode** | Anonim mod | ✅ Etkin |
| **Hide Client** | Client gizleme | ✅ Etkin |
| **Encrypt Headers** | Başlık şifreleme | ✅ Etkin |

### IP Filtreleme

1. **Tools** → **Options** → **Connection** → **IP Filtering**
2. **Filter path** ile IP engelleme listesi ekleyin
3. Listeleri düzenli güncelleyin

### Yaygın IP Filter Listeleri

| Liste | Kaynak | Açıklama |
| --- | --- | --- |
| **PeerGuardian** | phoenixlabs.org | Kapsamlı liste |
| **BlueTack** | bluetack.co.uk | Güvenlik odaklı |
| **IBlocklist** | iblocklist.com | Güncel listeler |

### 🔐 Proxy ve VPN

### SOCKS5 Proxy Kurulumu

1. **Tools** → **Options** → **Connection** → **Proxy Server**
2. **Type**: SOCKS5
3. **Host** ve **Port** bilgilerini girin
4. **Authentication** gerekirse aktifleştirin
5. **Use proxy for peer connections** seçin

### VPN Ayarları

| Ayar | Açıklama | Güvenlik |
| --- | --- | --- |
| **Bind to interface** | Ağ arayüzü bağlama | Yüksek |
| **Force proxy** | Zorunlu proxy | En yüksek |
| **DNS leak protection** | DNS sızıntı koruması | Kritik |

### VPN Kill Switch

1. **Advanced** → **Network Interface** bölümüne gidin
2. VPN ağ arayüzünü seçin (örn: tun0, wg0)
3. VPN kesilirse tüm torrent trafiği durur

### 🚨 Güvenlik Uyarıları

⚠️ **DİKKAT EDİLMESİ GEREKENLER**:

| Risk | Açıklama | Önlem |
| --- | --- | --- |
| **IP Sızıntısı** | Gerçek IP’nin görünmesi | VPN bind, kill switch |
| **DNS Sızıntısı** | DNS sorgularının sızması | Özel DNS sunucuları |
| **WebRTC Sızıntısı** | Tarayıcı IP sızıntısı | WebRTC devre dışı |
| **Tracker Sızıntısı** | Tracker’lara IP sızıntısı | Force proxy |

## ❓ SSS ve Sorun Giderme

### 🔧 Yaygın Sorunlar

### İndirme Hızı Problemleri

| Sorun | Olası Nedenler | Çözümler |
| --- | --- | --- |
| **Yavaş İndirme** | Az seeder, yanlış ayarlar | • Daha fazla seeder’lı torrent seç• Port ayarlarını kontrol et• Hız limitlerini kaldır |
| **Hiç İndirmiyor** | Firewall, proxy sorunu | • Port 6881-6889’u aç• UPnP’yi etkinleştir• Proxy ayarlarını kontrol et |
| **Kesilme** | Ağ bağlantısı, tracker sorunu | • İnternet bağlantısını test et• Tracker’ları güncelle• DHT’yi etkinleştir |

### Bağlantı Sorunları

| Hata Mesajı | Anlamı | Çözüm |
| --- | --- | --- |
| **“Firewalled”** | Port kapalı | UPnP etkinleştir veya manuel port aç |
| **“Tracker Error”** | Tracker’a erişilemiyor | URL’yi kontrol et, alternatif tracker ekle |
| **“Permission Denied”** | Dosya izin sorunu | Klasör izinlerini kontrol et |

### Dosya Sistemı Sorunları

| Sorun | Açıklama | Çözüm |
| --- | --- | --- |
| **Missing Files** | Dosyalar bulunamıyor | • Dosya konumunu değiştir• Torrent’i yeniden kontrol et |
| **Access Denied** | Yazma izni yok | • Klasör izinlerini düzenle• Yönetici olarak çalıştır |
| **Disk Full** | Disk alanı doldu | • Gereksiz dosyaları sil• Farklı diske taşı |

### 📋 Tanılama Adımları

### Bağlantı Testi

1. **Help** → **About** → kütüphane versiyonlarını kontrol et
2. **Tools** → **Options** → **Connection** → **Test Port**
3. Port durumunu gözlemle

### Log İnceleme

1. **View** → **Log** (F2)
2. Hata mesajlarını incele
3. **Tools** → **Options** → **Advanced** → loglama seviyesini artır

### Ağ Tanılaması

```bash
# Port kontrolü (Windows)
netstat -an | findstr :6881

# Port kontrolü (Linux)
netstat -tuln | grep 6881

# Bağlantı testi
telnet tracker-url.com 80
```

### 🔄 Resetleme

### Temiz Kurulum

1. QBittorrent’i kapat
2. Ayar klasörünü yedekle
3. Ayar klasörünü sil
4. QBittorrent’i başlat (varsayılan ayarlarla)
5. Gerekirse yedekten ayarları geri yükle

## 💡 İpuçları ve Püf Noktaları

### ⚡ Hız Artırma İpuçları

### En İyi Pratikler

| İpucu | Açıklama | Fayda |
| --- | --- | --- |
| **Popüler Torrent Seç** | Çok seeder’lı torrentler | Yüksek hız garantisi |
| **Peak Saatlerde İndir** | Akşam saatleri | Daha fazla aktif peer |
| **Upload Yap** | Paylaştığın kadar al | Daha iyi ratio |
| **Port Forward** | Manuel port açma | Daha iyi bağlantı |

### Optimum Ayarlar

| Kullanım Tipi | Global Download | Global Upload | Connections |
| --- | --- | --- | --- |
| **Ev Kullanıcısı** | Bandın %80’i | Bandın %20’si | 100-200 |
| **Paylaşım Odaklı** | Bandın %50’si | Bandın %80’i | 300-500 |
| **Sunucu** | Sınırsız | Sınırsız | 1000+ |

### 📁 Dosya Organizasyonu

### Akıllı Kategori Kullanımı

| Kategori | Save Path | Kullanım |
| --- | --- | --- |
| **Movies** | `D:\Downloads\Movies` | Film indirmeleri |
| **TV Shows** | `D:\Downloads\TV` | Dizi indirmeleri |
| **Software** | `D:\Downloads\Apps` | Yazılım indirmeleri |
| **Books** | `D:\Downloads\Books` | E-kitap indirmeleri |
| **Music** | `D:\Downloads\Music` | Müzik indirmeleri |

### Otomatik Sıralama

1. **Category defaults** her kategori için ayarlayın
2. **Auto TMM** (Automatic Torrent Management) etkinleştirin
3. **Content layout** olarak “Create subfolder” seçin

### 🤖 Otomasyon İpuçları

### RSS Otomasyonu

```bash
# TV Dizisi için örnek kural
Must Contain: Breaking.Bad.S\d+E\d+.1080p
Must Not Contain: HDCAM, TS, WEBRIP
Category: TV Shows
Save to: D:\Downloads\TV\Breaking Bad\
```

### Toplu İşlemler

| İşlem | Kısayol | Kullanım |
| --- | --- | --- |
| **Tümünü Durdur** | `Ctrl + A` → `Space` | Hızlı duraklama |
| **Kategori Değiştir** | `Seçim` → `Sağ Tık` → `Category` | Toplu organizasyon |
| **Öncelik Ayarla** | `Seçim` → `Sağ Tık` → `Priority` | Kuyruk yönetimi |

## 📖 Torrent Terminoloji Sözlüğü

### 🔤 Temel Terimler

| Terim | Açıklama | Kullanım |
| --- | --- | --- |
| **BitTorrent** | P2P dosya paylaşım protokolü | Ana teknoloji |
| **Client** | Torrent programı (QBittorrent gibi) | Yazılım |
| **Torrent Dosyası** | .torrent uzantılı meta dosya | İndirme başlatma |
| **Magnet Link** | Torrent bilgisinin URL formatı | Kolay paylaşım |
| **Hash** | Dosyanın benzersiz kimliği | Doğrulama |
| **Piece** | Dosyanın küçük parçası | İndirme birimi |

### 👥 Kullanıcı Tipleri

| Terim | Açıklama | Davranış |
| --- | --- | --- |
| **Seeder** | Dosyanın tamamına sahip kişi | Upload yapar |
| **Leecher** | Dosyayı indiren kişi | Download yapar |
| **Peer** | Ağdaki herhangi bir kullanıcı | Her iki davranış |
| **Snatcher** | İndirip kaçan kullanıcı | Sadece download |

### 🌐 Ağ Terimleri

| Terim | Açıklama | İşlev |
| --- | --- | --- |
| **Tracker** | Peer’ları buluşturan sunucu | Koordinasyon |
| **DHT** | Dağıtık Hash Tablosu | Tracker’sız peer bulma |
| **PEX** | Peer Exchange | Peer’lar arası bilgi paylaşımı |
| **LSD** | Local Service Discovery | Yerel ağda peer bulma |
| **Swarm** | Aynı torrent’teki tüm peer’lar | Topluluk |

### 📊 Performans Terimleri

| Terim | Açıklama | Birim |
| --- | --- | --- |
| **Ratio** | Upload/Download oranı | Sayısal oran |
| **Availability** | Dosyanın ağdaki mevcudiyeti | 0.0 - X.X |
| **ETA** | Estimated Time of Arrival | Zaman |
| **Seeds** | Seeder sayısı | Sayı |
| **Peers** | Aktif peer sayısı | Sayı |
| **Speed** | Transfer hızı | KB/s, MB/s |

### ⚙️ Teknik Terimler

| Terim | Açıklama | Kullanım |
| --- | --- | --- |
| **UPnP** | Universal Plug and Play | Port açma |
| **NAT-PMP** | NAT Port Mapping Protocol | Port yönlendirme |
| **Encryption** | Veri şifreleme | Güvenlik |
| **Proxy** | Aracı sunucu | Gizlilik |
| **VPN** | Virtual Private Network | Anonimlik |
| **Kill Switch** | VPN kopunca internet kesme | Güvenlik |

### 🏷️ Durum Terimleri

| QBittorrent Durumu | Açıklama | Renk Kodu |
| --- | --- | --- |
| **Downloading** | Aktif indirme | Yeşil |
| **Seeding** | Paylaşım | Mavi |
| **Paused** | Durakladı | Gri |
| **Queued** | Kuyrukta | Turuncu |
| **Checking** | Dosya kontrolü | Sarı |
| **Error** | Hata durumu | Kırmızı |
| **Missing Files** | Dosyalar yok | Mor |
| **Moving** | Taşınıyor | Açık mavi |

### 📁 Dosya Sistemi

| Terim | Açıklama | Örnek |
| --- | --- | --- |
| **Save Path** | Ana kayıt klasörü | `D:\Downloads` |
| **Incomplete Path** | Yarım dosya klasörü | `D:\Downloads\.incomplete` |
| **Category Path** | Kategori klasörü | `D:\Downloads\Movies` |
| **Content Layout** | Dosya düzeni | Subfolder/No subfolder |

### 🔧 Gelişmiş Terimler

| Terim | Açıklama | Kullanım |
| --- | --- | --- |
| **Sequential Download** | Sıralı indirme | Video önizleme |
| **Force Reannounce** | Zorla tracker güncelleme | Bağlantı sorunu |
| **Force Recheck** | Zorla dosya kontrolü | Dosya bütünlüğü |
| **Super Seeding** | Verimli paylaşım modu | Seed optimizasyonu |
| **Anonymous Mode** | Anonim mod | Gizlilik |