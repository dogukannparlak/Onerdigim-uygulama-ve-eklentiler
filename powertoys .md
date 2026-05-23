# ⚡ PowerToys

> **Kısa Açıklama:** Microsoft'un resmi Windows sistem araçları paketi; pencere yönetimi, hızlı başlatıcı, OCR, renk seçici ve onlarca yardımcı modül sunar.

0.9x · Windows 10/11 · MIT / ücretsiz · Sistem araçları

---

## 📌 Genel Bakış

PowerToys, Windows deneyimini güçlendiren ücretsiz ve açık kaynaklı bir araç koleksiyonudur. Microsoft tarafından resmi olarak desteklenir; [resmi dokümantasyonda](https://learn.microsoft.com/tr-tr/windows/powertoys/) **30 yardımcı program** listelenir. Pencere düzenleme, toplu yeniden adlandırma, ekrandan metin çıkarma, klavye yeniden eşleme gibi işlemleri ayrı uygulamalara gerek kalmadan tek pakette sunar. Her modül PowerToys Settings üzerinden ayrı ayrı açılıp kapatılabilir; **tüm modül kısayolları varsayılan değerlerdir ve istediğin tuş kombinasyonuna değiştirilebilir.**

> En güncel bilgi için [Microsoft PowerToys resmi sitesini](https://learn.microsoft.com/tr-tr/windows/powertoys) ve kurulu uygulamadaki **PowerToys Settings** ekranını kontrol et. Modül listesi, kısayollar ve ayar adları sürüme göre değişebilir.

---

## ✨ Öne Çıkan Özellikler

- **Modüler yapı** - İhtiyacın olan araçları aç, kullanmadıklarını kapat
- **Resmi Microsoft desteği** - Açık kaynak, düzenli güncelleme
- **Özelleştirilebilir kısayollar** - Her modülün aktivasyon tuşu Settings'ten değiştirilebilir; bu rehberdeki kısayollar yalnızca varsayılandır
- **Explorer entegrasyonu** - Sağ tık menüsü, önizleme paneli, toplu işlemler
- **Geliştirici dostu** - PowerRename, Color Picker, Keyboard Manager, Text Extractor
- **Ücretsiz** - Store, WinGet veya GitHub üzerinden kurulabilir

---

## 📥 İndirme ve Kurulum

### Yöntem 1: Microsoft Store ( Önerilen )

1. Microsoft Store'u aç
2. **PowerToys** ara
3. **Microsoft PowerToys** uygulamasını seç → **Al**

### Yöntem 2: WinGet (Terminal)

```powershell
winget install -e --id Microsoft.PowerToys
```

### Yöntem 3: UniGetUI

> UniGetUI açıkken arama çubuğuna **PowerToys** yaz ve kur.

### Yöntem 4: GitHub Releases

1. [github.com/microsoft/PowerToys/releases](https://github.com/microsoft/PowerToys/releases) adresine git
2. En son sürümü indir: `PowerToysUserSetup-x.x.x-x64.exe`
3. Kurulum dosyasını çalıştır

**Alternatif:** Chocolatey - `choco install powertoys`

---

## ⚙️ İlk Kurulum ve Önerilen Ayarlar

1. **PowerToys Settings aç:** Başlat menüsü → **PowerToys Settings** veya sistem tepsisindeki PowerToys simgesi → Settings
2. **Kısayolları gözden geçir:** Her modülde **Activation shortcut** alanından varsayılan tuşları kontrol et; çakışma varsa veya alışkanlığına uymuyorsa **değiştir**
3. **Başlangıçta çalıştır:** Settings → General → **Run at startup** açık bırak (önerilen)

> 💡 Kurulum sonrası Windows yeniden başlatma gerekmez. Kısayol değiştirdiğinde kaydetmen yeterli - yeni tuş kombinasyonu anında geçerli olur.

---

## 🚀 Temel Kullanım

### Modül yönetimi

1. PowerToys Settings'i aç
2. Sol menüden modülü seç → **Enable** ile aç/kapat
3. Modül ayarlarını yapılandır → değişiklikler çoğunlukla anında uygulanır

### ⌨️ Kısayolları özelleştirme

Bu rehberde geçen tüm kısayollar (`Win + Shift + C`, `Win + Ctrl + T` vb.) **varsayılan değerlerdir** - PowerToys'ta sabit değildir; her modül için farklı bir kombinasyon atayabilirsin. Komut Paleti'nde ayar adı **Etkinleştirme tuşu** olarak geçer.

1. PowerToys Settings → ilgili modülü seç (örn. **Color Picker**, **Always on top**)
2. **Activation shortcut** (veya **Shortcut**) alanına tıkla
3. İstediğin tuş kombinasyonuna bas → **Save** / **Apply**


| Durum                                | Ne yapmalısın?                                  |
| ------------------------------------ | ----------------------------------------------- |
| Başka uygulama aynı tuşu kullanıyor  | Modül ayarından farklı bir kısayol ata          |
| Varsayılan sana uymuyor              | Alıştığın kombinasyona değiştir                 |
| Kısayolu tamamen kapatmak istiyorsan | İlgili alanı temizle veya modülü **Disable** et |


> 💡 **Keyboard Manager** ile PowerToys kısayollarını değil, sistem genelindeki tuş ve kısayol eşlemelerini değiştirirsin - ikisi farklı katmandır.

### Settings alanları


| Sekme / Alan      | İşlev                                  |
| ----------------- | -------------------------------------- |
| **General**       | Başlangıçta çalıştır, güncelleme, tema |
| **Modül listesi** | Her aracı ayrı ayrı etkinleştir        |
| **Dashboard**     | Kurulu modüllerin özeti                |
| **Sistem tepsi**  | PowerToys simgesi ve bildirimler       |


### Güncelleme

- Otomatik: Settings → General → **Automatic updates**
- Manuel: Settings → General → **Check for updates** veya GitHub Releases

---

## 🔌 Modüller

PowerToys paketinde 30 modül vardır; bu rehberde kullandığım **16 modül** kategori sırasıyla anlatılır. Settings'te modül adı İngilizce veya Türkçe görünebilir - her başlıkta ikisi birlikte verilmiştir.

#### İçindekiler

**Sistem Araçları**

- [1. Command Palette - Komut Paleti](#arac-1)
  - Spotlight benzeri hızlı başlatıcı; uygulama, dosya ve komut araması yapar.
- [2. Color Picker - Renk Seçici](#arac-2)
  - Ekrandan renk seçip HEX, RGB, HSL vb. kodları panoya kopyalar.
- [3. Light Switch - Işık Düğmesi](#arac-3)
  - Günün saatine göre Windows açık/koyu temasını otomatik değiştirir.
- [4. Text Extractor - Metin Ayıklayıcısı](#arac-4)
  - Ekrandaki görüntüden OCR ile metin çıkarıp panoya kopyalar.

**Pencere Oluşturma ve Düzenle**

- [5. Always On Top - Her Zaman Üstte](#arac-5)
  - Seçili pencereyi diğer tüm pencerelerin üstünde sabitler.
- [6. Crop And Lock - Kırp ve Kilitle](#arac-6)
  - Uygulama penceresinin bir bölümünü kırparak küçük pencere veya küçük resim oluşturur.
- [7. FancyZones - FancyZones](#arac-7)
  - Özel bölge düzenleriyle pencere yönetimi ve sürükleyerek yaslama sağlar.
- [8. Grab And Move - Yakala ve Taşı](#arac-8)
  - Değiştirici tuş + sürükleyerek pencere taşıma ve yeniden boyutlandırma yapar.

**Giriş ve Çıkış**

- [9. Keyboard Manager - Klavye Yöneticisi](#arac-9)
  - Klavye tuşlarını ve kısayol kombinasyonlarını yeniden eşler.
- [10. Mouse utilities - Fare Yardımcı Programları](#arac-10)
  - İmleç bulma, tıklama vurgulama, uzun mesafe atlama ve nişangah araçlarını bir arada sunar.
- [11. Quick Accent - Hızlı Aksan](#arac-11)
  - Harf basılı tut + Space ile é, ñ, ü, ç gibi aksanlı karakterleri hızlı yazar.

**Dosya Yönetimi**

- [12. File Explorer add-ons - Dosya Gezgini Eklentileri](#arac-12)
  - Explorer'da SVG, PDF, Markdown ve kaynak kod için önizleme bölmesi ve küçük resim desteği ekler.
- [13. File Locksmith - Dosya Çilingiri](#arac-13)
  - “Dosya kullanımda” hatasında hangi sürecin dosyayı kilitlediğini gösterir.
- [14. Image Resizer - Resim Boyutlandırıcı](#arac-14)
  - Explorer sağ tık menüsünden görüntüleri hızlı ve toplu olarak yeniden boyutlandırır.
- [15. Peek - Gözatma](#arac-15)
  - Explorer'da dosyayı uygulama açmadan kısayolla hızlı önizler.
- [16. PowerRename - PowerRename](#arac-16)
  - Toplu dosya/klasör yeniden adlandırma; regex ve önizleme destekli.

> ⚠️ **Kısayol notu:** Aşağıdaki tablolarda **Varsayılan kısayol** sütunu Microsoft'un önerdiği tuşları gösterir. Hepsi **PowerToys Settings → [modül] → Activation shortcut** üzerinden değiştirilebilir.

---

### Sistem Araçları

<a id="arac-1"></a>

### 🎨 1- Command Palette - Komut Paleti

> Eski adı **PowerToys Run**; işlev aynıdır.

macOS Spotlight veya Linux dmenu benzeri hızlı başlatıcı ve komut merkezi. Uygulama arama, dosya bulma, hesaplama, sistem komutları ve onlarca yerleşik uzantı sunar. PowerToys Settings'te **Command Palette** / **Komut Paleti** adıyla geçer (eski adı: PowerToys Run).

#### Ne sağlar?

- **Hızlı başlatma** - Uygulama adı yaz → Enter
- **Uzantı tabanlı komutlar** - Dosya arama, hesap makinesi, WinGet, kayıt defteri, pano geçmişi vb.
- **Özelleştirilebilir arayüz** - Tema, akrilik arka plan, renk tonu, animasyonlar
- **Çoklu monitör** - Paleti fare imlecinin bulunduğu monitörde açabilirsin
- **Yuva (önizleme)** - Komutlara hızlı erişim için isteğe bağlı araç çubuğu
- **Store / WinGet uzantıları** - Ek uzantılar indirilebilir

#### Nasıl kullanılır?

1. **Etkinleştirme tuşu**na bas (Settings → **Komut Paleti** → **Genel** → **Etkinleştirme tuşu**; kalem simgesiyle değiştirilebilir)
2. Komut veya uygulama adı yaz
3. Enter ile çalıştır; ok tuşları veya fare ile seç

Tuş kombinasyonu tamamen sana bağlıdır - rehberde sabit bir kısayol varsayılmaz.

#### Ayarlar sekmesi

Settings → **Command Palette** / **Komut Paleti** penceresinde dört sekme vardır:

##### Genel

**Etkinleştirme**


| Ayar                                                                | Ne işe yarar?                                                                                                  |
| ------------------------------------------------------------------- | -------------------------------------------------------------------------------------------------------------- |
| **Etkinleştirme tuşu**                                              | Paleti açan tuş - **değiştirilebilir**                                                                         |
| **Düşük düzeyli klavye kancası kullanın**                           | Klavye sorunlarında dene; yükseltilmiş pencereden tetiklenince odaklanma sorununu giderebilir                  |
| **Tam ekran modunda kısayolları yoksay**                            | Tam ekranda yanlışlıkla açılmayı önler                                                                         |
| **Sistem buluşsal olarak tam ekranı algıladığında kısayolu yoksay** | Windows tam ekran veya Sunu Ayarları algıladığında devre dışı kalır (NVIDIA katmanı vb. yanlış tetikleyebilir) |
| **Kısayol tuşlarına hızlı basarak geçişe izin ver**                 | Tam ekran korumasını atlamak için 2 saniye içinde etkinleştirme tuşuna 3 kez bas                               |
| **Otomatik olarak ana sayfaya dön**                                 | Palet kapalıyken belirli süre sonra giriş sayfasına dön (Asla / süre seçenekleri)                              |
| **Etkinleştirildiğinde aramayı vurgula**                            | Açılışta önceki arama metnini seçer                                                                            |
| **Önceki sorguyu tut**                                              | Yeniden açıldığında son arama metnini korur                                                                    |
| **Tercih edilen monitör konumu**                                    | Çoklu monitörde paletin nerede açılacağı (örn. fare imleciyle izle)                                            |


**Davranış**


| Ayar                                | Ne işe yarar?                                     |
| ----------------------------------- | ------------------------------------------------- |
| **Sistem tepsisi simgesini göster** | Komut Paleti simgesini bildirim alanında gösterir |


**Geliştiriciler için**


| Ayar                                        | Ne işe yarar?                                                |
| ------------------------------------------- | ------------------------------------------------------------ |
| **Dışarıdan yeniden yüklemeyi etkinleştir** | `x-cmdpal://reload` ile uzantıları dışarıdan yeniden yükleme |


##### Kişiselleştirme


| Ayar                               | Ne işe yarar?                                                       |
| ---------------------------------- | ------------------------------------------------------------------- |
| **Uygulama teması modu**           | Açık / koyu / sistem ayarlarını kullan                              |
| **Malzeme**                        | Pencere arka plan malzemesi (Akrilik vb.) + **Opaklık** kaydırıcısı |
| **Arka plan**                      | Özel renk veya resim; **Renk tonu** ve **Renk yoğunluğu** ayarları  |
| **Uygulama ayrıntılarını göster**  | Uygulama satırlarında ayrıntıları otomatik genişlet                 |
| **Geri tuşu geri götürür**         | Arama alanı boşken Backspace ile önceki sayfaya dön                 |
| **Escape tuşu davranışı**          | Esc ile önce aramayı temizle / geri dön / kapat                     |
| **Tek tıklamayla etkinleştirme**   | Tek tıkla çalıştır veya seç + çift tıkla çalıştır                   |
| **Animasyonları devre dışı bırak** | Sayfa geçişlerinde animasyonu kapat                                 |


Üstte **Komut Paletini Aç** ve **Varsayılanlara sıfırla** butonları bulunur.

##### Uzantılar

Yerleşik ve indirilen uzantılar burada listelenir; her birini ayrı aç/kapat. Sağdaki **>** ile uzantıya özel ayarlara girilir. Üstte **Uzantıları ara** ve Store / WinGet bağlantısı vardır.

> 💡 Kullanmadığın uzantıları kapat; arama sonuçları sadeleşir. Ek uzantılar Microsoft Store veya WinGet üzerinden indirilebilir.

##### Yuva (Önizleme)

Komutlara hızlı erişim için isteğe bağlı araç çubuğu - henüz önizleme aşamasında.


| Ayar                       | Ne işe yarar?                                              |
| -------------------------- | ---------------------------------------------------------- |
| **Yuvayı Etkinleştir**     | Araç çubuğunu aç/kapat                                     |
| **Konum**                  | Yuvanın ekrandaki yeri (Üst, Alt vb.)                      |
| **Boyut**                  | Varsayılan veya kompakt (kompaktta alt başlıklar gizlenir) |
| **Tema modu**              | Açık / koyu / sistem                                       |
| **Malzeme**                | Akrilik vb. görsel malzeme                                 |
| **Arka plan**              | Özel renk veya resim                                       |
| **Her zaman en üstte tut** | Tam ekran olmayan uygulamaların üzerinde kalır             |


> ⚠️ Eski rehberlerde geçen **PowerToys Run → Plugins** yapısı artık **Komut Paleti → Uzantılar** sekmesidir. Tam ekranda kısayol çalışmıyorsa **Genel** sekmesindeki tam ekran koruma seçeneklerini veya **3 kez hızlı basma** geçişini kontrol et.

---

<a id="arac-2"></a>

### 🖌️ 2- Color Picker - Renk Seçici

Ekrandaki herhangi bir renkten HEX, RGB, HSL ve daha fazla format kodu çıkaran eyedropper aracı. Tasarımcılar ve geliştiriciler için vazgeçilmez.

#### Ne sağlar?

- **Çoklu format** - HEX, RGB, HSL, HSV, CMYK, CIELAB vb.
- **Zoom modu** - Hassas piksel seçimi
- **Panoya kopyala** - Tek tıkla renk kodu
- **Özel format** - Kendi format şablonunu tanımla

#### Aktivasyon


| Eylem              | Varsayılan kısayol | Açıklama             |
| ------------------ | ------------------ | -------------------- |
| **Renk seçici aç** | `Win + Shift + C`  | Color picker modu    |
| **Renk seç**       | Sol tık            | Seçili rengi kopyala |
| **Zoom**           | `Ctrl + Scroll`    | Yakınlaştır          |
| **İptal**          | `Esc`              | Seçimi iptal et      |


#### Desteklenen formatlar (özet)


| Format     | Örnek                   | Kullanım    |
| ---------- | ----------------------- | ----------- |
| **HEX**    | `#FF5733`               | Web tasarım |
| **RGB**    | `rgb(255, 87, 51)`      | CSS         |
| **HSL**    | `hsl(9, 100%, 60%)`     | Tasarım     |
| **CMYK**   | `cmyk(0, 66, 80, 0)`    | Baskı       |
| **CIELAB** | `lab(53.2, 80.1, 67.2)` | Renk bilimi |


---

<a id="arac-3"></a>

### 💡 3- Light Switch - Işık Düğmesi

Günün saatine göre Windows açık/koyu temasını otomatik değiştirir. Gün ışığına uyumlu çalışma ortamı için pratik bir seçenektir.

---

<a id="arac-4"></a>

### 📝 4- Text Extractor - Metin Ayıklayıcısı

Ekrandaki herhangi bir görüntüden metin çıkaran OCR aracı. Windows'un yerleşik OCR motorunu kullanır.

#### Ne sağlar?

- **Ekrandan metin** - Herhangi bir uygulamadan kopyala
- **Alan seçimi** - Fare ile bölge belirle
- **Otomatik pano** - Seçim sonrası panoya kopyala

#### Aktivasyon


| Eylem             | Varsayılan kısayol | Açıklama            |
| ----------------- | ------------------ | ------------------- |
| **Metin çıkarma** | `Win + Shift + T`  | OCR modunu başlat   |
| **Alan seçimi**   | Fare ile sürükle   | Metin bölgesini seç |


#### Performans ipuçları

- Yalnızca metin alanını seç; gereksiz grafikleri dahil etme
- Yüksek kontrast ve düz arka plan daha iyi sonuç verir
- Türkçe OCR için Windows'ta ilgili **dil paketinin** yüklü olması gerekebilir

---

### Pencere Oluşturma ve Düzenle

<a id="arac-5"></a>

### 📌 5- Always On Top - Her Zaman Üstte

Seçili pencereyi diğer tüm pencerelerin üstünde tutar. Referans doküman, hesap makinesi veya not defteri gibi sürekli görünür kalması gereken uygulamalar için idealdir.

#### Ne sağlar?

- **Her zaman üstte** - Aktif pencereyi sabitle veya sabitlemeyi kaldır
- **Saydamlık kontrolü** - Sabitlenmiş pencerede opaklığı artır/azalt kısayolları (ayarlardan özelleştirilir)
- **Görsel kenarlık** - Üstte tutulan pencereleri renk, kalınlık ve köşe yuvarlatmasıyla ayırt et
- **Ses bildirimi** - Sabitleme anında isteğe bağlı ses
- **Oyun Modu koruması** - Oyun Modu açıkken devreye girmeyi engelleyebilirsin
- **Başlık çubuğu menüsü** - İsteğe bağlı: pencere başlığına sağ tıkla → Her Zaman Üstte

#### Nasıl kullanılır?

1. Sabitlemek istediğin pencereyi odakla
2. **Etkinleştirme kısayolu**na bas (Settings → **Always on top** → **Etkinleştirme** bölümünden atanır; kalem simgesiyle değiştirilebilir)
3. Pencere üstte kalır; aynı kısayolla sabitlemeyi kaldırırsın

Microsoft varsayılanı `Win + Ctrl + T` olsa da tuş kombinasyonunu istediğin gibi değiştirebilirsin.

#### Ayarlar sekmesi

Settings → **Always on top** altında iki ana bölüm vardır:

**Etkinleştirme**


| Ayar                                                      | Ne işe yarar?                                                 |
| --------------------------------------------------------- | ------------------------------------------------------------- |
| **Etkinleştirme kısayolu**                                | Pencereyi sabitle / sabitlemeyi kaldır - **değiştirilebilir** |
| **Saydamlığı artır**                                      | Sabitlenmiş pencerede opaklığı yükselt - **değiştirilebilir** |
| **Saydamlığı azalt**                                      | Sabitlenmiş pencerede saydamlığı artır - **değiştirilebilir** |
| **Oyun Modu açıkken etkinleştirmeyin**                    | Oyun oynarken yanlışlıkla tetiklenmeyi önler                  |
| **Başlık çubuğu bağlam menüsünde Her Zaman Üstte Göster** | Pencere başlığına sağ tık menüsüne seçenek ekler              |


**Görünüm ve davranış**


| Ayar                                                     | Ne işe yarar?                                      |
| -------------------------------------------------------- | -------------------------------------------------- |
| **Sabitlenmiş pencerenin etrafında bir kenarlık göster** | Üstte tutulan pencereyi görsel olarak işaretler    |
| **Renk modu**                                            | Kenarlık rengi: Windows varsayılanı veya özel renk |
| **Opaklık (%)**                                          | Kenarlık şeffaflığı                                |
| **Kalınlık (piksel)**                                    | Kenarlık kalınlığı                                 |
| **Yuvarlak köşeleri etkinleştir**                        | Kenarlığı pencere köşelerine uyumlu yapar          |
| **Pencereyi sabitlerken ses çal**                        | Sabitleme anında ses geri bildirimi                |


---

<a id="arac-6"></a>

### ✂️ 6- Crop And Lock - Kırp ve Kilitle

Geçerli bir uygulamayı daha küçük bir pencereye kırpar veya küçük resim oluşturur. Başka programlarla çalışırken bir uygulamanın belirli bölümünü izlemek için kullanışlıdır. Detaylı referans: [Microsoft Learn - Crop And Lock](https://learn.microsoft.com/tr-tr/windows/powertoys/crop-and-lock)

#### Nasıl kullanılır?

1. Kırpmak istediğin pencereyi odakla
2. Aşağıdaki kısayollardan birine bas → fare ile alan seç
3. `Esc` ile seçimi iptal edebilirsin; kırpılmış pencereyi kapatınca özgün pencere geri gelir

#### Kırpma modları


| Mod                  | Varsayılan kısayol       | Ne yapar?                                                                                    |
| -------------------- | ------------------------ | -------------------------------------------------------------------------------------------- |
| **Küçük resim**      | `Win + Ctrl + Shift + T` | Seçili alanı canlı yansıtır; küçük resimden denetlenemez. Uygulamalar arası en uyumlu mod.   |
| **Yeniden ayrıştır** | `Win + Ctrl + Shift + R` | Uygulamayı kırpılmış pencereden denetlersin. Deneysel; bazı uygulamalarda sorun çıkarabilir. |
| **Ekran görüntüsü**  | `Win + Ctrl + Shift + S` | Statik anlık görüntü; özgün pencere değişince güncellenmez.                                  |


> 💡 Yeniden ayrıştır modu Hesap Makinesi, Not Defteri veya OneNote gibi uygulamalarda kötü tepki verebilir - sorun yaşarsan **Küçük resim** modunu dene. Tüm kısayollar Settings → **Crop and Lock** altından değiştirilebilir.

---

<a id="arac-7"></a>

### 🪟 7- FancyZones - FancyZones

Windows'un pencere yönetimini geliştirir; özelleştirilebilir bölge (zone) düzenleri oluşturup pencereleri bu bölgelere yaslamanı sağlar. Çoklu monitör kurulumları için optimize edilmiştir.

#### Ne sağlar?

- **Özel düzenler** - Sütun, satır, ızgara veya serbest bölge düzeni
- **Sürükleyerek yaslama** - Pencereyi bölgeye sürükle (Shift veya fare düğmesi ayarlanabilir)
- **Düzen düzenleyicisi** - Bölgeleri görsel olarak çiz, kaydet, monitör başına ata
- **Hızlı düzen geçişi** - Düzenleyicide tanımlanan düzen kısayolları
- **Bölgedeki pencere geçişi** - Aynı bölgedeki pencereler arasında döngüsel geçiş
- **Windows Snap geçersiz kılma** - İsteğe bağlı: `Win + ok` tuşlarını FancyZones bölgelerine yönlendir
- **Dışlanan uygulamalar** - Belirli programları FancyZones dışında bırak

#### Nasıl kullanılır?

1. Settings → **FancyZones** → **Düzen düzenleyicisini aç** ile düzen oluştur veya düzenle
2. Pencereyi sürüklerken bölgeleri etkinleştir (varsayılan: **Shift basılı tut** - **Bölgeler → Bölge davranışı** altından değiştirilebilir)
3. Pencereyi istediğin bölgeye bırak

Modül **Etkinleştirme kısayolu**, **Sonraki/Önceki pencere** ve düzen kısayollarının tamamı Settings'ten veya düzenleyiciden özelleştirilebilir; sabit tuş kombinasyonu varsayılmaz.

#### Ayarlar sekmesi

Settings → **FancyZones** altında üç ana bölüm vardır:

##### Üst bölüm


| Ayar                             | Ne işe yarar?                                                                     |
| -------------------------------- | --------------------------------------------------------------------------------- |
| **Düzen düzenleyicisini aç**     | Bölge düzenlerini oluştur, düzenle ve monitörlere ata                             |
| **Etkinleştirme kısayolu**       | Modülü etkinleştiren tuş - **değiştirilebilir** (kalem simgesi)                   |
| **Düzenleyiciyi ekranda başlat** | Çoklu monitörde editörün hangi ekranda açılacağı (örn. fare işaretçisinin konumu) |


##### Bölgeler

**Bölge davranışı** - FancyZones kullanılırken bölgelerin nasıl davranacağını yönetir:


| Ayar                                            | Ne işe yarar?                                                                      |
| ----------------------------------------------- | ---------------------------------------------------------------------------------- |
| **Shift tuşunu basılı tutma**                   | Pencere sürüklerken bölgeleri etkinleştirir                                        |
| **Birincil olmayan fare düğmesi**               | Bölge etkinleştirmesini fare düğmesiyle aç/kapat                                   |
| **Orta tıklama**                                | Birden çok bölgeyi kapsamaya geçiş                                                 |
| **Tüm monitörlerdeki bölgeleri göster**         | Sürüklerken her monitördeki bölgeleri gösterir                                     |
| **Bölgelerin monitörleri kaplamasına izin ver** | Bölgeler monitör sınırını aşabilir (tüm monitörler aynı DPI ölçeklemesinde olmalı) |
| **Birden çok bölge çakıştığında**               | Çakışan bölgelerde hangisinin seçileceği (örn. alana göre en küçük bölge)          |


**Bölge görünümü** - Bölgelerin görsel stilini özelleştirir:


| Ayar                        | Ne işe yarar?                                     |
| --------------------------- | ------------------------------------------------- |
| **Görünüm modu**            | Bölge rengi/stili (Windows varsayılanı veya özel) |
| **Bölge numarasını göster** | Bölgelerin üzerinde numara gösterir (1, 2, 3…)    |


##### Pencereler

**Pencere davranışı**


| Ayar                                                  | Ne işe yarar?                                                 |
| ----------------------------------------------------- | ------------------------------------------------------------- |
| **Çözünürlük/çalışma alanı değişince bölgelerde tut** | Ekran değişince pencereleri bölgesinde bırakır                |
| **Düzen değişince boyut/konumu eşleştir**             | Bölge düzeni güncellenince atanan pencereler yeni boyuta uyar |
| **Yeni pencereyi son bilinen bölgeye taşı**           | Yeni açılan pencereyi son kullandığı bölgeye yerleştirir      |
| **Yeni pencereleri etkin monitöre taşı**              | Deneysel: yeni pencereyi imlecin monitörüne alır              |
| **Tutturma kaldırılınca özgün boyutu geri yükle**     | Bölgeden çıkarınca pencereyi eski boyutuna döndürür           |
| **Sürüklenen pencereyi saydam yap**                   | Sürükleme sırasında pencere opaklığını düşürür                |
| **Alt pencerelerin tutturulmasına izin ver**          | Child window'ların da bölgeye yaslanmasına izin verir         |
| **Tutturulunca yuvarlak köşeleri devre dışı bırak**   | Yaslanmış pencerede köşe yuvarlatmasını kapatır               |


**Geçerli bölgede pencereler arasında geçiş** - Aynı bölgedeki pencereler arasında döngüsel geçiş:


| Ayar                | Ne işe yarar?                                 |
| ------------------- | --------------------------------------------- |
| **Ana anahtar**     | Özelliği aç/kapat                             |
| **Sonraki pencere** | Sıradaki pencereye geç - **değiştirilebilir** |
| **Önceki pencere**  | Önceki pencereye geç - **değiştirilebilir**   |


**Windows Snap'i Geçersiz Kılma** - Açıkken `Win + ok` tuşları Windows Snap yerine FancyZones bölgelerine taşır:


| Ayar                                        | Ne işe yarar?                                        |
| ------------------------------------------- | ---------------------------------------------------- |
| **Ana anahtar**                             | Windows Snap geçersiz kılmayı aç/kapat               |
| **Pencereleri şuna göre taşı**              | Bölge dizini + `Win + <` / `>` gibi yön tuşları      |
| **Tüm monitörlerde bölgeler arasında taşı** | Pencereyi monitörler arası bölge geçişine izin verir |


##### Düzenler


| Ayar                                   | Ne işe yarar?                                                                                                                       |
| -------------------------------------- | ----------------------------------------------------------------------------------------------------------------------------------- |
| **Hızlı düzen anahtarını etkinleştir** | Düzen bazlı kısayollar; her düzenin kısayolu **düzenleyicide** yapılandırılır                                                       |
| **Dışlanan uygulamalar**               | Satır başına bir `.exe` adı (örn. `outlook.exe`); listedeki uygulamalar FancyZones'u yok sayar, yalnızca Windows Snap'e tepki verir |


#### Düzen oluşturma

1. Settings → **FancyZones** → **Düzen düzenleyicisini aç**
2. Monitör seç (çoklu monitör için)
3. Hazır şablon seç veya yeni düzen oluştur
4. Bölgeleri çiz → kaydet ve uygula
5. İsteğe bağlı: **Hızlı düzen anahtarı** açıksa düzenleyicide düzen kısayollarını tanımla

> 💡 **Windows Snap'i Geçersiz Kılma** kapalıyken Windows'un yerleşik snap'i (`Win + ok`) normal çalışır; FancyZones yalnızca sürükleyerek yaslama ile devreye girer. İkisini birlikte kullanmak istiyorsan geçersiz kılmayı aç.

---

<a id="arac-8"></a>

### 🤲 8- Grab And Move - Yakala ve Taşı

Değiştirici tuşu basılı tutarak pencere içinden herhangi bir yere sürükleyerek taşıma ve yeniden boyutlandırma yapmanı sağlar. Başlık çubuğu veya ince kenarlık hedeflemeden pencereyi yönetmek için kullanışlıdır. Detaylı referans: [Microsoft Learn - Grab And Move](https://learn.microsoft.com/tr-tr/windows/powertoys/grab-and-move)

#### Nasıl kullanılır?

1. Settings → **Grab and Move** / **Yakala ve Taşı** modülünü aç
2. **Etkinleştirme değiştirici tuşu**nu basılı tut (varsayılan: **Alt**)
3. **Sol tık + sürükle** → pencereyi taşı | **Sağ tık + sürükle** → en yakın kenar/köşeden yeniden boyutlandır

#### Önemli ayarlar


| Ayar                                   | Ne işe yarar?                                                                    |
| -------------------------------------- | -------------------------------------------------------------------------------- |
| **Etkinleştirme değiştirici tuşu**     | **Alt** veya **Windows tuşu** - taşıma/yeniden boyutlandırma için basılı tutulur |
| **Alt menüsünü engelle**               | Sürükleme sonrası Alt tuşunun pencere menüsünü açmasını önler                    |
| **Sağ tıkla yeniden boyutlandır**      | Değiştirici + sağ tık sürüklemeyi aç/kapat                                       |
| **Oyun Modu açıkken etkinleştirmeyin** | Oyun oynarken yanlışlıkla tetiklenmeyi önler                                     |
| **Pencere geometrisini göster**        | Sürüklerken konum ve boyutu katman olarak gösterir                               |
| **Dışlanan uygulamalar**               | Satır başına bir `.exe` adı; listedeki uygulamalar hariç tutulur                 |


> 💡 Bazı dokunmatik yüzeylerde güvenilir çalışmayabilir. Değiştirici tuşu Settings'ten değiştirilebilir.

---

### Giriş ve Çıkış

<a id="arac-9"></a>

### ⌨️ 9- Keyboard Manager - Klavye Yöneticisi

Klavye tuşlarını yeniden atamanı ve özel kısayollar oluşturmanı sağlar. Ergonomi iyileştirme ve özel workflow'lar için idealdir.

#### Ne sağlar?

- **Key remapping** - Tek tuşu başka tuşa eşle (Caps Lock → Escape vb.)
- **Shortcut remapping** - Kısayol kombinasyonlarını değiştir

> Tüm eşlemeler **sistem genelinde** geçerlidir; uygulama bazlı kural yoktur.

#### Örnek eşlemeler

**Tuş yeniden atama:**


| Orijinal     | Yeni        |
| ------------ | ----------- |
| Caps Lock    | Escape      |
| Right Alt    | Right Ctrl  |
| Print Screen | Windows Key |


**Kısayol yeniden atama:**


| Orijinal | Yeni         |
| -------- | ------------ |
| Ctrl+C   | Ctrl+Shift+C |
| Alt+Tab  | Win+Tab      |


> ⚠️ Sistem düzeyinde tuş eşleme beklenmedik davranışlara yol açabilir; tek tek test et.

---

<a id="arac-10"></a>

### 🖱️ 10- Mouse utilities - Fare Yardımcı Programları

Settings'te **Mouse utilities / Fare yardımcı programları** altında birleşik bir modül olarak geçer. İmleci bulma, tıklamaları vurgulama, uzun mesafe atlama ve nişangah çizme gibi alt araçları içerir. Detaylı referans: [Microsoft Learn - Mouse utilities](https://learn.microsoft.com/tr-tr/windows/powertoys/mouse-utilities)

#### Alt araçlar özeti


| Alt araç                                         | Ne yapar?                                    | Varsayılan kısayol / tetikleme                |
| ------------------------------------------------ | -------------------------------------------- | --------------------------------------------- |
| **CursorWrap - İmleç Sarma**                     | İmleci monitör kenarları arasında kaydırır   | Settings'ten atanır                           |
| **Find My Mouse - Faremi Bul**                   | İmlecin konumunu spot ışığıyla vurgular      | `Ctrl + Ctrl`, fare sallama veya özel kısayol |
| **Mouse Highlighter - Fare Vurgulayıcı**         | Sol/sağ tıklamaları görsel olarak vurgular   | `Win + Shift + H` (aç/kapat)                  |
| **Mouse Jump - Fare Atlama**                     | İmleci uzun mesafede hızlıca taşır           | `Win + Shift + D`                             |
| **Crosshairs - Fare İşaretçisi Artı İşaretleri** | İmlecin üzerinde artı işareti çizer          | `Win + Alt + P`                               |
| **Kayan imleç** *(Crosshairs altında)*           | Kılavuzlu çizgilerle tek tuşla fare kontrolü | `Win + Alt + .`                               |


#### Find My Mouse - Faremi Bul

Ctrl'e çift basarak, fareyi sallayarak veya özel kısayolla imleci vurgular. Kapatmak için tıkla veya herhangi bir tuşa bas.


| Ayar                      | Seçenekler / not                                               |
| ------------------------- | -------------------------------------------------------------- |
| **Etkinleştirme yöntemi** | Sol/sağ `Ctrl` çift bas, **Fareyi sallayın**, **Özel kısayol** |
| **Görünüm**               | Arka plan rengi, spot rengi, yarıçap, animasyon süresi         |
| **Dışlanan uygulamalar**  | Belirli uygulamalarda devre dışı (oyunlar vb.)                 |


#### Mouse Highlighter - Fare Vurgulayıcı

Sunum ve ekran kaydı sırasında tıklamaları vurgular. `Win + Shift + H` ile modu aç/kapat; sol ve sağ tık farklı renklerle gösterilir.


| Ayar           | Seçenekler / not                                         |
| -------------- | -------------------------------------------------------- |
| **Vurgu modu** | **Öne çıkarma** (ekranı karartır) veya **Daire vurgusu** |
| **Renkler**    | Birincil/ikincil düğme ve imleç rengi özelleştirilebilir |
| **Solma**      | Gecikme ve süre ayarlanabilir                            |


#### CursorWrap, Jump ve Crosshairs

- **CursorWrap** - Kenardan geçerken imleci karşı tarafa taşır; dikey/yatay sarma modu ve `Ctrl`/`Shift` ile etkinleştirme seçenekleri vardır
- **Mouse Jump** - Tek ekranda veya çoklu monitörde uzun mesafe atlama; küçük resim boyutu varsayılan **1600×1200** px ile sınırlanabilir
- **Crosshairs** - Hassas hizalama için imleç merkezli artı işareti; renk, opaklık, kalınlık ve yönelim ayarlanır
- **Kayan imleç** - Erişilebilirlik özelliği; `Esc` veya tıklama ile iptal edilir

> 💡 Her alt aracın kısayolu ve davranışı Settings → **Mouse utilities** altında ayrı ayrı yapılandırılır. Oyun Modu açıkken devre dışı bırakma seçeneği birçok alt araçta mevcuttur.

---

<a id="arac-11"></a>

### ⌨️ 11- Quick Accent - Hızlı Aksan

Aksan karakterlerini (é, ñ, ü, ç vb.) hızlı yazmayı sağlar. Çoklu dil desteği ile uluslararası karakter girişini kolaylaştırır.

#### Aktivasyon


| Eylem           | Varsayılan tetikleme   | Açıklama                          |
| --------------- | ---------------------- | --------------------------------- |
| **Hızlı seçim** | Harf basılı tut + Space | En yaygın aksanı ekler (varsayılan Space) |


#### Örnekler

```
e + Space = é
a + Space = á
c + Space = ç
n + Space = ñ
```

#### Önemli ayarlar


| Ayar                 | Seçenekler                             |
| -------------------- | -------------------------------------- |
| **Etkinleştirme tuşu** | Varsayılan **Space** - Settings'ten değiştirilebilir |
| **Input Time**       | 300–1000ms basılı tutma                |
| **Excluded Apps**    | Oyunlar vb.                            |
| **Toolbar Position** | Above / Below / Center                 |


---

### Dosya Yönetimi

<a id="arac-12"></a>

### 📁 12- File Explorer add-ons - Dosya Gezgini Eklentileri

SVG, PDF, Markdown, kaynak kod ve daha fazlası için Explorer'da **önizleme bölmesi** ve **küçük resim** desteği ekler. Dosyayı ayrı uygulama açmadan içeriğini görmene olanak tanır. Detaylı referans: [Microsoft Learn - File Explorer add-ons](https://learn.microsoft.com/tr-tr/windows/powertoys/file-explorer)

#### Nasıl kullanılır?

1. Settings → **File Explorer** / **Dosya Gezgini** → istediğin uzantıları **Açık** yap
2. Explorer'da **Görünüm** → **Önizleme bölmesi** (veya `Alt + P`)
3. Önizleme çalışmıyorsa: **Görünüm → Seçenekler → Görünüm** → **Önizleme bölmesinde önizleme işleyicilerini göster** seçeneğini işaretle

#### Önizleme bölmesi


| Desteklenen türler              | Not                                                                |
| ------------------------------- | ------------------------------------------------------------------ |
| **SVG** (.svg)                  | Kareli gölge arka planı ayarlanabilir                              |
| **Markdown** (.md, .markdown …) |                                                                    |
| **Kaynak kod** (150+ uzantı)    | Monaco editör; sözdizimi vurgulama, mini harita, yapışkan kaydırma |
| **PDF** (.pdf)                  |                                                                    |
| **G-code / BGCODE / QOI**       | 3B baskı ve görüntü formatları                                     |


Kaynak kod önizlemesinde yazı tipi boyutu, maksimum dosya boyutu, JSON/XML biçimlendirme gibi ayarlar **Kaynak kod dosyaları (Monaco)** bölümünden yapılır.

#### Küçük resim simgesi önizlemesi


| Desteklenen türler                     |
| -------------------------------------- |
| SVG, PDF, G-code, BGCODE, **STL**, QOI |


#### Önemli notlar

- Önizleme işleyicileri etkinleştirildiğinde mevcut işleyicilerin üzerine yazar; **Outlook ile PDF önizleme** arasında uyumsuzluk bildirilmiştir
- Küçük resimler etkinleştirildikten sonra **yeniden başlatma** gerekebilir
- **OneDrive** gibi bulut klasörlerinde küçük resimler görünmeyebilir (buluttan alınır, yerel oluşturulmaz)
- Saydam SVG'lerde beyaz şekiller önizleme arka planında görünmeyebilir

---

<a id="arac-13"></a>

### 🔒 13- File Locksmith - Dosya Çilingiri

“Dosya kullanımda” hatalarında hangi sürecin dosyayı kilitlediğini gösterir. Silme, taşıma ve düzenleme sorunlarını hızlıca çözer.

#### Ne sağlar?

- **Süreç analizi** - Dosyayı hangi program kullanıyor?
- **Sağ tık entegrasyonu** - **What's using this file?**
- **Toplu analiz** - Çoklu dosya seçimi

#### Yaygın senaryolar


| Senaryo           | Sebep             | Çözüm            |
| ----------------- | ----------------- | ---------------- |
| Video silinmiyor  | Media player açık | Player'ı kapat   |
| Log kopyalanmıyor | Servis yazıyor    | Servisi durdur   |
| Excel açılmıyor   | Arka planda Excel | Süreci sonlandır |


---

<a id="arac-14"></a>

### 🖼️ 14- Image Resizer - Resim Boyutlandırıcı

Görüntüleri hızlı ve toplu olarak yeniden boyutlandırır. Web yayını, e-posta ekleri ve depolama optimizasyonu için idealdir.

#### Ne sağlar?

- **Sağ tık menüsü** - Explorer'da seçili görüntülerde **Resize pictures**
- **Preset boyutlar** - Önceden tanımlı çözünürlükler
- **Toplu işlem** - Ctrl+A ile klasördeki tüm resimler

#### Preset örnekleri


| Amaç               | Boyut     | Kullanım     |
| ------------------ | --------- | ------------ |
| **Instagram Post** | 1080×1080 | Sosyal medya |
| **Email eki**      | 800×600   | ~200KB hedef |
| **Web galeri**     | 1200×800  | ~500KB hedef |
| **Thumbnail**      | 200×150   | Önizleme     |


Preset'leri Settings → **Image Resizer** → **Encoder settings** altından özelleştirebilirsin.

---

<a id="arac-15"></a>

### 👁️ 15- Peek - Gözatma

Explorer'da dosya seçip kısayola basarak uygulama açmadan hızlı önizleme yapmanı sağlar. Görüntü, Office belgesi, video, Markdown, kaynak kod ve daha fazlasını destekler. Detaylı referans: [Microsoft Learn - Peek](https://learn.microsoft.com/tr-tr/windows/powertoys/peek)

#### Nasıl kullanılır?

1. File Explorer'da dosyayı seç
2. **Etkinleştirme kısayolu**na bas (varsayılan: **Space** - özelleştirilebilir)
3. Ok tuşlarıyla aynı klasördeki dosyalar arasında gez; **Enter** ile varsayılan programda aç

#### Önemli ayarlar


| Ayar                                  | Ne işe yarar?                                                                |
| ------------------------------------- | ---------------------------------------------------------------------------- |
| **Etkinleştirme kısayolu**            | Özel kısayol veya **Space** - Settings'ten değiştirilebilir                  |
| **Yükseltilmeden her zaman çalıştır** | PowerToys yönetici olarak çalışsa bile ağ paylaşımlarına erişimi iyileştirir |
| **Odak kaybedince otomatik kapat**    | Peek penceresi arka plana geçince kapanır                                    |
| **Silmeden önce onay iste**           | `Delete` ile Geri Dönüşüm Kutusu'na taşımadan önce uyarı gösterir            |
| **Kaynak kod (Monaco)**               | Metin kaydırma, biçimlendirme, yazı tipi, mini harita                        |


> 💡 Pencere boyutunu/konumunu **sabitle** düğmesiyle koruyabilirsin. Yalnızca dosyalar silinebilir; klasörler silinemeyebilir.

---

<a id="arac-16"></a>

### 🏷️ 16- PowerRename - PowerRename

Explorer'da seçtiğin dosya ve klasörleri toplu olarak yeniden adlandırır. Basit metin arama/değiştirmeden regex'e kadar genişler; uygulamadan önce önizleme gösterir. Detaylı referans: [Microsoft Learn - PowerRename](https://learn.microsoft.com/tr-tr/windows/powertoys/powerrename)

#### Ne sağlar?

- **Toplu yeniden adlandırma** - Aynı anda onlarca dosyayı tek işlemde değiştir
- **Önizleme** - Uygulamadan önce eski ve yeni adları yan yana gör
- **Geri alma** - İşlem sonrası Explorer'da `Ctrl + Z` ile son adımı geri al
- **Esnek hedefleme** - Yalnızca dosya adı, yalnızca uzantı veya tam ad
- **Regex desteği** - Karmaşık desenler (isteğe bağlı)
- **Numaralandırma ve tarih** - Sıra numarası veya dosya tarihini ada ekleme

#### Nasıl kullanılır?

1. File Explorer'da dosya/klasörleri seç (Ctrl / Shift ile çoklu seçim)
2. Sağ tık → **PowerRename ile yeniden adlandır** *(PowerToys'ta modül açık olmalı)*
3. **Şunu ara** ve **Bununla değiştir** alanlarını doldur
4. **Önizleme** sütununda sonucu kontrol et → **Uygula**

> 💡 Yanlış seçim yaptıysan pencereyi kapat; uygulamadan sonra Explorer'da **Geri Al** (`Ctrl + Z`) çoğu durumda yeterli olur.

#### Pencere seçenekleri

**Temel alanlar**


| Alan                 | Ne işe yarar?                                    |
| -------------------- | ------------------------------------------------ |
| **Şunu ara**         | Dosya adında aranacak metin veya regex deseni    |
| **Bununla değiştir** | Eşleşen kısmın yerine yazılacak metin            |
| **Önizleme**         | Seçili dosyaların eski ve yeni adlarını listeler |


**Sık kullanılan seçenekler**


| Seçenek                             | Ne işe yarar?                                                  |
| ----------------------------------- | -------------------------------------------------------------- |
| **Normal ifadeleri kullanma**       | Açıkken regex; kapalıyken düz metin arama                      |
| **Tüm örnekleri eşleştir**          | Aynı addaki tüm eşleşmeleri değiştirir (yalnızca ilkini değil) |
| **Büyük/küçük harfe duyarlı**       | Büyük/küçük harf farkını dikkate alır                          |
| **Yalnızca dosya adı**              | Uzantıya dokunmaz (`dosya.txt` → `yeni.txt`)                   |
| **Yalnızca uzantı**                 | Yalnızca uzantıyı değiştirir (`dosya.txt` → `dosya.pdf`)       |
| **Dosyaları / Klasörleri dahil et** | Hangi türlerin işleme gireceğini belirler                      |
| **Alt klasörleri dahil et**         | Alt klasörlerdeki öğeleri de listeye ekler                     |
| **Metin biçimlendirme**             | Tamamen küçük/büyük harf, cümle başı, her kelime büyük         |


**Önizleme filtreleri**

- **Orijinal** sütun başlığına tıkla → dosyayı yeniden adlandırma listesinden çıkar/ekle
- **Yeniden Adlandırıldı** sütun başlığına tıkla → yalnızca gerçekten değişecek dosyaları göster

#### Basit örnekler


| Ne yapmak istiyorsun?  | Şunu ara     | Bununla değiştir | Not                                                |
| ---------------------- | ------------ | ---------------- | -------------------------------------------------- |
| Uzantı değiştir        | `.jpg`       | `.png`           | Regex kapalı                                       |
| Boşluk → alt çizgi     | ` ` (boşluk) | `_`              | Regex kapalı                                       |
| Başına ekle            | `^`          | `backup_`        | Regex **açık**                                     |
| Sona ekle              | `$`          | `_eski`          | Regex **açık**                                     |
| Tarih formatı değiştir | `2024-01-15` | `15.01.2024`     | Regex açık: `(\d{4})-(\d{2})-(\d{2})` → `$3.$2.$1` |


**Numaralandırma** - *Bununla değiştir* alanında:

```
Image_${padding=2;start=1}_
```

`a.jpg`, `b.jpg` → `Image_01_a.jpg`, `Image_02_b.jpg`

**Dosya tarihi** - oluşturma tarihini ada eklemek için *Bununla değiştir* alanında `$YYYY`, `$MM`, `$DD` gibi desenler kullanılabilir (örn. `$YYYY-$MM-$DD_`).

#### Regex (kısa)

Karmaşık işlemler için **Normal ifadeleri kullanma** seçeneğini aç. Regex kullanırken genelde **Tüm örnekleri eşleştir** de açık olmalı.


| Şunu ara                  | Bununla değiştir | Sonuç                         |
| ------------------------- | ---------------- | ----------------------------- |
| `(.*).png`                | `$1_foo.png`     | `resim.png` → `resim_foo.png` |
| `(\d{2})-(\d{2})-(\d{4})` | `$3-$2-$1`       | `29-03-2020` → `2020-03-29`   |
| `^`                       | `2024_`          | Ada `2024_` öneki ekler       |


Gelişmiş regex (lookbehind vb.) için Settings → **Boost kitaplığını kullanma** seçeneğine bak.

#### Settings ayarları

Settings → **PowerRename**:


| Ayar                                   | Ne işe yarar?                                                          |
| -------------------------------------- | ---------------------------------------------------------------------- |
| **PowerRename göster**                 | Sağ tık menüsünde varsayılan veya yalnızca genişletilmiş menüde göster |
| **Bağlam menüsündeki simgeyi gizle**   | Menüdeki PowerRename simgesini gizler                                  |
| **Başlatmada bayrakları geri yükleme** | Son kullandığın seçenekleri hatırlar                                   |
| **Otomatik tamamlama**                 | Önceki arama/değiştirme terimlerini önerir                             |
| **Son kullanılan dizeleri göster**     | Pencere açılınca son değerleri doldurur                                |
| **Boost kitaplığını kullanma**         | Genişletilmiş regex desteği                                            |


---

## ⚠️ Bilinen Sorunlar ve Çözümleri


| Sorun                                 | Neden Olur                                   | Çözüm                                                                                     |
| ------------------------------------- | -------------------------------------------- | ----------------------------------------------------------------------------------------- |
| Kısayol çalışmıyor                    | Varsayılan tuş başka uygulamada kullanılıyor | Settings → modül → **Activation shortcut** ile farklı kombinasyon ata                     |
| Modül açılmıyor                       | Eski sürüm veya bozuk ayar                   | PowerToys'u güncelle; Settings → General → **Restart PowerToys**                          |
| FancyZones snap bozuk                 | Windows Snap + FancyZones çakışması          | **Windows Snap'i Geçersiz Kılma** ayarını kontrol et; gerekirse Explorer'ı yeniden başlat |
| OCR zayıf sonuç                       | Düşük kontrast / küçük metin                 | Daha büyük alan seç; kontrastı artır                                                      |
| Keyboard Manager beklenmedik davranış | Sistem tuşu eşlemesi                         | Eşlemeyi kaldır; tek tek test et                                                          |
| Ayarlar sıfırlanmadı                  | Bozuk config                                 | `%USERPROFILE%\AppData\Local\Microsoft\PowerToys\` yedekle ve temizle                     |
| Yüksek kaynak kullanımı               | Çok fazla aktif modül                        | Kullanmadıklarını kapat                                                                   |


### Tanı komutları (PowerShell)

```powershell
# PowerToys süreçlerini kontrol et
Get-Process | Where-Object {$_.Name -like "*PowerToys*"}

# Event Log kontrol
Get-WinEvent -LogName Application -MaxEvents 10 | Where-Object { $_.ProviderName -like "*PowerToys*" }
```

---

## 🔗 Faydalı Bağlantılar

- 🌐 [Resmi Dokümantasyon (TR)](https://learn.microsoft.com/tr-tr/windows/powertoys/)
- 💾 [GitHub](https://github.com/microsoft/PowerToys)
- 📦 [GitHub Releases](https://github.com/microsoft/PowerToys/releases)
- 🏪 [Microsoft Store](https://apps.microsoft.com/detail/XP89DCGQGKSL6D)
- 📦 [WinGet paketi](https://winget.run/pkg/Microsoft/PowerToys)

---

## 📝 Notlar

> PowerToys modülerdir; hepsini aynı anda açmak gerekmez. Bu rehberdeki kısayollar varsayılandır - alışkanlığına göre **Settings → [modül] → Activation shortcut** ile değiştirebilirsin. Keyboard Manager ve FancyZones gibi sistem genelinde etkisi olan modüllerde değişiklik yapmadan önce mevcut tuşlarını not al. En güncel bilgi için [resmi siteyi](https://learn.microsoft.com/tr-tr/windows/powertoys) ve **PowerToys Settings** uygulamasını kontrol et.

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
