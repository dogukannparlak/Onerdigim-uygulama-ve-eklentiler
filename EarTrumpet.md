# 🛠️ EarTrumpet

> **Kısa Açıklama:** Windows'ta her uygulamanın ses seviyesini ayrı ayrı kontrol etmeni ve çıkış cihazını hızlıca değiştirmeni sağlar.

Güncel · Windows 10/11 · Ücretsiz · Sistem Araçları

---

## 📌 Genel Bakış

EarTrumpet, Windows'un varsayılan ses karıştırıcısının ötesinde uygulama bazlı ses kontrolü sunar. Discord, tarayıcı, oyun ve medya oynatıcısının sesini birbirinden bağımsız ayarlayabilir; kulaklık, hoparlör veya HDMI çıkışı arasında geçiş yapabilirsin. Microsoft Store Community Choice Awards 2022 kazananıdır.

---

## ✨ Öne Çıkan Özellikler

- **Uygulama bazlı ses** - Her programın seviyesi ayrı kaydırıcı
- **Cihaz yönetimi** - Varsayılan çıkış/giriş cihazını hızlı değiştir
- **Sistem tepsisi** - Bildirim alanından anında erişim
- **Görsel ses çubukları** - Hangi uygulamanın ses verdiğini gör
- **Tema desteği** - Açık, koyu veya sistem teması
- **Ücretsiz** - Microsoft Store'dan güvenle kurulabilir

---

## 📥 İndirme ve Kurulum

### Yöntem 1: Microsoft Store ( Önerilen )

1. Microsoft Store'u aç
2. **EarTrumpet** ara (yayıncı: File-New-Project)
3. **Al** veya **Yükle** butonuna tıkla

[Direkt Store bağlantısı](https://www.microsoft.com/store/productId/9NBLGGH516XP)

> Otomatik güncelleme ve kolay kaldırma için Store sürümü tercih edilir.

### Yöntem 2: WinGet (Terminal)

```powershell
winget install File-New-Project.EarTrumpet
```

### Yöntem 3: UniGetUI

> UniGetUI açıkken arama çubuğuna **EarTrumpet** yaz ve kur.

### Yöntem 4: Chocolatey

```powershell
choco install eartrumpet
```

---

## ⚙️ İlk Kurulum ve Önerilen Ayarlar

1. **Simgeyi sabitle:** Kurulumdan sonra bildirim alanındaki EarTrumpet simgesini görünür tut (gizliyse ok işaretine tıkla → sürükle).
2. **Başlangıçta aç (isteğe bağlı):** Ayarlar → Windows ile birlikte başlat.
3. **Tema:** Ayarlardan açık/koyu veya sistem temasını seç.

> 💡 **İpucu:** EarTrumpet ses yükseltmez; yalnızca Windows ses seviyesini uygulama bazında ayırır. Ek amplifikasyon için Volume Master gibi araçlar ayrı düşünülmeli.

---

## 🚀 Temel Kullanım

### Uygulama sesini ayarlama

1. Bildirim alanındaki EarTrumpet simgesine **sol tıkla**
2. Listeden uygulamayı bul (Discord, Chrome, Spotify vb.)
3. Kaydırıcıyı istediğin seviyeye getir - diğer uygulamalar etkilenmez

### Çıkış cihazı değiştirme

1. EarTrumpet penceresinin üstünden çıkış cihazını seç (kulaklık, hoparlör, HDMI)
2. Seçim anında uygulanır

### Sistem tepsisi kısayolları

| Eylem | İşlev |
| ----- | ----- |
| Sol tık | Ana karıştırıcı penceresini aç |
| Sağ tık | Ayarlar ve bağlam menüsü |
| Tekerlek (simge üzerinde) | Ana sistem ses seviyesi |

---

## ⚠️ Bilinen Sorunlar ve Çözümleri


| Sorun | Neden Olur | Çözüm |
| ----- | ---------- | ----- |
| EarTrumpet açılmıyor | Servis veya Store sorunu | Windows'u yeniden başlat; Store'dan güncelle |
| Ses kontrolü çalışmıyor | Windows Audio servisi | `services.msc` → Windows Audio → Yeniden Başlat |
| Uygulama listede yok | Uygulama ses üretmiyor | Sesli bir uygulama çalıştır; listeyi yenile |
| Kısayol çalışmıyor | Başka uygulama ile çakışma | Ayarlardan kısayolu yeniden tanımla |


---

## 🔗 Faydalı Bağlantılar

- 🏪 [Microsoft Store](https://www.microsoft.com/store/productId/9NBLGGH516XP)
- 💾 [GitHub Sayfası](https://github.com/File-New-Project/EarTrumpet)

---

## 📝 Notlar

> EarTrumpet Windows ses API'sini kullanır; ses sürücüsü veya üçüncü parti ses yazılımı çakışmalarında sorun çıkabilir. Volume Master ile birlikte kullanıldığında toplam ses çok yüksek olabilir - her iki kaydırıcıyı da kontrol et.

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
