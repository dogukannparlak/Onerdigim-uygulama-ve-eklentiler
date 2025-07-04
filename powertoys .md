# powertoys

# Microsoft PowerToys

## 🎯 Genel Bakış

### Araç Hakkında

Microsoft PowerToys, Windows kullanıcıları için geliştirilmiş ücretsiz ve açık kaynaklı bir sistem araçları koleksiyonudur. Microsoft tarafından resmi olarak desteklenen PowerToys, günlük iş akışınızı hızlandıran ve Windows deneyiminizi geliştiiren güçlü araçlar sunar.

### 🚀 Kurulum ve Başlangıç

### Kurulum Yöntemleri

### 1️⃣ Microsoft Store (Önerilen)

1. Microsoft Store’u açın
2. “PowerToys” araması yapın
3. **Microsoft PowerToys** uygulamasını seçin
4. **Al** butonuna tıklayın

### 2️⃣ Winget ile Kurulum

```
winget install Microsoft.PowerToys
```

### 3️⃣ GitHub Releases

1. https://github.com/microsoft/PowerToys/releases adresine gidin
2. En son sürümü indirin: `PowerToysUserSetup-x.x.x-x64.exe`
3. İndirilen dosyayı çalıştırın

### 4️⃣ Chocolatey ile Kurulum

```
choco install powertoys
```

### ⚙️ İlk Yapılandırma

Kurulum sonrası PowerToys Settings uygulamasını açın:
- **Başlat Menüsü** → “PowerToys Settings”
- **System Tray** → PowerToys simgesi → Settings

---

## 🧩 Araçlar

## 📌 Always On Top - Herzaman Üstte

### 🎯 Özellik Açıklaması

Always On Top, seçili pencereleri diğer tüm pencerelerin üstünde tutmanızı sağlar. Referans dokümanlar, hesap makinesi veya not defteri gibi sürekli görünür olmasını istediğiniz uygulamalar için idealdir.

### 🔧 Aktivasyon ve Kullanım

| Eylem | Kısayol | Açıklama |
| --- | --- | --- |
| **Aktifleştir/Deaktifleştir** | `Win + Ctrl + T` | Aktif pencereyi üstte tut |
| **Görsel İndikatör** | Renkli çerçeve | Üstte tutulan pencereleri ayırt et |

### ⚙️ Yapılandırma Seçenekleri

| Ayar | Açıklama | Önerilen |
| --- | --- | --- |
| **Activation Shortcut** | Kısayol tuşu kombinasyonu | `Win + Ctrl + T` |
| **Frame Enabled** | Görsel çerçeve göster | ✅ Aktif |
| **Frame Color** | Çerçeve rengi | Mavi (varsayılan/isteğe göre değiştirilebilir) |
| **Frame Thickness** | Çerçeve kalınlığı | 5px(isteğe göre değiştirilebilir) |
| **Sound Enabled** | Ses bildirimi | ✅ Aktif |

---

## 🎨 Command Palette - Komut Paleti

### 🎯 Özellik Açıklaması

Command Palette (PowerToys Run), macOS Spotlight veya Linux dmenu benzeri hızlı uygulama başlatıcı ve sistem komut aracıdır. Dosya arama, hesaplama, sistem komutları ve plugin desteği sunar.

### 🔧 Aktivasyon ve Temel Kullanım

| Eylem | Kısayol | Açıklama |
| --- | --- | --- |
| **Paleti Aç** | `Alt + ctr + Space`  (ayarlardan değiştirebilrsiniz) | Command palette’i aç |
| **Uygulama Başlat** | `program_adı` + Enter | Uygulama ara ve çalıştır |
| **Dosya Ara** | `dosya_adı` | Sistem genelinde dosya ara |

### 🧩 Plugin Özellikleri

Kullanılacak Pluginleri etkinleştirme, devre dışı bırakma veya özelleştirme işlemlerini Ayarlar menüsü aracılığıyla yapılandırabilirsiniz.

