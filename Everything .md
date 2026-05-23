# 🛠️ Everything

> **Kısa Açıklama:** Windows'ta dosya ve klasör adlarına göre anlık arama yapan hafif ve hızlı arama aracı.

Güncel · Windows · Ücretsiz · Sistem Araçları

---

## 📌 Genel Bakış

Everything, Windows'un yerleşik aramasına kıyasla dosya adlarını neredeyse anında bulan bir arama motorudur. NTFS birimlerinde dosya adı indeksi tutar; yazdıkça sonuçlar gerçek zamanlı güncellenir. İçerik araması yapmaz - dosya adı ve meta veri odaklıdır. Reklamsız ve düşük bellek kullanır.

---

## ✨ Öne Çıkan Özellikler

- **Anlık arama** - Yazarken sonuçlar görünür
- **Düşük kaynak** - Az RAM ve disk kullanımı
- **NTFS entegrasyonu** - Dosya değişikliklerini otomatik izler
- **Gelişmiş sorgular** - Joker (`*`, `?`), OR (`|`), NOT (`!`)
- **Filtreler** - Ses, video, resim, doküman grupları
- **Ücretsiz** - Reklam veya spyware içermez

---

## 📥 İndirme ve Kurulum

### Yöntem 1: Resmi Site ( Önerilen )

1. [voidtools.com](https://www.voidtools.com/) adresine git
2. **Download** → **x64 Installer** (veya sisteme uygun sürüm) indir
3. Kurulum sihirbazını takip et
4. İsteğe bağlı: **Lite** sürüm - ETP/FTP/HTTP sunucu özellikleri olmadan daha sade kurulum

> Normal sürüm çoğu kullanıcı için uygundur; yalnızca arama istiyorsan Lite yeterli olabilir.

### Yöntem 2: WinGet (Terminal)

```powershell
winget install voidtools.Everything
```

### Yöntem 3: UniGetUI

> UniGetUI açıkken arama çubuğuna **Everything** yaz ve kur.

### Yöntem 4: Chocolatey

```powershell
choco install everything
```

---

## ⚙️ İlk Kurulum ve Önerilen Ayarlar

Ayarlar: **Araçlar → Seçenekler** (veya `Ctrl+P`)

1. **Everything Service:** Genel → **Everything Service** işaretle; **Run as administrator** kapalı bırak - UAC uyarısı azalır, NTFS indekslemesi sürekli çalışır.
2. **Arayüz:** Genel → **Arayüz** → **Arka planda çalıştır**, **Tepsi simgesi göster** ve **Tepsi simgesine tek tıklamayla aç** açık kalsın.
3. **Kısayol tuşu:** Genel → **Klavye** → hızlı açma kısayolunu tanımla (ör. `Ctrl+Alt+E`).

> 💡 **İpucu:** NTFS dışı (FAT32, exFAT) veya ağ sürücüleri için **İndeksler → Klasörler → Ekle** ile manuel ekleme gerekir.

---

## 📋 Seçenekler - Son Kullanıcı İçin Önemli Ayarlar

Sol menüdeki kategorilerden günlük kullanımda işine yarayanlar:

### Genel → Arayüz

- **Yazdığım gibi ara** - Yazdıkça anında sonuç (varsayılan açık)
- **Arka planda çalıştır** - Kapatınca tepsi simgesinde kalır
- **Tepsi simgesine tek tıklamayla aç** - Bildirim alanından hızlı erişim

### Genel → Arama

- **Hızlı ASCII araması** - Standart karakterlerde daha hızlı arama
- **Yol ayıracı içerdiğinde yolu eşleştir** - `downloads\` gibi klasör yolu aramaları
- **Jokerlerde bütün dosya adını eşleştir** - `*` ve `?` ile tam eşleşme
- **İşletici üstünlüğü** - `OR > AND` (birden fazla kelimede mantık sırası)

### Genel → Sonuçlar

- **Yeniden adlandırırken uzantıyı seçme** - `.pdf` uzantısını yanlışlıkla silmeyi önler
- **Tarihi / boyutu büyükten küçüğe sırala** - En yeni veya en büyük dosyalar üstte

### Genel → Görünüm

- **Vurgulanan arama terimlerini göster** - Eşleşen kısımlar vurgulanır
- **Araç ipuçlarını göster** - Fare ile üzerine gelince bilgi

### Genel → Bağlam Menüsü

- Sağ tık menüsünden **Adı / Yolu / Tam adı panoya kopyala** - Dosya yolunu hızlı paylaş

### İndeksler

- **NTFS** - Sabit diskler otomatik dahil; **Değişiklikleri izle** açık kalsın
- **Klasörler** - NTFS olmayan veya ağ klasörlerini manuel ekle
- **Dışında Tutma** - Temp, `$Recycle.Bin` gibi klasörleri aramadan hariç tut
- **Yeniden Oluşturmaya Zorla** - İndeks bozulursa sıfırdan tara

> ETP/FTP ve HTTP Sunucusu gelişmiş özelliklerdir; yalnızca ağ üzerinden erişim gerekiyorsa kullan. Lite sürümde bu seçenekler yoktur.

---

## 🚀 Temel Kullanım

### Hızlı arama

1. Everything'i aç
2. Arama kutusuna yaz - sonuçlar anında listelenir
3. Dosyaya çift tıkla veya Enter ile aç

### Sık kullanılan sorgular

| Sorgu | Sonuç |
| ----- | ----- |
| `rapor` | Adında "rapor" geçen dosyalar |
| `*.pdf` | Tüm PDF dosyaları |
| `*.jpg \| *.png` | JPG veya PNG dosyaları |
| `downloads\ *.mp3` | Downloads klasöründeki MP3'ler |
| `size:>1GB` | 1 GB'dan büyük dosyalar |

> `content:kelime` ile dosya içeriği aranabilir; indekslenmediği için yavaştır.

---

## ⚠️ Bilinen Sorunlar ve Çözümleri


| Sorun | Neden Olur | Çözüm |
| ----- | ---------- | ----- |
| Sonuç yok / eksik | NTFS indekslenmemiş | Everything Service açık mı kontrol et; sürücü NTFS mi bak |
| UAC uyarısı | Yönetici modu | Service kullan; "Run as administrator" kapat |
| Ağ sürücüsü görünmüyor | Manuel ekleme gerekir | Seçenekler → İndeksler → Klasörler → Ekle |
| FAT32 disk yok | Otomatik indeks yok | Seçenekler → İndeksler → Klasörler ile ekle |
| İndeks güncel değil | USN veya servis sorunu | Seçenekler → İndeksler → **Yeniden Oluşturmaya Zorla** |


---

## 🔗 Faydalı Bağlantılar

- 🌐 [Resmi Web Sitesi](https://www.voidtools.com/)
- 📖 [Arama Sözdizimi (FAQ)](https://www.voidtools.com/support/everything/searching/)
- 🔧 [Everything Toolbar (isteğe bağlı)](https://github.com/srwi/EverythingToolbar) - Görev çubuğundan arama

---

## 📝 Notlar

> Everything yalnızca **dosya adı** indeksler; Windows Search gibi e-posta veya belge içeriği taramaz - bu yüzden çok hızlıdır. Görev çubuğu entegrasyonu isteyenler [Everything Toolbar](https://github.com/srwi/EverythingToolbar) eklentisine bakabilir (ayrı kurulum).

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
