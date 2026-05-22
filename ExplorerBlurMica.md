# 🛠️ ExplorerBlurMica

> **Kısa Açıklama:** Windows Dosya Gezgini'ne blur, Acrylic veya Mica efekti ekleyerek şeffaf, modern bir görünüm sağlar.

2.0.1 · Windows 10/11 · Açık kaynak (LGPL/GPL) · Görsel / Kişiselleştirme

---

## 📌 Genel Bakış

ExplorerBlurMica, yalnızca **Dosya Gezgini** pencerelerine cam benzeri arka plan efektleri uygular. Windows 11'in Mica görünümünü Explorer'a taşımak veya Windows 10'da Acrylic efekti kullanmak isteyenler için pratik bir çözümdür. StartAllBack, OldNewExplorer ve üçüncü parti temalarla uyumludur.

> Tüm sistem genelinde blur istiyorsan geliştiricinin **DWMBlurGlass** projesine bak.

---

## ✨ Öne Çıkan Özellikler

- **Blur / Acrylic / Mica** — Beş farklı efekt türü (`effect=0`–`4`)
- **Açık/koyu mod uyumu** — Sistem temasına göre renk ayarı
- **RGBA renk kontrolü** — Karışım rengini ve şeffaflığı ince ayarla
- **Temiz arayüz** — Adres çubuğu, scrollbar ve WinUI arka planlarını kaldır
- **Hafif kurulum** — DLL kaydı; arka planda çalışan ayrı bir uygulama yok
- **Ücretsiz ve açık kaynak** — GitHub'dan indirilir

---

## 📥 İndirme ve Kurulum

> WinGet veya Store paketi yok; kurulum GitHub Release üzerinden yapılır.

### Yöntem 1: GitHub Release — Önerilen

1. [Release sayfasından](https://github.com/Maplespe/ExplorerBlurMica/releases/latest) `Release_x64.zip` indir
2. Arşivi `C:\Program Files\ExplorerBlurMica` gibi kalıcı bir klasöre çıkar
3. `register.cmd` dosyasını **yönetici olarak** çalıştır
4. Açık Dosya Gezgini pencerelerini kapatıp yeniden aç

### Kaldırma

1. `uninstall.cmd` dosyasını **yönetici olarak** çalıştır
2. Klasörü sil

> Explorer çökerse `ESC` tuşunu basılı tutarak Gezgini aç, ardından kaldır.

---

## ⚙️ İlk Kurulum ve Önerilen Ayarlar

Kurulumdan sonra aynı klasördeki `config.ini` dosyasını düzenle. Kaydettikten sonra Gezgini yeniden aç.

### Efekt seçimi


| `effect` | Efekt        | Uyumluluk           |
| -------- | ------------ | ------------------- |
| `0`      | Blur         | Win11 22H2'ye kadar |
| `1`      | Acrylic      | Win10 ve Win11      |
| `2`      | Mica         | Yalnızca Win11      |
| `3`      | Blur (Clear) | Win10 ve Win11      |
| `4`      | MicaAlt      | Yalnızca Win11      |


### Önerilen ayarlarım

```ini
[config]
effect=1
clearAddress=true
clearBarBg=true
clearWinUIBg=true
showLine=true

[light]
r=255
g=255
b=255
a=200

[dark]
r=0
g=0
b=0
a=120
```

- **Acrylic (`effect=1`)** — Win10/11'de en dengeli seçenek
- **Temizleme seçenekleri** — Adres çubuğu, scrollbar ve WinUI arka planı kaldırılır
- `**showLine=true`** — Sol panel ile dosya listesi arasındaki ayırıcı çizgiyi gizler
- **Renkler** — Açık modda beyaz ton, koyu modda siyah ton; `a` değeri şeffaflığı belirler (0–255)

> 💡 Düşük performanslı sistemlerde `effect=0` veya `a` değerini düşürmeyi dene.

---

## 🚀 Temel Kullanım

### Efektin devreye girmesi

1. Kurulumdan sonra yeni bir Dosya Gezgini penceresi aç
2. Efekt birkaç saniye içinde görünür
3. Değişiklik yoksa `config.ini`'yi kontrol et ve pencereleri tamamen kapatıp aç

### Ayar değiştirme

1. Kurulum klasöründeki `config.ini` dosyasını Not Defteri ile aç
2. `effect`, `clearAddress`, `[light]` / `[dark]` bölümlerini düzenle
3. Kaydet → Dosya Gezgini pencerelerini kapatıp yeniden aç

---

## ⚠️ Bilinen Sorunlar ve Çözümleri


| Sorun            | Neden Olur              | Çözüm                                                                            |
| ---------------- | ----------------------- | -------------------------------------------------------------------------------- |
| Efekt görünmüyor | Eski pencere oturumu    | Tüm Gezgini pencerelerini kapat; gerekirse `register.cmd`'yi tekrar çalıştır     |
| Explorer çöküyor | Uyumsuz efekt veya ayar | `ESC` basılı tut → `uninstall.cmd` çalıştır → `config.ini`'yi varsayılana döndür |
| Renkler yanlış   | Hatalı RGBA değeri      | `r/g/b/a` değerlerinin 0–255 arasında olduğundan emin ol                         |
| Mica çalışmıyor  | Win10 veya eski Win11   | `effect=1` (Acrylic) veya `effect=3` dene                                        |
| Performans düşük | Yoğun blur/Mica         | `effect=0` kullan veya `a` değerini düşür                                        |


---

## 🔗 Faydalı Bağlantılar

- 💾 [GitHub Sayfası](https://github.com/Maplespe/ExplorerBlurMica)
- 📦 [Son Sürüm (Release)](https://github.com/Maplespe/ExplorerBlurMica/releases/latest)

---

## 📝 Notlar

> ExplorerBlurMica bir shell extension'dır; yönetici haklarıyla kayıt edilir ve Explorer sürecine müdahale eder. Windows güncellemelerinden sonra efekt kaybolursa `register.cmd`'yi yeniden çalıştırmak yeterli olabilir. Resmi son sürüm Şubat 2024'ten beri 2.0.1; yeni Windows sürümlerinde uyumluluk sorunu yaşarsan GitHub Issues sayfasını kontrol et.

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