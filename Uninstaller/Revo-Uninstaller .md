# 🛠️ Revo Uninstaller

> **Kısa Açıklama:** Programları kaldırırken artık dosya ve kayıt defteri girdilerini tarayıp temizler; Windows kaldırıcısının bıraktığı kalıntıları giderir.

Free / Pro · Windows 10/11 · Freeware / ücretli · Sistem Araçları

---

## 📌 Genel Bakış

Revo Uninstaller, önce programın kendi kaldırıcısını çalıştırır, ardından sistemde kalan dosya ve kayıt defteri artıklarını tarar. Windows'un "Program Ekle/Kaldır" bölümü yalnızca ana kaydı siler; Revo derinlemesine temizlik sunar. **Free** sürümü çoğu kullanıcı için yeterlidir; **Pro** zorla kaldırma, toplu silme ve gerçek zamanlı kurulum izleme ekler.

---

## ✨ Öne Çıkan Özellikler

- **Derin tarama** — Kaldırma sonrası artık dosya ve registry temizliği
- **Hunter Mode** — Simge veya pencereye sürükleyerek program bul ve kaldır
- **Windows UWP** — Mağaza uygulamalarını ayrı listeden yönet
- **Yedekleme** — Kaldırma öncesi otomatik geri yükleme noktası
- **Ek araçlar (Free)** — Başlangıç yöneticisi, geçici dosya ve tarayıcı temizliği
- **Pro ekstraları** — Zorla kaldırma, toplu kaldırma, kurulum monitörü, Logs Database

---

## 📥 İndirme ve Kurulum

### Yöntem 1: Resmi Site — Önerilen

1. [revouninstaller.com](https://www.revouninstaller.com/) adresine git
2. **Revo Uninstaller Free** veya **Pro** indir (30 gün Pro denemesi mevcut)
3. Kurulum sihirbazını takip et — istenmeyen ek yazılım tekliflerine dikkat et

### Yöntem 2: WinGet (Terminal) — Free

```powershell
winget install RevoUninstaller.RevoUninstaller
```

> WinGet genelde Free sürümünü kurar. Pro için resmi siteden lisans satın al.

### Yöntem 3: UniGetUI

> UniGetUI açıkken arama çubuğuna **Revo Uninstaller** yaz ve kur.

---

## ⚙️ İlk Kurulum ve Önerilen Ayarlar

1. **Yedekleme açık kalsın:** Ayarlar → kaldırma öncesi **Sistem Geri Yükleme Noktası** oluştur
2. **Tarama modu:** Varsayılan **Orta** tarama çoğu program için yeterli; **Gelişmiş** yalnızca inatçı kalıntılar için
3. **Hunter Mode:** Sistem tepsisindeki veya masaüstündeki bilinmeyen programlar için kullan
4. **Free vs Pro:** Günlük kullanımda Free yeterli; zorla kaldırma veya toplu silme gerekiyorsa Pro düşün

> 💡 Modern 64-bit Windows'ta Free sürümün 64-bit program desteği sınırlı olabilir; sorun yaşarsan Pro veya [BCU](Bulk-Crap-Uninstaller%20.md) alternatifine bak.

---

## 🚀 Temel Kullanım

### Normal kaldırma

1. Revo'yu aç → listeden programı seç
2. **Uninstall** → programın kendi kaldırıcısı çalışır
3. Tarama modunu seç (Güvenli / Orta / Gelişmiş)
4. Bulunan artıkları incele → **Delete** ile temizle

### Hunter Mode

1. Ana pencerede **Hunter Mode** ikonuna tıkla (hedef simgesi)
2. Kaldırmak istediğin program simgesine veya penceresine sürükle
3. Menüden **Uninstall** seç

### Free vs Pro — hızlı karşılaştırma

| Özellik | Free | Pro |
| ------- | ---- | --- |
| Artık tarama | Evet | Evet |
| Hunter Mode | Evet | Evet |
| Zorla kaldırma | Hayır | Evet |
| Toplu kaldırma | Hayır | Evet |
| Kurulum monitörü | Hayır | Evet |
| Logs Database | Hayır | Evet |

---

## ⚠️ Bilinen Sorunlar ve Çözümleri

| Sorun | Neden Olur | Çözüm |
| ----- | ---------- | ----- |
| Sistem bozuldu | Kritik registry silindi | Geri yükleme noktasından dön; Gelişmiş taramada dikkatli ol |
| 64-bit program kaldırılamıyor | Free sürüm sınırı | Pro kullan veya BCU dene |
| WinGet eski sürüm | Paket gecikmesi | [revouninstaller.com](https://www.revouninstaller.com/) üzerinden güncel sürüm indir |
| Kurulumda ek yazılım | Installer bundle | Önerilen yazılımları reddet; özelleştirilmiş kurulum seç |
| Program listede yok | Bozuk kayıt | Pro **Forced Uninstall** veya BCU **Force Uninstall** |

---

## 🔗 Faydalı Bağlantılar

- 🌐 [Resmi Web Sitesi](https://www.revouninstaller.com/)
- 📥 [Free İndirme](https://www.revouninstaller.com/free-download/)
- 📖 [Nasıl Yapılır Rehberleri](https://www.revouninstaller.com/support/how-to-guides/)
- ❓ [SSS](https://www.revouninstaller.com/support/faq/)

---

## 📝 Notlar

> Revo kayıt defterine müdahale eder; "Gelişmiş" taramada bilmediğin girdileri silme. Free sürüm temel temizlik ve Hunter Mode için iyidir; onlarca program toplu silmek için [Bulk Crap Uninstaller](Bulk-Crap-Uninstaller%20.md) daha uygun olabilir.

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