### Hesap Makinesi Plugin

```
Örnekler:
= 15 * 23
= sqrt(144)
= log(100)
= 2^8
```

### Sistem Komutları

| Komut | Açıklama | Kullanım |
| --- | --- | --- |
| `shutdown` | Sistemi kapat | `shutdown` + Enter |
| `restart` | Sistemi yeniden başlat | `restart` + Enter |
| `lock` | Sistemi kilitle | `lock` + Enter |
| `sleep` | Uyku moduna geç | `sleep` + Enter |

### Registry Editor

```
Örnekler:
reg HKEY_CURRENT_USER
reg SOFTWARE
```

---

## 🖱️ Find My Mouse - Faremi Bul

### 🎯 Özellik Açıklaması

Find My Mouse, özellikle çoklu monitör kurulumlarında fare imlecini bulmayı kolaylaştıran bir araçtır. Ctrl tuşuna çift basarak fare konumunu vurgular.

### 🔧 Aktivasyon ve Kullanım

| Eylem | Kısayol | Açıklama |
| --- | --- | --- |
| **Fare Bul** | `Ctrl + Ctrl` (çift bas) | Fare konumunu vurgula |
| **Sürekli Aktivasyon** | `Ctrl` (basılı tut) | Sürekli vurgulama |

### ⚙️ Yapılandırma Seçenekleri

| Ayar | Açıklama | Değer Aralığı |
| --- | --- | --- |
| **Activation Method** | Aktivasyon yöntemi | Çift tıklama/Basılı tutma |
| **Background Color** | Arka plan rengi | Özelleştirilebilir |
| **Spotlight Radius** | Spot ışığı yarıçapı | Özelleştirilebilir |
| **Animation Duration** | Animasyon süresi | Özelleştirilebilir |
| **Exclude Apps** | Dışlanacak uygulamalar | Özelleştirilebilir |

## 🔦 Mouse Highlighter - Fare Vurgulayıcı

### 🎯 Özellik Açıklaması

Mouse Highlighter, sunumlar ve eğitimler sırasında fare hareketlerini vurgulamak için kullanılan profesyonel bir araçtır. Fare çevresinde görsel efektler oluşturur.

### 🔧 Aktivasyon ve Kullanım

| Eylem | Kısayol | Açıklama |
| --- | --- | --- |
| **Vurgulama Başlat** | `Win + Shift + H` | Mouse highlighter aktif et |
| **Vurgulama Durdur** | `Win + Shift + H` | Mouse highlighter kapat |
| **Sol Tık Vurgusu** | Sol fare tık | Tık noktasını vurgula |
| **Sağ Tık Vurgusu** | Sağ fare tık | Farklı renkte vurgu |

### ⚙️ Görsel Ayarlar

### Spot Işığı Ayarları

| Ayar | Açıklama | Değer Aralığı |
| --- | --- | --- |
| **Spotlight Radius** | Spot yarıçapı | 20 - 100px |
| **Opacity** | Şeffaflık | 0.1 - 1.0 |
| **Color** | Renk | Özelleştirilebilir |
| **Fade Delay** | Solma gecikmesi | 0 - 5 saniye |

### Tık Vurgulama Ayarları

| Ayar | Açıklama | Seçenekler |
| --- | --- | --- |
| **Left Click Color** | Sol tık rengi | Sarı (Özelleştirilebilir) |
| **Right Click Color** | Sağ tık rengi | Kırmızı (Özelleştirilebilir) |
| **Fade Duration** | Solma süresi | Özelleştirilebilir |
| **Radius** | Vurgu yarıçapı | Özelleştirilebilir |

---

## 👁️ Preview Pane - Göz Atma

### 🎯 Özellik Açıklaması

Preview Pane, Windows File Explorer’da dosyaları açmadan önizleme yapmanızı sağlar. Görüntü, video, metin ve kod dosyaları için gelişmiş önizleme desteği sunar.

---

