# 🛠️ Bulk Crap Uninstaller (BCU)

> **Kısa Açıklama:** Çok sayıda programı toplu kaldırır; artık dosya ve kayıt defteri kalıntılarını temizler.

6.1 · Windows 10/11 · Apache 2.0 / ücretsiz · Sistem Araçları

---

## 📌 Genel Bakış

Bulk Crap Uninstaller (BCU), Windows'un yerleşik kaldırıcısının ötesinde gizli, taşınabilir, Steam, UWP ve Chocolatey paketlerini de algılar. Önce programın kendi kaldırıcısını çalıştırır; ardından artıkları tarar. Bloatware temizliği veya format öncesi toplu kaldırma için idealdir; tamamen ücretsiz ve açık kaynaktır.

---

## ✨ Öne Çıkan Özellikler

- **Toplu kaldırma** - Birden fazla uygulamayı tek seferde sil
- **Geniş algılama** - Normal, gizli, portable, UWP, Steam, Windows Update
- **Artık temizliği** - Kaldırma sonrası dosya ve kayıt defteri taraması
- **Zorla kaldırma** - Bozuk veya kaldırıcısı olmayan programlar
- **Başlangıç yöneticisi** - Otomatik başlayan uygulamaları yönet
- **Taşınabilir sürüm** - USB'den çalıştırılabilir

---

## 📥 İndirme ve Kurulum

### Yöntem 1: SourceForge - Önerilen

1. [SourceForge proje sayfasına](https://sourceforge.net/projects/bulk-crap-uninstaller/) git
2. **Download** ile en güncel sürümü indir
3. **Setup** (normal kurulum) veya **Portable** (taşınabilir) dosyasını çalıştır

> **Setup:** .NET 8 gerekirse otomatik kurulur. **Portable:** .NET dahil, dosya boyutu daha büyük.

### Yöntem 2: Resmi Site

1. [bcuninstaller.com](https://www.bcuninstaller.com/) adresine git
2. İndirme bağlantısından sürümü seç ve kur

### Yöntem 3: WinGet (Terminal)

```powershell
winget install Klocman.BulkCrapUninstaller
```

### Yöntem 4: UniGetUI

> UniGetUI açıkken arama çubuğuna **Bulk Crap Uninstaller** yaz ve kur.

Alternatif: [GitHub Releases](https://github.com/Klocman/Bulk-Crap-Uninstaller/releases)

---

## ⚙️ İlk Kurulum ve Önerilen Ayarlar

1. **İlk tarama:** Uygulamayı aç; yüklü program listesi otomatik yüklenir
2. **Yedek:** Ayarlardan kaldırma öncesi **Sistem Geri Yükleme Noktası** oluşturmayı aç
3. **Filtre:** Gereksiz sistem bileşenlerini yanlışlıkla silmemek için filtre kullan

> 💡 Kaldırmadan önce program adını ve yayıncısını kontrol et; bilinmeyen girişleri araştır.

---

## 🚀 Temel Kullanım

### Tek program kaldırma

1. Listeden programı seç
2. **Uninstall** (Kaldır) butonuna tıkla
3. Orijinal kaldırıcı çalışır → artık taraması sorulur → onayla

### Toplu kaldırma

1. Birden fazla program seç
2. **Uninstall** → toplu kaldırma başlar
3. Sessiz kaldırma destekleyen programlar otomatik işlenir

### Artık temizliği

1. Zaten kaldırılmış bir programın kalıntıları varsa listede ara
2. Kaldırma sonrası **Leftovers** (artıklar) ekranında işaretle
3. Silmeden önce listeyi gözden geçir

---

## ⚠️ Bilinen Sorunlar ve Çözümleri


| Sorun                  | Neden Olur                | Çözüm                                                                                           |
| ---------------------- | ------------------------- | ----------------------------------------------------------------------------------------------- |
| .NET hatası            | Runtime eksik             | [.NET 8 Desktop Runtime](https://dotnet.microsoft.com/download) kur veya Portable sürümü kullan |
| Program silinmiyor     | Edge gibi sistem bileşeni | Windows'un entegre uygulamaları zor kaldırılır; dikkatli ol                                     |
| Yanlış program silindi | Toplu seçim hatası        | Geri yükleme noktasından geri dön                                                               |
| Liste çok uzun         | Çok sayıda algılama       | Filtre ve arama kullan; gizli korumalıları ayrı incele                                          |
| Kaldırıcı takılıyor    | Bozuk uninstaller         | BCU çöken kaldırıcıları yönetir; gerekirse Force Uninstall                                      |


---

## 🔗 Faydalı Bağlantılar

- 📦 [SourceForge (İndirme)](https://sourceforge.net/projects/bulk-crap-uninstaller/)
- 🌐 [Resmi Web Sitesi](https://www.bcuninstaller.com/)
- 💾 [GitHub Sayfası](https://github.com/Klocman/Bulk-Crap-Uninstaller)
- 📖 [Çevrimiçi Kılavuz](https://github.com/Klocman/Bulk-Crap-Uninstaller/wiki)

---

## 📝 Notlar

> BCU güçlü bir araçtır; kayıt defteri ve sistem dosyalarına müdahale eder. Kritik Windows bileşenlerini kaldırmaktan kaçın. [Revo-vs-Bulk-Crap-Uninstaller.md](Revo-vs-Bulk-Crap-Uninstaller.md) dosyasında Revo ile karşılaştırmaya bakabilirsin - toplu kaldırma ve ücretsiz kullanım için BCU genelde tercih edilir.

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
