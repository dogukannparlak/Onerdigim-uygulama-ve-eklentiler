# ExplorerBlurMica

## Genel Bakış

ExplorerBlurMica, Windows 10 ve Windows 11 için dosya gezgininde arka plan blur (bulanıklık), Acrylic veya Mica efektleri ekleyen bir uygulamadır. Bu proje, Windows Explorer’ın görsel deneyimini modern ve şeffaf efektlerle zenginleştirmek için geliştirilmiştir.

**Proje URL:** [https://github.com/Maplespe/ExplorerBlurMica](https://github.com/Maplespe/ExplorerBlurMica)

## Özellikler

### Efekt Türleri

- **Blur (Bulanıklık):** Klasik bulanıklık efekti
- **Acrylic:** Windows 10 tarzı yarı saydam efekt
- **Mica:** Windows 11’e özel modern material efekt
- **Blur (Clear):** Temiz bulanıklık efekti (Windows 10 ve 11’de çalışır)
- **MicaAlt:** Mica’nın alternatif versiyonu

### Kişiselleştirme Seçenekleri

- Özel karışım renkleri ayarlama
- Açık/Koyu mod otomatik uyum
- RGBA renk bileşenleri ile tam kontrol
- Adres çubuğu arka plan temizleme
- Scrollbar arka plan temizleme
- WinUI arka plan temizleme

### Uyumluluk

- **Windows 10:** Tam destek
- **Windows 11 22H2:** XamlIslands desteği
- **Windows 11 23H2:** WinUI3 desteği
- **Üçüncü parti yazılımlar:** StartAllBack, OldNewExplorer gibi uygulamalarla uyumlu
- **Temalar:** Üçüncü parti temalarla uyumlu

## Kurulum

### Adım 1: İndirme

1. [GitHub Release sayfasından](https://github.com/Maplespe/ExplorerBlurMica/releases) en son sürümü indirin
2. Dosyayı `C:\Program Files` gibi uygun bir konuma çıkarın

### Adım 2: Kurulum

1. `register.cmd` dosyasını **yönetici olarak** çalıştırın
2. Dosya Gezgini pencerelerini yeniden açın
3. Efektlerin devreye girmesi için birkaç saniye bekleyin

**Manuel kurulum komutu:**

```
regsvr32 "dosya_yolu/ExplorerBlurMica.dll"
```

### Kaldırma

1. `uninstall.cmd` dosyasını **yönetici olarak** çalıştırın
2. Kalan dosyaları silin

**Manuel kaldırma komutu:**

```
regsvr32 /u "dosya_yolu/ExplorerBlurMica.dll"
```

**⚠️ Önemli Not:** Eğer Explorer çökerse, `ESC` tuşunu basılı tutarak Explorer’ı açın ve programı kaldırın.

## Yapılandırma Dosyası

Yapılandırma dosyası (`config.ini`) ile tüm ayarları özelleştirebilirsiniz:

### Temel Ayarlar

```
[config]
# Efekt türü: 0=Blur, 1=Acrylic, 2=Mica, 3=Blur(Clear), 4=MicaAlt
effect=1

# Adres çubuğu arka planını temizle
clearAddress=true

# Scrollbar arka plan rengini temizle
clearBarBg=true

# Windows 11 WinUI/XamlIslands toolbar arka planını kaldır
clearWinUIBg=true

# TreeView ve DUIView arasında ayırıcı çizgi göster
showLine=true

[light]
# Açık mod için RGBA renk değerleri
r=220    # Kırmızı (0-255)
g=220    # Yeşil (0-255)
b=220    # Mavi (0-255)
a=160    # Şeffaflık (0-255, 0=tamamen şeffaf, 255=opak)

[dark]
# Koyu mod için RGBA renk değerleri
r=0      # Kırmızı
g=0      # Yeşil
b=0      # Mavi
a=120    # Şeffaflık
```

### Efekt Türü Açıklamaları

| Efekt | Açıklama | Uyumluluk |
| --- | --- | --- |
| 0 - Blur | Klasik bulanıklık | Windows 11 22H2’ye kadar |
| 1 - Acrylic | Yarı saydam cam efekt | Windows 10 ve 11 |
| 2 - Mica | Modern material | Sadece Windows 11 |
| 3 - Blur(Clear) | Temiz bulanıklık | Windows 10 ve 11 |
| 4 - MicaAlt | Mica alternatifi | Sadece Windows 11 |

## Kişisel Ayarlarım

```
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

### Ayar Açıklamaları

- **Efekt:** Acrylic (1) - Modern yarı saydam cam efekti
- **Adres çubuğu temizleme:** Aktif - Daha temiz görünüm
- **Scrollbar temizleme:** Aktif - Scrollbar arka planı şeffaf
- **WinUI temizleme:** Aktif - Toolbar arka planı şeffaf
- **Ayırıcı çizgi:** Aktif - TreeView ve liste arasında çizgi

**Renk Ayarları:**
- **Açık mod:** Beyaz tonları (255,255,255) %78 şeffaflık ile
- **Koyu mod:** Siyah tonları (0,0,0) %47 şeffaflık ile

## Sorun Giderme

### Yaygın Sorunlar

1. **Efekt görünmüyor:**
    - Explorer pencerelerini tamamen kapatıp yeniden açın
    - Yapılandırma dosyasını kontrol edin
    - DLL dosyasının doğru konumda olduğundan emin olun
2. **Explorer çöküyor:**
    - ESC tuşunu basılı tutarak Explorer’ı açın
    - Programı kaldırın (`uninstall.cmd`)
    - Yapılandırma ayarlarını varsayılana döndürün
3. **Renkler yanlış:**
    - RGBA değerlerini kontrol edin (0-255 arası)
    - Sistem tema ayarlarını kontrol edin

### Performans İpuçları

- Düşük performanslı sistemlerde `effect=0` (Blur) kullanın
- Şeffaflık değerini (a) düşürerek performansı artırabilirsiniz
- Gereksiz temizleme seçeneklerini kapatın

## Teknik Detaylar

### Gereksinimler

- Windows 10 1809+ veya Windows 11
- .NET Framework (otomatik yüklenir)
- Yönetici hakları (kurulum için)

### Kullanılan Teknolojiler

- C++ ile geliştirilmiş DLL
- Python GUI (minhook ve customtkinter bağımlılıkları)
- Windows API entegrasyonu
- Shell Extension mimarisi

### Lisans

- LGPL-3.0 ve GPL-3.0 çifte lisans
- Açık kaynak proje
- Ticari kullanım için uygun

## İlgili Projeler

Eğer sistem genelinde blur efekti istiyorsanız, aynı geliştiricinin **DWMBlurGlass** projesine bakın.

---

**Son Güncelleme:** 2024-02-11

**Sürüm:** 2.0.1

**Geliştirici:** Maplespe

**GitHub:** [https://github.com/Maplespe/ExplorerBlurMica](https://github.com/Maplespe/ExplorerBlurMica)