## ⌨️ Quick Accent - Hızlı Aksan

### 🎯 Özellik Açıklaması

Quick Accent, aksan karakterlerini (é, ñ, ü gibi) hızlı bir şekilde yazmayı sağlar. Çoklu dil desteği ile international karakter girişini kolaylaştırır.

### 🔧 Aktivasyon ve Kullanım

| Eylem | Kısayol | Açıklama |
| --- | --- | --- |
| **Hızlı Seçim** | `Harf + Boşluk` | En yaygın aksanı ekle |

### ⚙️ Yapılandırma Seçenekleri

| Ayar | Açıklama | Seçenekler |
| --- | --- | --- |
| **Activation Key** | Aktivasyon tuşu | Left/Right/Both Shift |
| **Input Time** | Basılı tutma süresi | 300-1000ms |
| **Excluded Apps** | Dışlanacak uygulamalar | Oyunlar |
| **Toolbar Position** | Menü konumu | Above/Below/Center |

### 💡 Kullanım İpuçları

### Hızlı Yaygın Aksanlar

```
e + Space = é (Fransızca için)
a + Space = á (İspanyolca için)
c + Space = ç (Türkçe için)
n + Space = ñ (İspanyolca için)
```

## 📝 Text Extractor - Metin Ayıklayıcı

### 🎯 Özellik Açıklaması

Text Extractor (PowerToys OCR), ekrandaki herhangi bir görüntüden metin çıkarmanızı sağlayan güçlü bir Optical Character Recognition (OCR) aracıdır. Modern AI tabanlı metin tanıma teknolojisi kullanır.

### 🔧 Aktivasyon ve Kullanım

| Eylem | Kısayol | Açıklama |
| --- | --- | --- |
| **Metin Çıkarma** | `Win + Shift + T` (Özelleştirilebilir) | OCR modunu başlat |
| **Alan Seçimi** | Fare ile seç  | Metin alanını seç |
| **Otomatik Kopyalama** | Seçim tamamlandığında | Panoya kopyalar |

### Performans Artırma

```
Optimize Edilmiş Kullanım:
1. Sadece metin alanını seç
2. Gereksiz grafikleri dahil etme
3. Yüksek kontrast kullan
4. Düz arka plan tercih et
```

---

## 🎨 Color Picker - Renk Seçici

### 🎯 Özellik Açıklaması

Color Picker, ekrandaki herhangi bir renkten HEX, RGB, HSL kodu çıkarmanızı sağlayan profesyonel bir eyedropper aracıdır. Tasarımcılar ve geliştiriciler için vazgeçilmez bir araçtır.

### 🔧 Aktivasyon ve Kullanım

| Eylem | Kısayol | Açıklama |
| --- | --- | --- |
| **Renk Seçici Aç** | `Win + Shift + C` | Color picker modunu başlat |
| **Renk Seç** | `Sol Tık` | Seçili rengi kopyala |
| **Zoom Modu** | `Ctrl + Scroll` | Hassas seçim için yakınlaştır |
| **İptal** | `Esc` | Renk seçimi iptal et |

### 🎨 Renk Formatları

### Desteklenen Formatlar

