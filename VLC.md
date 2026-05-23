# 🛠️ VLC Media Player

> **Kısa Açıklama:** Neredeyse tüm video ve ses formatlarını ek codec paketi gerektirmeden oynatan ücretsiz medya oynatıcısı.

Güncel · Windows/macOS/Linux/Android · Ücretsiz / açık kaynak · Medya

---

## 📌 Genel Bakış

VLC, VideoLAN tarafından geliştirilen evrensel bir medya oynatıcısıdır. MP4, MKV, AVI, MP3, FLAC ve yüzlerce formatı ek yazılım kurmadan açar. Windows Media Player veya tarayıcı oynatıcıların açamadığı dosyaları, bozuk veya yarım kalmış medyayı bile çoğu zaman oynatabilir.

---

## ✨ Öne Çıkan Özellikler

- **Evrensel format desteği** - Codec paketi gerekmez
- **Altyazı desteği** - SRT, ASS ve diğer formatlar
- **Dönüştürme** - Video/ses formatı değiştirme
- **Ağ akışı** - URL ile çevrimiçi video oynatma
- **Platformlar arası** - Windows, macOS, Linux, Android, iOS
- **Ücretsiz** - Reklamsız, açık kaynak

---

## 📥 İndirme ve Kurulum

### Yöntem 1: Resmi Site ( Önerilen )

1. [videolan.org/vlc](https://www.videolan.org/vlc/) adresine git
2. **Download VLC** butonuna tıkla
3. Kurulum sihirbazını takip et

> Kurulumda istenmeyen yazılım tekliflerine dikkat et; yalnızca VLC'yi seç.

### Yöntem 2: Microsoft Store

Microsoft Store'da **VLC** ara (yayıncı: VideoLAN) ve yükle.

### Yöntem 3: WinGet (Terminal)

```powershell
winget install VideoLAN.VLC
```

### Yöntem 4: UniGetUI

> UniGetUI açıkken arama çubuğuna **VLC** yaz ve kur.

---

## ⚙️ İlk Kurulum ve Önerilen Ayarlar

1. **Varsayılan oynatıcı (isteğe bağlı):** Ayarlar → Uygulamalar → Varsayılan uygulamalar → Video için VLC seç
2. **Donanım hızlandırma:** Araçlar → Tercihler → Giriş / Codecs → Donanım hızlandırmalı kod çözmeyi dene (sorun olursa kapat)
3. **Altyazı:** Araçlar → Tercihler → Altyazılar → UTF-8 kodlama
4. **Arayüz dili:** Araçlar → Tercihler → Arayüz → Dil → Türkçe

> 💡 Oynatma sorunu yaşarsan donanım hızlandırmayı kapatmak çoğu zaman işe yarar.

---

## 🚀 Temel Kullanım

### Dosya oynatma

1. VLC'yi aç → **Medya → Dosya Aç** (`Ctrl + O`)
2. Veya video/ses dosyasını VLC penceresine **sürükle-bırak**
3. Çift tıkla veya Enter ile oynat

### Oynatma listesi

1. **Medya → Dosya Aç** ile birden fazla dosya seç
2. Veya **Ctrl + L** ile oynatma listesi panelini aç

### Klavye kısayolları


| Kısayol     | İşlev            |
| ----------- | ---------------- |
| `Space`     | Oynat / duraklat |
| `F` / `F11` | Tam ekran        |
| `Ctrl + O`  | Dosya aç         |
| `Ctrl + L`  | Oynatma listesi  |
| `+` / `-`   | Ses seviyesi     |
| `[` / `]`   | Oynatma hızı     |


---

## ⚠️ Bilinen Sorunlar ve Çözümleri


| Sorun                         | Neden Olur          | Çözüm                                                  |
| ----------------------------- | ------------------- | ------------------------------------------------------ |
| Ses-görüntü senkronu bozuk    | Codec veya kaynak   | Araçlar → Senkronizasyon ile gecikmeyi ayarla          |
| Video takılıyor / siyah ekran | Donanım hızlandırma | Tercihler → Giriş/Codecs → donanım hızlandırmayı kapat |
| Altyazı bozuk karakter        | Yanlış kodlama      | Tercihler → Altyazılar → UTF-8                         |
| Ses yok                       | Yanlış ses kanalı   | Ses → Ses kanalı → Stereo veya 5.1 dene                |
| Ağ akışı açılmıyor            | URL veya protokol   | Medya → Ağ akışı aç (`Ctrl + N`); URL'yi kontrol et    |


---

## 🔗 Faydalı Bağlantılar

- 🌐 [Resmi Web Sitesi](https://www.videolan.org/vlc/)
- 📖 [Desteklenen Formatlar](https://www.videolan.org/vlc/features.html)
- 💾 [GitHub Sayfası](https://github.com/videolan/vlc)

---

## 📝 Notlar

> VLC çok yönlüdür ama günlük kullanımda çoğu kişi yalnızca dosya açmak için kullanır. Gelişmiş özellikler (IPTV, ekran kaydı, Chromecast) mevcuttur; ayrıntılar için resmi wiki'ye bak. Kurulumda sunulan ek yazılımları reddetmek güvenli kurulum için önerilir.

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