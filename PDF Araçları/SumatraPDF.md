# SumatraPDF

# SumatraPDF: Minimalist Performans Odaklı PDF Görüntüleyici

## 🎯 Özet ve Genel Bakış

SumatraPDF, performans ve sadelik felsefesi üzerine inşa edilmiş açık kaynaklı, Windows özelinde tasarlanmış hafif belge görüntüleyicidir. Adobe Reader’ın karmaşıklığına alternatif olarak geliştirilmiş, tek dosyalık taşınabilir yapısı ve minimal kaynak kullanımıyla öne çıkmaktadır.

# 🚀 **Detaylı Kurulum ve Yapılandırma**

## 📥 **Kurulum Yöntemleri**

### **Yöntem 1: Paket Yöneticileri**

```powershell
# Chocolatey
choco install sumatrapdf

# Winget
winget install SumatraPDF.SumatraPDF

# Scoop
scoop install sumatrapdf
```

### **Yöntem 2: Elle Kurulum**

1. [sumatrapdfreader.org](https://www.sumatrapdfreader.org/download-free-pdf-viewer) adresine git
2. “İndir” → “64-bit” seç
3. ZIP dosyasını indir ve çıkart
4. `SumatraPDF.exe` dosyasını çalıştır

## 🛠️ **Kapsamlı Özellik Analizi**

### 📄 **Desteklenen Format Matrisi**

### **Belge Formatları**

| Format | Desteklenen Özellikler | Notlar |
| --- | --- | --- |
| **PDF** | Görüntüleme, Arama, Not Ekleme | Ana format, tam destek |
| **XPS/OpenXPS** | Görüntüleme, Arama | Microsoft formatı |
| **DjVu** | Görüntüleme, Arama | Taranmış belgeler için |
| **PostScript (.ps)** | Görüntüleme | Teknik belgeler |

### **E-kitap Formatları**

| Format | Özellikler |
| --- | --- |
| **EPUB** | Esnek metin, İçindekiler |
| **MOBI** | Kindle formatı |
| **FB2** | FictionBook |
| **PDB** | PalmDoc |
| **TCR** | Psion Text |

### **Arşiv ve Görüntü Formatları**

```
Çizgi Roman Arşivleri:
✅ CBZ (ZIP tabanlı)
✅ CBR (RAR tabanlı)
✅ CB7 (7z tabanlı)
✅ CBT (TAR tabanlı)

Görüntü Formatları:
✅ JPG/JPEG - EXIF veri desteği
✅ PNG - Şeffaflık desteği
✅ GIF - Animasyon desteği (sabit)
✅ WEBP - Modern format
✅ TIFF - Çok sayfa desteği
✅ AVIF - Yeni nesil format
✅ HEIF - Apple formatı

Özel Formatlar:
✅ CHM - Windows Yardım dosyaları
✅ SVG - Vektörel grafikler (temel)
```

## 🎨 **Kullanıcı Arayüzü ve Deneyim**

### **Minimalist Tasarım Felsefesi**

```
Arayüz Öğeleri:
✅ Başlık çubuğu - Belge başlığı
✅ Menü çubuğu - Varsayılan gizli (F9)
✅ Araç çubuğu - Minimal simgeler
✅ Durum çubuğu - Sayfa bilgisi
✅ İçerik alanı - Maksimum alan

Varsayılan Gizli:
- Favoriler paneli
- Yer imleri paneli
- Arama paneli
- İçindekiler tablosu
- Sayfa küçük resimleri

Erişim Yöntemleri:
- Klavye kısayolları (birincil)
- Sağ tık bağlam menüsü
- Komut paleti (Ctrl+K)
- Dokunma hareketleri (sınırlı)
```

### **Klavye Kısayolları (Tam Liste)**

```
Dosya İşlemleri:
Ctrl+O          Dosya aç
Ctrl+Shift+O    Yeni pencerede aç
Ctrl+W          Mevcut sekmeyi kapat
Ctrl+Shift+W    Pencereyi kapat
Ctrl+Q          Uygulamadan çık
Ctrl+R          Belgeyi yeniden yükle

Gezinme:
J / Aşağı       Sonraki sayfa
K / Yukarı      Önceki sayfa
Ctrl+G          Sayfaya git
Home           İlk sayfa
End            Son sayfa
Ctrl+Home      Belge başlangıcı
Ctrl+End       Belge sonu

Görüntüleme Kontrolleri:
+ / Ctrl++     Yakınlaştır
- / Ctrl+-     Uzaklaştır
Ctrl+0         Sayfayı sığdır
Ctrl+1         Gerçek boyut
Ctrl+2         Genişliğe sığdır
Ctrl+3         İçeriğe sığdır
Z              Zoom değiştir
F              Sayfa sığdırma değiştir
F11            Tam ekran
F12            Sunum modu

Arama:
Ctrl+F         Bul
F3             Sonrakini bul
Shift+F3       Öncekini bul
Ctrl+Shift+F   Tüm sekmelerde bul

Görüntüleme:
Ctrl+L         Tek sayfa
Ctrl+Shift+L   Karşılıklı sayfalar
Ctrl+Shift+B   Kitap görünümü
Ctrl+Shift+C   Sürekli
R              Saat yönünde döndür
Shift+R        Saat yönü tersine döndür

Gelişmiş:
F9             Menüyü göster/gizle
F6             Adres çubuğuna odaklan
Ctrl+K         Komut paleti
Ctrl+Shift+D   Hata ayıklama bilgisi
Ctrl+Alt+P     Yazdırma önizleme
```

---

# 📚 **Hızlı Referans**

### ⚡ **Kritik Komutlar ve Kısayollar**

### **Günlük Kullanım**

```
Dosya İşlemleri:
Ctrl+O    - Dosya aç
Ctrl+W    - Sekme kapat
Ctrl+R    - Yeniden yükle

Gezinme:
J/K       - Sayfa ileri/geri
Ctrl+G    - Sayfaya git
Home/End  - İlk/Son sayfa

Görüntüleme:
+/-       - Yakınlaştır/Uzaklaştır
Ctrl+0    - Sayfayı sığdır
F11       - Tam ekran

Arama:
Ctrl+F    - Ara
F3        - Sonrakini bul
```

### **Gelişmiş Özellikler**

```
Sistem Entegrasyonu:
-register-for-pdf     - PDF ilişkilendirme
-install-browser-plugin - Tarayıcı entegrasyonu
-extract-text         - Metin çıkarma

Hata Ayıklama ve Analiz:
-debug               - Hata ayıklama modu
-bench               - Performans testi
-stress-test         - Kararlılık testi
```

# 🐛 **Sorun Giderme ve Teknik Destek**

### ⚠️ **Yaygın Sorunlar ve Çözümleri**

### **Başlatma Sorunları**

```
Sorun: "Uygulama başlatılamadı" (Application failed to start)
Çözüm:
1. Yönetici olarak çalıştır
2. Windows Olay Görüntüleyicisini kontrol et
3. Antivirüsü geçici olarak devre dışı bırak
4. Yeni bir kopya indir
5. Ayarlar dosyasını temizle

Sorun: "Eksik DLL hataları" (Missing DLL errors)
Çözüm:
1. Visual C++ Redistributable yükle
2. Windows Update çalıştır
3. Sistem dosya denetleyicisi: sfc /scannow
4. Kayıt defteri temizliği
5. Temiz Windows kurulumu (ekstrem)

Sorun: Yavaş başlatma
Çözüm:
1. Windows Defender gerçek zamanlı taramayı devre dışı bırak
2. SumatraPDF'yi antivirüs istisnalarına ekle
3. Zararlı yazılım tarama
4. Başlangıç programlarını devre dışı bırak
5. SSD depolama kullan
```

### **Dosya Açma Sorunları**

```
Sorun: "PDF dosyası açılamıyor" (Cannot open PDF file)
Sorun Giderme:
1. Dosya bozulmasını kontrol et: Tarayıcıda aç
2. Farklı PDF ile test et
3. Dosya izinlerini kontrol et
4. PDF ilişkilendirmelerini geçici olarak devre dışı bırak
5. SumatraPDF ayarlarını sıfırla

Sorun: "Metin karışık görünüyor" (Text appears garbled)
Çözümler:
1. Yazı tipi kurulum sorunları
2. Kodlama problemleri
3. Bozuk PDF yazı tipleri
4. Bölgesel ayarlar
5. Dil paketi kurulumu

Sorun: "Resimler görüntülenmiyor" (Images not displaying)
Düzeltmeler:
1. Grafik sürücü güncellemesi
2. DirectX kurulumu
3. Renk profili sorunları
4. Donanım hızlandırmayı devre dışı bırak
5. Sistem grafik ayarları
```

### **Performans Sorunları**

```
Problem: High memory usage
Optimization:
1. Close unused tabs
2. Clear document cache
3. Reduce page preloading
4. Disable background loading
5. Restart application regularly

Problem: Slow page rendering
Solutions:
1. Graphics driver update
2. Hardware acceleration toggle
3. Reduce zoom level
4. Close other applications
5. Increase virtual memory

Problem: Search is slow
Improvements:
1. Index-based search for large docs
2. Reduce search scope
3. Use exact phrase matching
4. Close other documents
5. Restart with fresh cache
```

## 🔧 **Gelişmiş Sorun Giderme**

### **Debug Modu ve Günlük Kaydı**

```bash
# Debug information
SumatraPDF.exe -debug

# Verbose logging
SumatraPDF.exe -log

# Memory usage analysis
SumatraPDF.exe -mem-trace

# Crash dump generation
SumatraPDF.exe -crash-handler

# Performance profiling
SumatraPDF.exe -profile
```

### **Sistem Entegrasyonu Sorunları**

```
Registry Fixes:
1. Default PDF association reset
2. Context menu registration
3. Shell extension registration
4. File type icon restoration
5. Browser plugin conflicts

Command Line Repairs:
# Re-register file associations
SumatraPDF.exe -register-for-pdf

# Install browser plugin
SumatraPDF.exe -install-browser-plugin

# Repair installation
SumatraPDF-install.exe /REPAIR

# Clean uninstall
SumatraPDF-install.exe /UNINSTALL /S
```

---

# 🔗 **Temel Bağlantılar**

### **Resmi Kaynaklar**

- **Ana Site**: [sumatrapdfreader.org](https://www.sumatrapdfreader.org/)
- **İndirme**: [sumatrapdfreader.org/download](https://www.sumatrapdfreader.org/download-free-pdf-viewer)
- **GitHub**: [github.com/sumatrapdfreader/sumatrapdf](https://github.com/sumatrapdfreader/sumatrapdf)