| **Format** | **Açıklama** | **Örnek** | **Kullanım Alanı** |
| --- | --- | --- | --- |
| **HEX** | Hexadecimal | `#FF5733` | Web tasarım |
| **RGB** | Red Green Blue | `rgb(255, 87, 51)` | CSS, kod |
| **HSL** | Hue Saturation Lightness | `hsl(9, 100%, 60%)` | Tasarım |
| **HSV** | Hue Saturation Value | `hsv(9, 80%, 100%)` | Grafik yazılım |
| **CMYK** | Cyan Magenta Yellow Black | `cmyk(0, 66, 80, 0)` | Baskı tasarımı |
| **VEC4** | Vector 4 | `(1.0, 0.34, 0.2, 1.0)` | Oyun geliştirme |
| **HSB** | Hue Saturation Brightness *(HSV eşdeğeri)* | `hsb(9, 80%, 100%)` | Grafik yazılım, dijital sanat |
| **HSI** | Hue Saturation Intensity | `hsi(9°, 0.88, 0.73)` | Görüntü işleme, analiz |
| **HWB** | Hue Whiteness Blackness | `hwb(9, 30%, 20%)` | CSS4, web tasarım |
| **NCol** | Natural Color System | `NCS S 1080-Y70R` | İç mimarlık, renk teorisi |
| **CIELAB** | CIE L*a*b* renk uzayı | `lab(53.2, 80.1, 67.2)` | Renk bilimi, baskı teknolojisi |
| **CIEXYZ** | CIE 1931 renk uzayı | `xyz(0.41, 0.22, 0.02)` | Renk dönüştürme, endüstri |
| **Decimal** | Ondalık sayılarla ifade edilen renkler | `16729395` | Yazılım, veritabanı işlemleri |
| **HEX int** | Tam sayı olarak kullanılan HEX | `0xFF5733` | Kodlama, düşük seviye işlemler |

### ⚙️ Yapılandırma Seçenekleri

### Genel Ayarlar

| Ayar | Açıklama | Seçenekler |
| --- | --- | --- |
| **Default Color Format** | Varsayılan format | HEX, RGB, HSL vb. |
| **Show Color Name** | Renk ismini göster | Özelleştirilebilir |
| **Copy to Clipboard** | Otomatik kopyalama | Özelleştirilebilir |
| Kendi formatını oluşturabilirsin | - | Özelleştirilebilir |

## ➕ New+ - Gelişmiş Yeni Dosya

### 🎯 Özellik Açıklaması

New+, Windows sağ tık menüsüne gelişmiş “Yeni Dosya” seçenekleri ekler. Geliştiriciler ve power user’lar için önceden tanımlanmış şablonlarla hızlı dosya oluşturma imkanı sunar.

### 🔧 Aktivasyon ve Kullanım

| Eylem | Konum | Açıklama |
| --- | --- | --- |
| **Sağ Tık Menüsü** | Desktop/Explorer | “New+” seçeneğini kullan |
| **Şablon Seçimi** | Alt menü | İstenen dosya türünü seç |
| **Hızlı Oluşturma** | Çift tık | Dosyayı oluştur ve aç |

### ⚙️ Özel Şablon Ekleme

### Şablon Klasörü

PowerToys şablonları şu konumda saklar:

```
%USERPROFILE%\AppData\Local\Microsoft\PowerToys\NewPlus\Templates
```

### Yeni Şablon Oluşturma

1. **Template klasörüne** gidin
2. **Yeni dosya** oluşturun (örn: `template.jsx`)
3. **İçeriği** tanımlayın:

```jsx
// React Component Templateimport React from 'react';const ComponentName = () => {
  return (
    <div>      <h1>Hello World</h1>    </div>  );};export default ComponentName;
```

1. **PowerToys Settings** → **New+** → **Refresh Templates**

### Template Değişkenleri

| Değişken | Açıklama | Örnek |
| --- | --- | --- |
| `{{filename}}` | Dosya adı | `MyComponent` |
| `{{date}}` | Mevcut tarih | `2024-01-15` |
| `{{time}}` | Mevcut saat | `14:30:25` |
| `{{author}}` | Kullanıcı adı | `JohnDoe` |

### 💡 Kullanım Örnekleri

### Web Geliştirme Workflow

```
1. Proje klasöründe sağ tık
2. New+ → HTML Page
3. New+ → CSS Style
4. New+ → JavaScript
5. Hızlı prototip hazır!
```

### DevOps Workflow

```
1. Proje root'da sağ tık
2. New+ → Docker File
3. New+ → YAML Config (docker-compose)
4. New+ → ENV Variables
5. Container ortamı hazır!
```

### Dokümantasyon Workflow

