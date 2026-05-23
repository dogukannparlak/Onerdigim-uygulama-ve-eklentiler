# 🛠️ QuickLook

> **Kısa Açıklama:** Dosyayı açmadan Space tuşuyla anında önizlemen; macOS Quick Look deneyimini Windows'a taşır.

4.5.x · Windows 10/11 · GPL-3.0 · Verimlilik

---

## 📌 Genel Bakış

QuickLook, Dosya Gezgini, masaüstü ve Aç/Kaydet pencerelerinde seçili dosyayı tek tuşla önizlemeni sağlar. Resim, PDF, video, metin ve Office dosyalarını ayrı program açmadan hızlıca kontrol etmek isteyenler için idealdir. Windows'un yerleşik önizlemesinden farklı olarak ok tuşlarıyla klasördeki diğer dosyalar arasında gezinebilirsin.

---

## ✨ Öne Çıkan Özellikler

- **Space ile önizleme** - Dosyayı seç, Space'e bas, anında gör
- **Ok tuşlarıyla gezinme** - Aynı klasördeki dosyalar arasında hızlı geçiş
- **Çok format desteği** - Resim, PDF, video, ses, metin, arşiv ve daha fazlası
- **Plugin desteği** - Office, e-kitap, klasör listesi gibi ek görüntüleyiciler
- **Arka planda çalışır** - Sistem tepsisinde; ihtiyaç anında devreye girer
- **Ücretsiz** - Açık kaynak, reklamsız

---

## 📥 İndirme ve Kurulum

### Yöntem 1: Microsoft Store ( Önerilen )

1. Microsoft Store'u aç
2. **QuickLook** ara (yayıncı: Paddy Xu)
3. **Al** veya **Yükle** butonuna tıkla

[Store bağlantısı](https://www.microsoft.com/store/apps/9NV4BS3L1H4S)

> Otomatik güncelleme ve kolay kaldırma için Store sürümü tercih edilir.

### Yöntem 2: WinGet (Terminal)

```powershell
winget install QL-Win.QuickLook
```

### Yöntem 3: UniGetUI

> UniGetUI açıkken arama çubuğuna **QuickLook** yaz ve kur.

---

## ⚙️ İlk Kurulum ve Önerilen Ayarlar

1. **Çalıştığını kontrol et:** Kurulumdan sonra sistem tepsisinde QuickLook simgesi görünmeli
2. **Başlangıçta aç:** Ayarlardan Windows ile birlikte başlatmayı etkinleştir
3. **Test et:** Herhangi bir dosyayı seç → Space

> 💡 Plugin kurulumu: QuickLook çalışırken `.qlplugin` dosyasını seç, Space'e bas, **Install** butonuna tıkla ve QuickLook'u yeniden başlat.

---

## 🚀 Temel Kullanım

### Dosya önizleme

1. Dosya Gezgini veya masaüstünde bir dosyayı seç
2. **Space** tuşuna bas - önizleme penceresi açılır
3. **↑ ↓ ← →** ile aynı klasördeki diğer dosyalara geç
4. **Space** veya **Esc** ile kapat

### Klavye kısayolları


| Kısayol           | İşlev                             |
| ----------------- | --------------------------------- |
| `Space`           | Önizlemeyi aç / kapat             |
| `Esc`             | Önizlemeyi kapat                  |
| `Enter`           | Dosyayı varsayılan uygulamayla aç |
| `↑ ↓ ← →`         | Diğer dosyalara geç               |
| `Ctrl + Tekerlek` | PDF yakınlaştırma                 |


---

## ⚠️ Bilinen Sorunlar ve Çözümleri


| Sorun                          | Neden Olur              | Çözüm                                                                                  |
| ------------------------------ | ----------------------- | -------------------------------------------------------------------------------------- |
| Space çalışmıyor               | Odak başka pencerede    | Explorer'a tıkla; Everything arama kutusu açıksa kapat                                 |
| Önizleme açılmıyor             | Servis durmuş           | QuickLook'u yeniden başlat; gerekirse WinGet sürümünü dene                             |
| Win11 donma / şeffaflık hatası | Görüntü API uyumsuzluğu | `%APPDATA%\QuickLook\user_config.ini` → `[Appearance]` altında `UseTransparency=false` |



---

## 🔗 Faydalı Bağlantılar

- 🏪 [Microsoft Store](https://www.microsoft.com/store/apps/9NV4BS3L1H4S)
- 💾 [GitHub Sayfası](https://github.com/QL-Win/QuickLook)
- 📦 [Son Sürüm (Release)](https://github.com/QL-Win/QuickLook/releases/latest)
- 🔌 [Plugin Listesi](https://github.com/QL-Win)

---

## 📝 Notlar

> Store sürümünde bazı gelişmiş özellikler veya plugin desteği sınırlı olabilir; sorun yaşarsan GitHub/WinGet sürümünü dene. Windows Defender bazen QuickLook'u yanlış pozitif olarak işaretleyebilir - resmi kaynaktan indirdiğinden emin ol.

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
