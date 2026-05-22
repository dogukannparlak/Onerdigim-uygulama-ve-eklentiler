# 🛠️ UniGetUI

> **Kısa Açıklama:** WinGet, Chocolatey, Scoop ve diğer paket yöneticilerini tek grafik arayüzden kurman, güncellemen ve kaldırmanı sağlar.

Güncel · Windows 10/11 · Ücretsiz / açık kaynak · Sistem Araçları

---

## 📌 Genel Bakış

UniGetUI (eski adı WingetUI), Windows'ta komut satırı bilgisi gerektirmeden yazılım kurulumu ve güncellemesi yapmanı sağlar. WinGet, Chocolatey, Scoop, pip, npm ve .NET Tool paketlerini tek yerden yönetir. Bu repodaki diğer uygulama rehberlerinde geçen "UniGetUI ile kur" yöntemi bu aracı kullanır.

---

## ✨ Öne Çıkan Özellikler

- **Tek arayüz** — Birden fazla paket yöneticisini birleştirir
- **Arama ve keşif** — Paket adı veya açıklama ile ara
- **Toplu işlem** — Birden fazla paketi aynı anda kur, güncelle veya kaldır
- **Otomatik güncelleme** — Güncelleme bildirimi ve zamanlanmış kontrol
- **Export/Import** — Paket listesini yedekle ve başka PC'ye aktar
- **Türkçe dil desteği** — 30+ dil arasında Türkçe mevcut

---

## 📥 İndirme ve Kurulum

### Yöntem 1: Microsoft Store — Önerilen

1. Microsoft Store'u aç
2. **UniGetUI** ara (yayıncı: Devolutions)
3. **Al** veya **Yükle** butonuna tıkla

> Otomatik güncelleme için Store sürümü tercih edilir.

### Yöntem 2: WinGet (Terminal)

```powershell
winget install --exact --id Devolutions.UniGetUI
```

> Eski paket adı `MartiCliment.UniGetUI` artık geçerli değil; `Devolutions.UniGetUI` kullan.

### Yöntem 3: GitHub Release

1. [GitHub Releases](https://github.com/Devolutions/UniGetUI/releases) sayfasına git
2. `UniGetUI.Installer.exe` indir
3. Yönetici olarak çalıştır

---

## ⚙️ İlk Kurulum ve Önerilen Ayarlar

1. **Yönetici izni:** İlk açılışta UAC onayını ver
2. **Dil:** Ayarlar → Dil → **Türkçe** seç
3. **Winget kontrolü:** Ana ekranda Winget'in algılandığını doğrula; algılanmıyorsa [App Installer](https://apps.microsoft.com/detail/9NBLGGH4NNS1) güncelle
4. **Güncelleme kontrolü:** Ayarlar → otomatik güncelleme bildirimini aç

> 💡 Çoğu kullanıcı yalnızca WinGet yeterli; Chocolatey ve Scoop isteğe bağlı ek paket kaynaklarıdır.

---

## 🚀 Temel Kullanım

### Paket kurma

1. UniGetUI'yi aç
2. Arama çubuğuna uygulama adını yaz (ör. **Everything**, **VLC**)
3. Paketi seç → **Yükle** / **Install**
4. Kurulum tamamlanınca listede görünür

### Paket güncelleme ve kaldırma

1. Sol menüden **Güncellemeler** veya **Yüklü paketler** sekmesine git
2. Güncellenecek paketleri seç → **Güncelle**
3. Kaldırmak için pakete sağ tık → **Kaldır**

### Klavye kısayolları

| Kısayol | İşlev |
| ------- | ----- |
| `Ctrl + F` | Arama |
| `Ctrl + R` / `F5` | Listeyi yenile |
| `Ctrl + Shift + U` | Tümünü güncelle |
| `Ctrl + ,` | Ayarlar |

---

## ⚠️ Bilinen Sorunlar ve Çözümleri

| Sorun | Neden Olur | Çözüm |
| ----- | ---------- | ----- |
| Paket kurulamıyor | Winget veya izin sorunu | Terminali yönetici aç; `winget install --id Paket.Adı` ile dene |
| Winget algılanmıyor | App Installer eski | Microsoft Store'dan App Installer güncelle |
| Erişim reddedildi | UAC / antivirus | UniGetUI'yi yönetici olarak çalıştır; güvenlik duvarı istisnası ekle |
| .NET hatası | Runtime eksik | [.NET 8 Desktop Runtime](https://dotnet.microsoft.com/download) kur |
| Yavaş arama | Önbellek | Ayarlardan önbelleği temizle ve listeyi yenile |

---

## 🔗 Faydalı Bağlantılar

- 🌐 [Resmi Web Sitesi](https://devolutions.net/unigetui/)
- 💾 [GitHub Sayfası](https://github.com/Devolutions/UniGetUI)
- 📖 [Dokümantasyon](https://github.com/Devolutions/UniGetUI/wiki)

---

## 📝 Notlar

> Bir paket UniGetUI'de kurulmazsa sorun çoğu zaman WinGet kaynağındadır — aynı komutu PowerShell'de `winget install --id ...` ile dene. npm/pip paketleri geliştirici araçları içindir; günlük yazılım kurulumu için WinGet yeterlidir.

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
