# 🛠️ Monitorian

> **Kısa Açıklama:** Windows'ta birden fazla monitörün parlaklığını tek yerden, kaydırıcı ile kolayca ayarlamanı sağlar.

4.14 · Windows 10/11 · Ücretsiz · Sistem Araçları

---

## 📌 Genel Bakış

Monitorian, Windows'un yerleşik parlaklık kontrolünün ötesinde harici monitörleri DDC/CI üzerinden yönetir. Her monitör için ayrı kaydırıcı sunar; istersen hepsini birlikte ayarlayabilirsin. Türkçe dil desteği vardır.

---

## ✨ Öne Çıkan Özellikler

- **Çoklu monitör** - Her ekran için ayrı parlaklık kaydırıcısı
- **Birlikte ayarla** - Tüm monitörleri tek seferde değiştir
- **Tepsi simgesi** - Bildirim alanından hızlı erişim

---

## 📥 İndirme ve Kurulum

### Yöntem 1: Microsoft Store ( Önerilen )

1. Microsoft Store'u aç
2. **Monitorian** ara
3. **Al** veya **Yükle** butonuna tıkla

[Store bağlantısı](https://apps.microsoft.com/detail/9nw33j738bl0?hl=tr-TR&gl=TR)

### Yöntem 2: WinGet (Terminal)

```powershell
winget install emoacht.Monitorian
```

Store sürümü için:

```powershell
winget install Monitorian -s msstore
```

### Yöntem 3: UniGetUI

> UniGetUI açıkken arama çubuğuna **Monitorian** yaz ve kur.

---

## ⚙️ İlk Kurulum ve Önerilen Ayarlar

1. **Simgeyi sabitle:** Bildirim alanında Monitorian simgesini görünür tut.
2. **DDC/CI açık olsun:** Harici monitörün OSD menüsünden DDC/CI etkinleştir.
3. **Başlangıçta aç (isteğe bağlı):** Ayarlardan **Start on sign in** işaretle.

> 💡 **İpucu:** Monitör listede görünmüyorsa kablo/docking istasyonu DDC/CI desteklemiyor olabilir. Doğrudan DisplayPort veya HDMI dene.

---

## 🚀 Temel Kullanım

### Parlaklık ayarlama

1. Bildirim alanındaki Monitorian simgesine **sol tıkla**
2. İlgili monitörün kaydırıcısını istediğin seviyeye getir
3. Tüm monitörler için **Unison** (birlikte) seçeneğini kullanabilirsin

### Monitör adını değiştirme

Monitör adına **basılı tut** - düzenlenebilir hale gelir; monitörleri ayırt etmek için kullanışlıdır.

---

## ⚠️ Bilinen Sorunlar ve Çözümleri

| Sorun | Çözüm |
| ----- | ----- |
| Harici monitör listede yok | Monitör OSD → DDC/CI açık; kablo/dock uyumluluğunu kontrol et |
| Parlaklık değişmiyor | Monitör modeli DDC/CI desteklemiyor olabilir; farklı bağlantı dene |
| Laptop ekranı görünmüyor | Normal - çoğu laptop ekranı dahili kontrol kullanır; harici monitörler için tasarlanmış |

---

## 🔗 Faydalı Bağlantılar

- 🏪 [Microsoft Store](https://apps.microsoft.com/detail/9nw33j738bl0?hl=tr-TR&gl=TR)
- 💾 [GitHub Sayfası](https://github.com/emoacht/monitorian)
- 📦 [İndirme (Releases)](https://github.com/emoacht/monitorian/releases)

---

## 📝 Notlar

> Harici monitör parlaklığını fiziksel tuşlara basmadan ayarlamak isteyenler için en pratik seçeneklerden biri. Store sürümünde kısayol tuşları gibi ek özellikler abonelikle sunulur; temel parlaklık kontrolü ücretsizdir.

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

*Son güncelleme: 2026-05-23*