```
1. Docs klasöründe sağ tık
2. New+ → README.md
3. New+ → Changelog.md
4. New+ → License.md
5. Proje dokümantasyonu hazır!
```

---

## 🪟 FancyZones - Pencere Düzenleme

### 🎯 Özellik Açıklaması

FancyZones, Windows’un pencere yönetimi özelliklerini geliştirir ve özelleştirilebilir pencere düzenleri (layouts) oluşturmanızı sağlar. Çoklu monitör kurulumları için optimize edilmiş bu araç, productivity’nizi önemli ölçüde artırır.

### 🔧 Aktivasyon ve Kullanım

| Eylem | Kısayol | Açıklama |
| --- | --- | --- |
| **Zone Editor Aç** | `Win + Shift + \` | Layout düzenleyicisini aç |
| **Pencere Taşıma** | `Shift + Sürükle` | Pencereyi zone’lara yerleştir |
| **Zone Highlight** | `Shift` (basılı tut) | Mevcut zone’ları göster |
| **Snap Override** | `Shift + Win + Ok` | Zone’lar arası geçiş |

### 🎨 Hazır Layout Şablonları

### Tek Monitör Layouts

| Layout | Açıklama | Kullanım Senaryosu |
| --- | --- | --- |
| **Focus** | Tek büyük alan | Tam ekran çalışma |
| **Columns** | 2-3 dikey sütun | Kod editörü + terminal |
| **Rows** | 2-3 yatay satır | Tarayıcı + referans |
| **Grid** | 2x2, 3x3 ızgara | Çoklu uygulama |
| **Priority Grid** | Ana + yardımcı alanlar | Ana çalışma + yan görevler |

### Çoklu Monitör Layouts

| Konfigürasyon | Layout Önerisi | Verimlilik |
| --- | --- | --- |
| **Geliştirici Setup** | Kod (Ana) + Dokümantasyon (Yan) | %40 artış |
| **Tasarımcı Setup** | Tasarım (Ana) + Araçlar (Yan) | %35 artış |
| **Trader Setup** | Grafikler (Ana) + Veriler (Yan) | %50 artış |

### ⚙️ Özel Layout Oluşturma

### Layout Editor Kullanımı

1. **Win + Shift + `** ile editörü açın
2. **Monitor** seçin (çoklu monitör için)
3. **Template** seçin veya **Create new layout**
4. **Zone’ları** çizin ve ayarlayın
5. **Save & Apply** ile uygulayın

### Zone Ayarlama İpuçları

| Ayar | Açıklama | Önerilen |
| --- | --- | --- |
| **Zone Padding** | Zone’lar arası boşluk | 8-16px |
| **Zone Overlap** | Üst üste binme | %5-10 |
| **Snap Sensitivity** | Yakalama hassasiyeti | Medium |
| **Show Zones** | Zone görünürlüğü | Shift basılı |

### 🔧 Gelişmiş Özellikler

### Zone Behaviors

| Davranış | Açıklama | Ayar |
| --- | --- | --- |
| **Override Windows Snap** | Varsayılan snap’i geçersiz kıl | ✅ Önerilen |
| **Move Windows Between Zones** | Zone’lar arası taşıma | ✅ Aktif |
| **Restore Original Size** | Orijinal boyuta dönüş | ⚙️ İhtiyaçsal |
| **Multi-Monitor Spanning** | Çoklu monitör geçişi | ✅ Aktif |

### Hotkeys ve Kısayollar

```
Win + Left/Right → Zone değiştir
Win + Up → Maksimize (zone içinde)
Win + Down → Minimize
Shift + Sürükle → Zone'a yerleştir
```

---

## 🏷️ PowerRename - Toplu Yeniden Adlandırma

### 🎯 Özellik Açıklaması

PowerRename, dosya ve klasörleri toplu olarak yeniden adlandırmanızı sağlayan güçlü bir araçtır. Regex desteği, preview fonksiyonu ve batch processing ile karmaşık adlandırma işlemlerini kolaylaştırır.

