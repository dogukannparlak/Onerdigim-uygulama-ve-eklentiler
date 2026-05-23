# 🛠️ LocalSend

> **Kısa Açıklama:** Aynı WiFi ağındaki cihazlar arasında internet veya bulut olmadan dosya paylaşmanı sağlar.

1.17 · Windows / Android / iOS / macOS / Linux · Ücretsiz · Dosya Paylaşımı

---

## 📌 Genel Bakış

LocalSend, AirDrop benzeri yerel ağ dosya transferi sunan açık kaynak bir uygulamadır. Telefon, bilgisayar ve tablet arasında hesap açmadan, kablo takmadan dosya gönderebilirsin. Veriler yalnızca yerel ağda kalır; buluta yüklenmez.

---

## ✨ Öne Çıkan Özellikler

- **İnternetsiz** - Aynı WiFi ağı yeterli; veriler ağ dışına çıkmaz
- **Çoklu platform** - Windows, Android, iOS, macOS, Linux
- **Şifreli transfer** - HTTPS ile güvenli aktarım

---

## 📥 İndirme ve Kurulum

### Yöntem 1: Resmi Site ( Önerilen )

1. [localsend.org/tr](https://localsend.org/tr) adresine git
2. **İndir** butonuna tıkla ve Windows sürümünü kur

### Yöntem 2: WinGet (Terminal)

```powershell
winget install LocalSend.LocalSend
```

### Yöntem 3: UniGetUI

> UniGetUI açıkken arama çubuğuna **LocalSend** yaz ve kur.

---

## ⚙️ İlk Kurulum ve Önerilen Ayarlar

1. **Her cihaza kur:** Gönderen ve alan cihazda LocalSend açık olmalı.
2. **Aynı ağ:** İkisi de aynı WiFi'ye bağlı olsun (misafir ağ / AP isolation kapalı).
3. **Cihaz adı:** Ayarlardan cihazını tanınabilir bir isimle adlandır.

> 💡 **İpucu:** Cihaz görünmüyorsa Windows ağ profilini **Özel** yap. Güvenlik için isteğe bağlı PIN doğrulaması açılabilir.

---

## 🚀 Temel Kullanım

### Dosya gönderme

1. LocalSend'i aç
2. **Gönder** sekmesinden dosya veya metin seç
3. Listeden hedef cihaza tıkla
4. Karşı tarafta **Kabul et** - transfer başlar

### Dosya alma

1. **Al** sekmesinde bekle
2. Gelen isteği onayla
3. Dosya varsayılan olarak **İndirilenler** klasörüne kaydedilir

---

## ⚠️ Bilinen Sorunlar ve Çözümleri

| Sorun | Çözüm |
| ----- | ----- |
| Cihaz listede görünmüyor | Aynı WiFi; router'da AP isolation kapalı; Windows ağı **Özel** yap |
| Transfer yavaş | 5 GHz WiFi kullan; mümkünse cihazları router'a yakın tut |
| Güvenlik duvarı engelliyor | Port **53317** (TCP/UDP) için LocalSend'e izin ver |

---

## 🔗 Faydalı Bağlantılar

- 🌐 [Resmi Site (TR)](https://localsend.org/tr)
- 💾 [GitHub Sayfası](https://github.com/localsend/localsend)
- 📦 [İndirme (Releases)](https://github.com/localsend/localsend/releases)

---

## 📝 Notlar

> Gmail taslaklarına veya USB kabloya gerek kalmadan telefon–PC arası dosya aktarımı için pratik bir çözüm. Otomatik güncelleme yok; güncellemeleri elle veya WinGet ile yap.

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
