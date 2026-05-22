# 🛠️ Playnite

> **Kısa Açıklama:** Steam, Epic, GOG, Xbox ve diğer platformlardaki oyunlarını tek kütüphanede toplayan açık kaynak oyun başlatıcısı.

10.53 · Windows 10/11 · MIT / ücretsiz · Oyun

---

## 📌 Genel Bakış

Playnite tüm oyunlarını tek arayüzde gösterir; kapak görselleri, filtreler ve istatistikler sunar. Oyun mağazası değildir — çoğu oyun yine Steam, Epic veya ilgili platform üzerinden başlatılır. Emülatör desteği ve Big Picture modu ile TV/kumanda kullanımına da uygundur.

---

## ✨ Öne Çıkan Özellikler

- **Çoklu platform** — Steam, Epic, GOG, Xbox, Ubisoft, EA, Battle.net ve daha fazlası
- **Otomatik metadata** — IGDB vb. kaynaklardan kapak, açıklama, tür bilgisi
- **Big Picture** — TV ve gamepad için tam ekran mod
- **Tema ve eklenti** — Arayüz özelleştirme, ek entegrasyonlar
- **Emülatör desteği** — Retro oyunları aynı kütüphanede topla
- **Ücretsiz** — Açık kaynak, reklamsız

---

## 📥 İndirme ve Kurulum

### Yöntem 1: Resmi Site — Önerilen

1. [playnite.link](https://playnite.link/) adresine git
2. **Download** → **Installer** veya **Portable** seç
3. Kurulum sihirbazını tamamla

> **Installer:** sistem entegrasyonu ve otomatik güncelleme. **Portable:** USB'den taşınabilir.

### Yöntem 2: WinGet (Terminal)

```powershell
winget install Playnite.Playnite
```

### Yöntem 3: UniGetUI

> UniGetUI açıkken arama çubuğuna **Playnite** yaz ve kur.

Alternatif: [GitHub Releases](https://github.com/JosefNemec/Playnite/releases)

---

## ⚙️ İlk Kurulum ve Önerilen Ayarlar

1. **İlk sihirbaz:** Açılışta yüklü platformları (Steam, Epic, GOG…) otomatik tespit et → onayla
2. **Kütüphane güncelle:** `Ctrl + F5` ile oyunları içe aktar
3. **Metadata:** Ayarlar → Kütüphane → otomatik metadata ve görsel indirmeyi aç (IGDB önerilir)
4. **Başlangıçta güncelle:** Ayarlardan açılışta kütüphane taramasını etkinleştir (isteğe bağlı)

> 💡 Oyun başlamıyorsa ilgili platform istemcisinin (Steam, Epic vb.) kurulu ve giriş yapılmış olması gerekir.

---

## 🚀 Temel Kullanım

### Oyun oynama

1. Playnite'ı aç — oyunlar grid veya liste görünümünde listelenir
2. Oyuna çift tıkla veya **Play** — ilgili platform üzerinden başlar
3. Yeni oyun eklediysen **Ctrl + F5** ile kütüphaneyi yenile

### Manuel oyun / emülatör

1. **Ctrl + Shift + A** → Oyun ekle
2. El ile, emülatör veya klasör tarama seçeneklerinden birini kullan

### Big Picture (TV modu)

1. **F11** veya View → **Fullscreen mode**
2. Gamepad ile gezin; oturma odası / TV kurulumu için uygundur

### Klavye kısayolları

| Kısayol | İşlev |
| ------- | ----- |
| `Ctrl + F` | Hızlı arama |
| `Ctrl + F5` | Kütüphaneyi güncelle |
| `Ctrl + D` | Metadata indir |
| `F2` | Filtre paneli |
| `F3` | Seçili oyunu düzenle |
| `F11` | Tam ekran / Big Picture |
| `Ctrl + ,` | Ayarlar |

---

## ⚠️ Bilinen Sorunlar ve Çözümleri

| Sorun | Neden Olur | Çözüm |
| ----- | ---------- | ----- |
| Oyun başlamıyor | Platform istemcisi kapalı | Steam/Epic/GOG uygulamasını aç; giriş yap |
| Oyun listede yok | Kütüphane güncel değil | `Ctrl + F5`; Ayarlar → Entegrasyonlar → platformu kontrol et |
| Kapak görseli yok | Metadata inmemiş | Oyun → Düzenle → Meta veri indir; veya `Ctrl + D` |
| Yanlış oyun yolu | Taşınmış kurulum | Oyun → Düzenle → Kurulum → executable yolunu düzelt |
| Xbox / Game Pass sorunu | Xbox uygulaması | Microsoft Store Xbox app güncel mi; hesaba giriş yap |
| Eklenti hatası | Sürüm uyumsuzluğu | Eklentiyi güncelle veya devre dışı bırak |

---

## 🔗 Faydalı Bağlantılar

- 🌐 [Resmi Web Sitesi](https://playnite.link/)
- 📖 [Dokümantasyon](https://playnite.link/docs/)
- 💾 [GitHub Sayfası](https://github.com/JosefNemec/Playnite)
- 🎨 [Temalar ve eklentiler](https://github.com/JosefNemec/Playnite/wiki/Community-add-ons)
- 💬 [Discord topluluğu](https://discord.gg/playnite)

---

## 📝 Notlar

> Playnite kütüphane yöneticisidir; oyun satın almaz ve DRM'yi atlatmaz. Tema/eklenti kurulumu: Ayarlar → Add-ons → Browse → `.pext` / `.pthm` dosyasını indirip yükle. Playnite 11 geliştirme aşamasında; günlük kullanım için kararlı 10.x sürümü yeterlidir.

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