### 🔧 Aktivasyon ve Kullanım

| Eylem | Konum | Açıklama |
| --- | --- | --- |
| **PowerRename Aç** | Sağ tık menüsü | Seçili dosyalarda “PowerRename” |
| **Toplu Seçim** | Ctrl+A veya Shift | Çoklu dosya seçimi |
| **Preview** | Otomatik | Değişiklik önizlemesi |

### 🔧 Temel İşlemler

### Basit Metin Değiştirme

| İşlem | Search | Replace | Sonuç |
| --- | --- | --- | --- |
| **Uzantı Değiştirme** | `.jpg` | `.png` | image.jpg → image.png |
| **Prefix Ekleme** | `^` | `backup_` | file.txt → backup_file.txt |
| **Suffix Ekleme** | `$` | `_old` | file.txt → file_old.txt |
| **Boşluk Kaldırma** |  | `_` | my file.txt → my_file.txt |

### Regex ile Gelişmiş İşlemler

| İşlem | Regex Pattern | Replace | Örnek |
| --- | --- | --- | --- |
| **Tarihleri Düzenle** | `(\d{4})-(\d{2})-(\d{2})` | `$3.$2.$1` | 2024-01-15 → 15.01.2024 |
| **Sayı Sıralaması** | `(.+)` | `$1_(##)` | file → file_01, file_02 |
| **Büyük Harf** | `([a-z])` | `\U$1` | filename → FILENAME |
| **CamelCase** | `[ _]([a-z])` | `\U$1` | my_file → MyFile |

### 💡 Pratik Kullanım Örnekleri

### Fotoğraf Düzenleme

```
Problem: IMG_001.jpg, IMG_002.jpg, IMG_003.jpg
Hedef: 2024_Tatil_001.jpg, 2024_Tatil_002.jpg

Search: IMG_(\d+)
Replace: 2024_Tatil_$1
```

### Kod Dosyası Organizasyonu

```
Problem: component.js, component.css, component.html
Hedef: MyComponent.js, MyComponent.css, MyComponent.html

Search: component
Replace: MyComponent
```

---

## 🖼️ Image Resizer - Görüntü Boyutlandırma

### 🎯 Özellik Açıklaması

Image Resizer, görüntüleri hızlı ve toplu olarak yeniden boyutlandırmanızı sağlayan kullanıcı dostu bir araçtır. Web yayını, email ekleri ve storage optimizasyonu için idealdir.

### 🔧 Aktivasyon ve Kullanım

| Eylem | Konum | Açıklama |
| --- | --- | --- |
| **Resize Images** | Sağ tık menüsü | Seçili görüntülerde |
| **Toplu Seçim** | Ctrl+A | Klasörteki tüm resimler |
| **Hızlı İşlem** | Çift tık | Preset boyutlarla |

### 📏 Preset Boyutlar

### Sosyal Medya Optimizasyonu

| Platform | Boyut | Açıklama | Kullanım |
| --- | --- | --- | --- |
| **Instagram Post** | 1080x1080 | Kare format | Sosyal paylaşım |
| **Instagram Story** | 1080x1920 | Dikey format | Story içeriği |
| **Facebook Cover** | 1200x630 | Yatay banner | Kapak fotoğrafı |
| **Twitter Header** | 1500x500 | Banner format | Profil başlığı |
| **LinkedIn Post** | 1200x627 | Profesyonel | İş içeriği |

### Web ve E-posta

| Amaç | Boyut | Kalite | Dosya Boyutu |
| --- | --- | --- | --- |
| **Email Eki** | 800x600 | 80% | ~200KB |
| **Web Galeri** | 1200x800 | 90% | ~500KB |
| **Thumbnail** | 200x150 | 70% | ~50KB |
| **Avatar** | 256x256 | 90% | ~100KB |

---

## ⌨️ Keyboard Manager - Tuş Yönetimi

### 🎯 Özellik Açıklaması

