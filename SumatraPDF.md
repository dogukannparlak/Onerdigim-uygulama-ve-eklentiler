# 🛠️ SumatraPDF

> **Kısa Açıklama:** Windows için hafif, hızlı ve taşınabilir belge görüntüleyici; PDF okumak için Adobe Reader'a hafif alternatif.

Güncel · Windows · Açık kaynak (GPL) · PDF Araçları

---

## 📌 Genel Bakış

SumatraPDF, performans ve sadelik odaklı açık kaynaklı bir belge okuyucudur. Düşük bellek kullanımı, anında açılış ve minimal arayüzüyle PDF, e-kitap ve çizgi roman formatlarını görüntüler. PDF düzenleme veya oluşturma sunmaz; salt okuma odaklıdır.

---

## ✨ Öne Çıkan Özellikler

- **Hafif ve hızlı** - Düşük RAM kullanımı, anında açılış
- **Taşınabilir** - ZIP veya tek EXE; kurulum zorunlu değil
- **Çoklu format** - PDF, EPUB, MOBI, DjVu, XPS, CBZ/CBR, CHM
- **Minimal arayüz** - Menü varsayılan gizli (F9); odak okuma
- **Arama ve gezinme** - Metin arama, sayfa atlama
- **Açık kaynak** - Kod GitHub'da incelenebilir

---

## 📥 İndirme ve Kurulum

### Yöntem 1: Resmi Site (Önerilen)

1. [sumatrapdfreader.org](https://www.sumatrapdfreader.org/download-free-pdf-viewer) adresine git
2. **İndir** → **64-bit** seç
3. ZIP dosyasını indir ve çıkart
4. `SumatraPDF.exe` dosyasını çalıştır

> Taşınabilir sürüm kurulum gerektirmez. Kalıcı kurulum isteyenler aynı sayfadan installer sürümünü de indirebilir.

### Yöntem 2: WinGet (Terminal)

```powershell
winget install SumatraPDF.SumatraPDF
```

### Yöntem 3: UniGetUI

> UniGetUI açıkken arama çubuğuna **SumatraPDF** yaz ve kur.

### Yöntem 4: Chocolatey

```powershell
choco install sumatrapdf
```

### Yöntem 5: Scoop

```powershell
scoop install sumatrapdf
```

---

## ⚙️ İlk Kurulum ve Önerilen Ayarlar

1. **Varsayılan PDF okuyucu:** Windows → Ayarlar → Uygulamalar → Varsayılan uygulamalar → `.pdf` için SumatraPDF seç.
2. **Dosya ilişkilendirme:** PDF dosyalarına çift tıklayınca doğrudan açılsın.
3. **Arayüz:** Menü gizli kalabilir; gerektiğinde `F9` ile göster/gizle.

> 💡 **İpucu:** Açılış yavaşsa SumatraPDF klasörünü antivirüs istisnalarına eklemeyi dene.

---

## 🚀 Temel Kullanım

### PDF açma ve okuma

1. `SumatraPDF.exe` çalıştır veya bir PDF dosyasına çift tıkla
2. Okumak için sayfalar arasında gezin
3. Metin aramak için `Ctrl+F` kullan

---

## ⚠️ Bilinen Sorunlar ve Çözümleri


| Sorun                 | Neden Olur                   | Çözüm                                               |
| --------------------- | ---------------------------- | --------------------------------------------------- |
| PDF açılmıyor         | Dosya bozuk veya izin sorunu | Başka bir PDF ile dene; dosya izinlerini kontrol et |
| Yavaş açılış          | Antivirüs taraması           | SumatraPDF klasörünü istisnaya ekle                 |
| Metin bozuk görünüyor | PDF yazı tipi veya kodlama   | Farklı PDF ile test et; güncel sürüm kullan         |


---

## 🔗 Faydalı Bağlantılar

- 🌐 [Resmi Web Sitesi](https://www.sumatrapdfreader.org/)
- 💾 [GitHub Sayfası](https://github.com/sumatrapdfreader/sumatrapdf)
- 📥 [İndirme Sayfası](https://www.sumatrapdfreader.org/download-free-pdf-viewer)

---

## 📝 Notlar

> SumatraPDF salt okuma odaklıdır; PDF düzenleme veya birleştirme için Bento PDF gibi farklı araçlarla birlikte kullanılabilir. Adobe Acrobat Reader'a kıyasla çok daha hafiftir; gelişmiş PDF düzenleme özellikleri sunmaz.

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
