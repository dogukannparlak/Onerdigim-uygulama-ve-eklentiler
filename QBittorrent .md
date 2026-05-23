# 🛠️ qBittorrent

> **Kısa Açıklama:** Reklamsız, açık kaynak BitTorrent istemcisi; torrent ve magnet linkleriyle dosya indirmeni sağlar.

Güncel · Windows 10/11 · Ücretsiz / açık kaynak · İndirme

---

## 📌 Genel Bakış

qBittorrent, dosyaları merkezi sunucudan değil diğer kullanıcılardan (P2P) parçalar halinde indiren BitTorrent protokolünü kullanan bir istemcidir. `.torrent` dosyası veya magnet link ile indirme başlatılır. µTorrent'e reklamsız alternatif olarak bilinir; Web arayüzü, arama ve RSS desteği sunar.

---

## ✨ Öne Çıkan Özellikler

- **Reklamsız ve ücretsiz** - Spyware veya gizli yazılım yok
- **Magnet desteği** - Link yapıştırarak hızlı indirme
- **RSS otomasyonu** - Kurallara göre otomatik indirme
- **Platformlar arası** - Windows, Linux, macOS

---

## 📥 İndirme ve Kurulum

### Yöntem 1: Resmi Site ( Önerilen )

1. [qbittorrent.org/download](https://www.qbittorrent.org/download) adresine git
2. Windows sürümünü indir
3. Kurulum sihirbazını takip et

### Yöntem 2: WinGet (Terminal)

```powershell
winget install qBittorrent.qBittorrent
```

### Yöntem 3: UniGetUI

> UniGetUI açıkken arama çubuğuna **qBittorrent** yaz ve kur.

---

## ⚙️ İlk Kurulum ve Önerilen Ayarlar

1. **Dil:** Araçlar → Seçenekler → Davranış → Arayüz dili → **Türkçe**
2. **İndirme klasörü:** Araçlar → Seçenekler → İndirmeler → Varsayılan kayıt yolu

> 💡 İndirme tamamlandıktan sonra paylaşım (seeding) devam eder; bant genişliğini tüketmemesi için hız limiti veya otomatik durdurma ayarla.

---

## 🚀 Temel Kullanım

### Torrent ekleme

1. `.torrent` dosyasını qBittorrent penceresine **sürükle-bırak**
2. Veya **Ctrl + O** → torrent dosyasını seç
3. İndirme konumunu onayla → **Tamam**

### Magnet link ekleme

1. Magnet linkini kopyala
2. **Ctrl + Shift + O** → linki yapıştır
3. Veya qBittorrent açıkken **Ctrl + V** (pano otomatik algılanır)

### Klavye kısayolları


| Kısayol            | İşlev                   |
| ------------------ | ----------------------- |
| `Ctrl + O`         | Torrent dosyası ekle    |
| `Ctrl + Shift + O` | Magnet / URL ekle       |
| `Ctrl + P`         | Duraklat / devam et     |
| `Delete`           | Seçili torrent'i kaldır |
| `F3`               | RSS okuyucu             |


---

## ⚠️ Bilinen Sorunlar ve Çözümleri


| Sorun                      | Neden Olur              | Çözüm                                                      |
| -------------------------- | ----------------------- | ---------------------------------------------------------- |
| İndirme yavaş              | Az seeder / port kapalı | UPnP açık mı kontrol et; farklı torrent dene               |
| Metadata bekliyor          | Magnet henüz eşleşmedi  | Birkaç dakika bekle; DHT etkin olsun                       |
| Port kapalı (turuncu ikon) | Router / firewall       | Araçlar → Seçenekler → Bağlantı → UPnP/NAT-PMP etkinleştir |
| Dosya bulunamıyor          | Taşınmış veya silinmiş  | Sağ tık → Konumu belirt                                    |
| Disk dolu                  | Hedef sürücü dolu       | İndirme klasörünü değiştir veya yer aç                     |


---

## 🔗 Faydalı Bağlantılar

- 🌐 [Resmi Web Sitesi](https://www.qbittorrent.org/)
- 💾 [GitHub Sayfası](https://github.com/qbittorrent/qBittorrent)
- 📖 [Wiki / SSS](https://github.com/qbittorrent/qBittorrent/wiki)

---

## 📝 Notlar

> BitTorrent yasal içerikler (Linux ISO, açık kaynak yazılımlar vb.) için kullanılabilir; telif hakkı ihlali yasal sorumluluk doğurur. P2P ağında IP adresin görünür - VPN kullanımı gizlilik tercihinize bağlıdır. Yalnızca güvendiğin kaynaklardan torrent indir.

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

*Son güncelleme: 2026-05-22*