Keyboard Manager, klavye tuşlarını yeniden atamanızı ve özel kısayollar oluşturmanızı sağlar. Ergonomi iyileştirme, international layout’lar ve özel workflow’lar için idealdir.

### 🔧 İki Ana Fonksiyon

### 1. Key Remapping (Tuş Yeniden Atama)-örnek

| Orijinal Tuş | Yeni Atama |
| --- | --- |
| **Caps Lock** | **Escape** |
| **Right Alt** | **Right Ctrl** |
| **Print Screen** | **Windows Key** |
| **Insert** | **Delete** |

### 2. Shortcut Remapping (Kısayol Yeniden Atama)-örnek

| Orijinal Kısayol | Yeni Atama |
| --- | --- |
| **Ctrl+C** | **Ctrl+Shift+C** |
| **Alt+Tab** | **Win+Tab** |
| **Win+L** | **Ctrl+Alt+L** |

## 🔒 File Locksmith - Dosya Çilingiri

### 🎯 Özellik Açıklaması

File Locksmith, “dosya kullanımda” hatalarını çözmek için hangi sürecin dosyayı kilitlediğini gösterir. Dosya silme, taşıma ve düzenleme işlemlerinde karşılaşılan sorunları hızlıca çözer.

### 🔧 Aktivasyon ve Kullanım

| Eylem | Konum | Açıklama |
| --- | --- | --- |
| **What’s using this file?** | Sağ tık menüsü | Dosya kilit analizi |
| **Bulk Analysis** | Çoklu seçim | Toplu dosya kontrolü |
| **Process Details** | Ana pencere | Detaylı süreç bilgisi |

### 💡 Kullanım Senaryoları

### Yaygın “Dosya Kullanımda” Sorunları

| Senaryo | Sebep | Çözüm |
| --- | --- | --- |
| **Video dosyası silinmiyor** | Media player açık | Player’ı kapat |
| **Log dosyası kopyalanmıyor** | Servis yazıyor | Servisi durdur |
| **Excel dosyası açılmıyor** | Arka planda Excel | Excel sürecini sonlandır |
| **Temp dosyalar silinmiyor** | Antivirus taraması | Antivirus’ü beklet |

---

---

## 🛠️ Diğer Yararlı Araçlar

PowerToys paketi içinde yukarıda detaylandırılan araçların yanında başka faydalı araçlar da bulunur:

### 🔧 Ek Araçlar

| Araç | Açıklama | Kısayol | Kullanım Alanı |
| --- | --- | --- | --- |
| **Shortcut Guide** | Windows kısayolları rehberi | `Win` (basılı tut) | Öğrenme ve hatırlama |
| **Screen Ruler** | Ekran cetveli ve ölçüm | `Win + Shift + M` | Tasarım ve geliştirme |
| **Hosts File Editor** | Hosts dosyası düzenleme | Settings’den | Ağ yönetimi |
| **Registry Preview** | Registry dosya önizleme | File Explorer | Sistem yönetimi |
| **Environment Variables** | Çevre değişkenleri | Settings’den | Geliştirme |

## 🔧 Sorun Giderme Araçları

### Tanı Komutları

PowerShell ile sistem kontrolü:

```powershell
# PowerToys süreçlerini kontrol et
Get-Process | Where-Object {$_.Name -like "*PowerToys*"}

# PowerToys servislerini kontrol et
Get-Service | Where-Object {$_.Name -like "*PowerToys*"}

# Event Log kontrol
Get-EventLog -LogName Application -Source "*PowerToys*" -Newest 10
```

### Sıfırlama ve Temizlik

```
# PowerToys ayarlarını sıfırla
%USERPROFILE%\AppData\Local\Microsoft\PowerToys\

# Geçici dosyaları temizle
%TEMP%\PowerToys\

# Registry temizlik (dikkatli kullanın)
HKEY_CURRENT_USER\Software\Microsoft\PowerToys
```

---