# 🛠️ WinToys

> **Kısa Açıklama:** Windows'un gizli ayarlarına, sistem araçlarına ve optimizasyon seçeneklerine tek arayüzden erişmeni sağlayan ücretsiz sistem yönetim aracı.

2.x · Windows 10/11 · Ücretsiz · Sistem yönetimi

---

## 📌 Genel Bakış

WinToys, Windows Ayarlar uygulamasında dağınık duran veya hiç bulunmayan sistem yönetimi araçlarını tek yerde toplar. Donanım bilgisi, uygulama kaldırma, hizmet yönetimi, temizlik ve gizlilik ayarları gibi işlemleri terminal veya registry açmadan yapmanı sağlar. Windows'un yerleşik araçlarına kıyasla daha hızlı erişim ve açıklayıcı arayüz sunar.

---

## ✨ Öne Çıkan Özellikler

WinToys sol menüsünde 6 sekme vardır; rehber bu yapıya göre düzenlenmiştir:

- **Giriş** - Donanım kartları, canlı CPU/GPU/RAM ve sistem özeti
- **Uygulamalar** - Kurulu programları listele, kaldır, sıfırla
- **Hizmetler** - Windows hizmetlerini filtrele, başlat veya durdur
- **Performans** - Güç planı, oyun ayarları, başlangıç uygulamaları
- **Sağlık** - Temizlik, güncelleme, onarım (DISM/SFC/CHKDSK), pil raporu
- **İnce Ayarlar** - Masaüstü, Explorer, gizlilik, reklam ve sistem tweak'leri

---

## 📥 İndirme ve Kurulum

### Yöntem 1: Microsoft Store ( Önerilen )

1. Microsoft Store'u aç
2. **WinToys** ara
3. **Al** butonuna tıkla

### Yöntem 2: WinGet (Terminal)

```powershell
winget install "WinToys"
```

### Yöntem 3: UniGetUI

> UniGetUI açıkken arama çubuğuna **WinToys** yaz ve kur.

**Alternatif:** [GitHub Releases](https://github.com/bogdandonduk/WinToys/releases) - kurulum dosyası (`WinToys-x.x.x-Setup.exe`) veya taşınabilir ZIP (`WinToys.exe`).

---

## ⚙️ İlk Kurulum ve Önerilen Ayarlar

1. **Yönetici izni:** İlk açılışta izin isteyebilir - onayla; uygulama ve hizmet listeleri için gereklidir
2. **İlk tarama:** WinToys sistemi tarar ve varsayılan ayarları yükler; birkaç saniye bekle
3. **Giriş sayfasını incele:** Donanım kartları ve canlı istatistiklerle sistemin genel durumunu kontrol et

> 💡 Tam liste göremiyorsan WinToys'u sağ tık → **Yönetici olarak çalıştır** ile aç.

---

# 🏠 Giriş

WinToys açıldığında karşına çıkan ilk sekme; bilgisayarının genel durumunu tek bakışta gösterir.

### Donanım kartları

| Kart | Ne gösterir |
| ---- | ----------- |
| **Sistem** | Bilgisayar modeli |
| **İşlemci** | CPU marka ve modeli |
| **Ekran Kartı** | GPU bilgisi |
| **Hafıza** | Toplam RAM |

### Sistem durumu

| Kart | Ne gösterir |
| ---- | ----------- |
| **Depolama** | Toplam disk kapasitesi |
| **Windows** | İşletim sistemi sürümü |
| **Çalışma Süresi** | Bilgisayarın açık kaldığı süre |
| **Performans** | Genel performans skoru |

### Canlı istatistikler

Alt panelde anlık veriler görünür:

- **CPU, GPU, RAM** kullanım yüzdeleri
- **Ağ trafiği** - indirme/yükleme hızı ve toplam veri
- **Özet sayaçlar** - kurulu uygulama, aktif süreç ve hizmet sayıları (yalnızca özet; ayrı süreç yönetimi sekmesi yok)

> 💡 Windows sürüm kartının üzerine gelince lisans durumu, ürün anahtarı ve güncelleme bilgisi gibi ek detaylar tooltip olarak görünür.

---

# 📱 Uygulamalar

Kurulu tüm programları listeler; arama, filtre ve hızlı eylemler sunar.

### Nasıl kullanılır?

1. Sol menüden **Uygulamalar** sekmesine git
2. Arama çubuğuyla program bul veya filtre/sıralama menüsünü kullan
3. Her satırda sürüm, geliştirici, boyut ve kurulum tarihi görünür

### Renk kodları

| Renk | Tür | Örnek |
| ---- | --- | ----- |
| 🟡 **Sarı** | Klasik masaüstü programı (Win32) | 7-Zip, Chrome |
| 🔵 **Mavi** | Microsoft Store uygulaması (UWP) | Ayarlar, Store uygulamaları |

### ⋯ menü eylemleri

| Eylem | Ne işe yarar |
| ----- | ------------ |
| **Kapat** | Açık programı sonlandır |
| **Gözat** | Kurulum klasörünü aç |
| **Arama** | Uygulama hakkında web'de ara |
| **Sıfırla** | Uygulama verilerini sıfırla (sorun giderme) |
| **Kaldır** | Programı sistemden kaldır |

> 💡 **Sıfırla** ve **Kaldır** geri alınamaz olabilir; özellikle Store uygulamalarında dikkatli ol.

---

# ⚙️ Hizmetler

Windows arka plan hizmetlerini listeler; durumlarını görmeni ve yönetmeni sağlar.

### Nasıl kullanılır?

1. Sol menüden **Hizmetler** sekmesine git
2. Arama çubuğu veya filtre menüsüyle hizmet bul
3. Yeşil çizgi = çalışıyor; çizgi yok = durdurulmuş

### Filtreler

**Tümü** · **Kullanışsız** · **Microsoft** · **Üçüncü taraf** · **Durum** · **Mod**

### ⋯ menü eylemleri

| Eylem | Ne işe yarar |
| ----- | ------------ |
| **Başlat** | Durdurulmuş hizmeti çalıştır |
| **Durdur** | Çalışan hizmeti durdur |
| **Yeniden Başlat** | Hizmeti yenile |
| **Gözat** | Hizmet dosyasının konumunu aç |
| **Arama** | Hizmet hakkında web'de ara |
| **Mod** | Başlangıç türünü değiştir (Otomatik / Elle / Devre dışı) |

> ⚠️ Tanımadığın bir hizmeti kapatma veya devre dışı bırakma. Yanlış müdahale ağ, ses, yazdırma veya güncelleme sorunlarına yol açabilir.

---

# 🚀 Performans

Sistem hızı, güç tüketimi ve oyun performansı için Windows ayarlarını tek ekranda toplar. Her seçeneğin üzerine gelince açıklama tooltip'i görünür.

### Nasıl kullanılır?

1. Sol menüden **Performans** sekmesine git
2. İhtiyacına göre anahtarı aç/kapat
3. **Başlangıç uygulamaları** için **Yapılandır** butonuna tıkla

### Güç ve performans

| Ayar | Ne işe yarar |
| ---- | ------------ |
| **Nihai performans güç planı** | CPU ve GPU'nun tam güç kullanmasına izin verir; dizüstünde pil tüketimini artırır |
| **HAGS** (Donanım hızlandırmalı GPU zamanlaması) | GPU görev dağılımını iyileştirir; gecikmeyi ve CPU yükünü azaltabilir |
| **VBS** (Sanallaştırma tabanlı güvenlik) | Ek güvenlik katmanı sağlar; kapalıyken oyunlarda hafif performans artışı görülebilir |

> 💡 **Nihai performans** bazı cihazlarda desteklenmeyebilir; WinToys uyarı gösterir. **VBS** kapatmak güvenliği düşürür - yalnızca performans için bilinçli tercih et.

### Başlangıç uygulamaları

**Yapılandır** ile açılan listede:

- **Yenile** - listeyi güncelle
- **Yeni başlangıç uygulaması ekle** - manuel program ekle
- **Yenisi eklenince bildir** - yeni başlangıç öğesi uyarısı

Gereksiz başlangıç programlarını kapatmak açılış süresini kısaltır.

### Uygulama ve arka plan

| Ayar | Ne işe yarar |
| ---- | ------------ |
| **Uygulamaları yeniden başlat** | Oturum kapanınca açık uygulamaları otomatik geri yükler |
| **Arka plan uygulamaları** | Store uygulamalarının arka planda çalışmasına izin verir |
| **Etkinlik geçmişi** | Kullandığın uygulama, dosya ve site geçmişini kaydeder |

> 💡 **Etkinlik geçmişi** kapalıyken gizlilik artar; Windows zaman çizelgesi ve geçmiş önerileri sınırlanır.

### Görsel ayarlar

Eski veya düşük donanımlı cihazlar için önerilir.

| Ayar | Ne işe yarar |
| ---- | ------------ |
| **En iyi performans için görsel efektleri ayarlayın** | Animasyon ve efektleri azaltır; arayüz daha sade olur |
| **Saydamlık** | Başlat menüsü ve görev çubuğu şeffaflık efektleri |

### Oyun ayarları

| Ayar | Ne işe yarar |
| ---- | ------------ |
| **Oyun modu** | Oyun oynarken arka plan işlemlerini önceliklendirir |
| **Pencereli mod iyileştirme seçenekleri** | Tam ekran olmayan oyunlarda performans iyileştirmesi |
| **Arka planda kayıt** | Xbox Game Bar arka plan kaydı; kapalıyken kaynak tasarrufu |
| **Diskten Hızlı Getirme** (DirectStorage) | Uyumlu SSD ve oyunlarda daha hızlı yükleme |

### Arka plan hizmetleri

| Ayar | Ne işe yarar |
| ---- | ------------ |
| **Arama indeksleme** | Windows aramasını hızlandırır; arka planda disk taraması yapar |
| **Teslim İyileştirme** | Windows güncellemelerini ağdaki diğer cihazlarla paylaşır |
| **Ağ bağdaştırıcısı yerleşik işlemci** | Ağ işlerini CPU yerine ağ kartına devreder (destekleyen kartlarda) |

> ⚠️ **Teslim İyileştirme** internetten güncelleme paylaşımını açabilir; yalnızca yerel ağda bırakmak için Windows Ayarlar'dan ince ayar yap. **Arama indekslemeyi** kapatmak aramayı yavaşlatır.

---

# 🏥 Sağlık

Sistem bakımı, temizlik, güncelleme ve onarım araçlarını tek ekranda toplar. Kilitlenme, yavaşlık veya disk doluluğu gibi sorunlarda ilk bakılacak bölümdür.

### Nasıl kullanılır?

1. Sol menüden **Sağlık** sekmesine git
2. Soruna göre ilgili aracı seç (temizlik, onarım, tanılama vb.)
3. Butonlu işlemlerde (**Denetle**, **Oluştur**, **Tamirat**) işlem bitene kadar bekle

### Tanılama ve hızlı onarım

| Araç | Ne işe yarar | Eylem |
| ---- | ------------ | ----- |
| **Bellek teşhis** | RAM hatalarını kontrol eder | **Denetle** - yeniden başlatma sonrası test çalışır |
| **Grafik sürücüsü** | Ekran donması/titremesinde GPU sürücüsünü sıfırlar | **Yeniden Başlat** |
| **Simge önbelleği** | Boş, bulanık veya bozuk simgeleri düzeltir | **Yeniden oluştur** |
| **Uyku hapı** | Bilgisayarı uyku modundan uyandıran zamanlanmış görevleri bulur | **Durdur** |

> 💡 **Bellek teşhis** çalışırken bilgisayar kapanır; kaydedilmemiş işlerini kapat.

### Güncelleme yönetimi

| Ayar | Ne işe yarar |
| ---- | ------------ |
| **Sistem Güncellemeleri** | Windows güncelleme davranışını ayarlar; yeni güncellemeleri kontrol eder |
| **Sürücü güncellemeleri** | Donanım sürücülerini otomatik arar ve günceller |
| **Uygulama Güncellemeleri** | Store uygulamalarını otomatik indirip kurar |
| **Ortak kurulumcular** | Yeni çevre birimi takılınca ek kurulum görevlerini çalıştırır |

### Önyükleme ve güç

| Ayar | Ne işe yarar |
| ---- | ------------ |
| **Hızlı başlatma** | Kapatma sonrası açılışı hızlandırır (hibrit kapatma) |
| **Hazırda bekletme** | Oturum durumunu `hiberfil.sys` dosyasına kaydeder; disk alanı kullanır |

> 💡 **Hızlı başlatma** kapalıyken tam kapatma yapılır; çift önyükleme sorunlarında kapatmayı dene. **Hazırda bekletme** kapalıyken hiberfil.sys silinir ve disk alanı açılır.

### Temizlik

Disk alanı açmak için manuel temizlik seçenekleri:

| Seçenek | Ne temizler |
| ------- | ----------- |
| **Gereksiz** | Geçici dosyalar, çöp kutusu, önbellek |
| **Dosya Gezgini** | Gezginci geçmişi ve önbellekleri |
| **Microsoft Store** | Store uygulama önbelleği |
| **Ağ** | DNS önbelleği |
| **Sistem Geri Yükleme** | Eski geri yükleme noktaları |

> ⚠️ **Sistem Geri Yükleme** temizliği geri alınamaz; önemli noktaları silmeden önce düşün.

### Otomatik bakım

| Ayar | Ne işe yarar |
| ---- | ------------ |
| **Sürücü İyileştirme** | SSD/HDD birleştirme ve optimizasyon zamanlaması |
| **Akıllı Depolama** | Geçici sistem dosyalarını otomatik temizler |

### Pil raporu (dizüstü)

WinToys → Sağlık → **Pil raporu** → **Oluştur** ile Windows'un standart pil raporu (`battery-report.html`) üretilir. Dosya genelde kullanıcı klasöründe oluşur; tarayıcıda aç.

#### Raporda neler var?

| Bölüm | Ne gösterir |
| ----- | ----------- |
| **Üst bilgi** | Bilgisayar adı, model, BIOS, Windows sürümü, rapor tarihi |
| **Installed batteries** | Pil kimliği ve sağlık verileri |
| **Recent usage** | Son 7 gün - Active/Suspended, AC/Battery, kalan % ve mWh |
| **Battery usage** | Pil tüketim oturumları - süre, harcanan % ve mWh (+ grafik) |
| **Usage history** | Haftalık/günlük AC ve pil kullanım süreleri |
| **Battery capacity history** | Zaman içinde tam şarj kapasitesinin değişimi |
| **Battery life estimates** | Gözlemlenen tüketime göre tahmini pil ömrü |

#### Installed batteries - okuma rehberi

| Alan | Anlamı |
| ---- | ------ |
| **NAME / MANUFACTURER** | Pil modeli ve üretici |
| **SERIAL NUMBER** | Seri numarası |
| **CHEMISTRY** | Pil tipi (ör. Li-I = lityum iyon) |
| **DESIGN CAPACITY** | Fabrika çıkışı hedef kapasite (mWh) |
| **FULL CHARGE CAPACITY** | Şu an %100 şarjda alabildiğin gerçek kapasite (mWh) |
| **CYCLE COUNT** | Tam şarj döngüsü sayısı |

**Kapasite oranı** = FULL CHARGE ÷ DESIGN × 100

Örnek: 49.770 ÷ 60.000 = **%83** → aşağıdaki tabloda **İyi** aralığı.

| Oran | Durum |
| ---- | ----- |
| %90–100 | Mükemmel |
| %80–89 | İyi |
| %60–79 | Orta - belirgin azalma |
| %40–59 | Zayıf - pil değişimi yaklaşabilir |
| <%40 | Kritik - acil değişim önerilir |

#### Battery usage - pil oturumları

Son 7 günde pilde geçen her oturum listelenir:

- **DURATION** - ne kadar süre pilde kaldın
- **ENERGY DRAINED** - o oturumda harcanan % ve mWh

Uzun oturumlar ve yüksek mWh değerleri pilin hangi kullanımlarda hızlı bittiğini gösterir.

#### Battery life estimates - tahmini ömür

İki sütun vardır:

| Sütun | Anlamı |
| ----- | ------ |
| **AT FULL CHARGE** | Mevcut pil kapasitesiyle tahmini kullanım süresi |
| **AT DESIGN CAPACITY** | Fabrika kapasitesiyle tahmini kullanım süresi |

En alttaki **Since OS install** satırı, kurulumdan bu yana tüm gözlemlere dayalı genel tahmini verir (ör. aktif kullanımda ~3–4 saat).

> 💡 Raporu ayda bir oluştur; **Battery capacity history** bölümünden kapasite düşüşünü zaman içinde takip edebilirsin. Masaüstü bilgisayarlarda pil bölümü boş veya "no batteries" görünür - normaldir.

### Onar (DISM / SFC / CHKDSK)

Kilitlenme, donma, mavi ekran veya başarısız güncelleme sonrası önerilir.

| Araç | Ne yapar |
| ---- | -------- |
| **DISM** | Bozuk Windows bileşen görüntüsünü onarır - internet gerekir |
| **SFC** | Korunan sistem dosyalarını tarar ve bozuk olanları değiştirir |
| **CHKDSK** | Disk hatalarını ve bozuk sektörleri kontrol eder - C: sürücüsü için yeniden başlatma gerekebilir |

1. En az bir aracı işaretle
2. **Tara** ile sorun tespiti veya doğrudan **Tamirat** ile onarım başlat

> ⚠️ Onarım uzun sürebilir; işlem sırasında bilgisayarı kapatma. Sorun devam ederse Windows yeniden kurulumu düşün.

---

# 🔧 İnce Ayarlar

Windows'un registry ve Ayarlar uygulamasında dağınık duran tweak'leri kategorilere ayırarak sunar. Her seçeneğin üzerine gelince açıklama tooltip'i görünür.

### Nasıl kullanılır?

1. Sol menüden **İnce Ayarlar** sekmesine git
2. Kategori başlığını aç (Masaüstü, Başlat Menüsü, Dosya Gezgini…)
3. Anahtarı değiştir - çoğu ayar anında uygulanır

> 💡 Aşağıdaki **Benim ayarım** sütunu kişisel kurulumumu gösterir; senin ihtiyacına göre farklı seçebilirsin.

### Özet - kişisel tercihlerim

- **Gizlilik odaklı:** Telemetri, konum ve reklamlar kapalı; yalnızca CEIP ve hata raporlama açık
- **Temiz Başlat menüsü:** Bing arama, Store önerileri ve hesap bildirimleri kapalı
- **Verimli Explorer:** Uzantılar ve gizli dosyalar görünür; açılış **Bu bilgisayar**
- **Prodüktivite:** Pano geçmişi, Print Screen ekran görüntüsü, görevi sonlandır açık
- **Güvenli gelişmiş:** God Mode ve Geliştirici Modu kapalı; UAC standart seviyede

---

### 🖥️ Masaüstü

Masaüstü simgeleri, sağ tık menüsü ve duvar kağıdı kalitesi.

| Ayar | Ne işe yarar | Benim ayarım |
| ---- | ------------ | ------------ |
| **Bu Bilgisayar** | Masaüstünde Bu PC simgesi | ✅ Açık |
| **Geri Dönüşüm Kutusu** | Çöp kutusu simgesi | ✅ Açık |
| **Araçlar** | Masaüstünde sistem araçları kısayolu simgesi | ❌ Kapalı |
| **Kısayol oku** | Kısayol simgelerindeki ok işareti | ❌ Kapalı |
| **Simge etiketleri için gölgeler** | Simge yazılarının altında gölge | ✅ Açık |
| **Masaüstünü Göster** | Sağ alt köşeye tıklayınca pencereleri gizle | ✅ Açık |
| **Başlık çubuğu penceresi salla** | Pencere sallayınca diğerlerini küçült (Aero Shake) | ❌ Kapalı |
| **Klasik içerik menüsü** | Windows 10 tarzı sağ tık menüsü | ❌ Kapalı |
| **Duvar kağıdı kalitesi** | Arka plan görüntü sıkıştırma (kaydırıcı) | Maksimum |

---

### 📱 Başlat Menüsü

Başlat araması, Store önerileri ve güç menüsü.

| Ayar | Ne işe yarar | Benim ayarım |
| ---- | ------------ | ------------ |
| **Arama yaparken web sonuçlarını dahil et** | Başlat aramasında Bing sonuçları | ❌ Kapalı |
| **Otomatik yükleme önerileri** | Store uygulama önerileri | ❌ Kapalı |
| **Hesap bildirimleri** | Microsoft hesabı bildirimleri | ❌ Kapalı |
| **Güç menüsünde hazırda bekletme modunu göster** | Kapat menüsünde Hibernate seçeneği | ❌ Kapalı |

> 💡 Bing aramasını kapatmak Başlat menüsünü hızlandırır ve yerel sonuçlara odaklanır.

---

### 📁 Dosya Gezgini

Dosya görünümü, gizli dosyalar ve açılış konumu.

| Ayar | Ne işe yarar | Benim ayarım |
| ---- | ------------ | ------------ |
| **Dosya uzantısını göster** | `.exe`, `.pdf` gibi uzantıları gösterir | ✅ Açık |
| **Gizli öğeleri ve sistem öğelerini göster** | Gizli dosya ve klasörleri listeler | ✅ Açık |
| **Çıkarma işlemi tamamlandıktan sonra dosyaları göster** | ZIP çıkarınca hedef klasörü açar | ❌ Kapalı |
| **Klasik Arayüz** | Eski Explorer görünümü | ❌ Kapalı |
| **Dosyalar için önizleme bölmesini göster** | Sağ panelde dosya önizlemesi | ❌ Kapalı |
| **Gezinti bölmesinde geri dönüşüm kutusunu göster** | Sol panelde çöp kutusu kısayolu | ✅ Açık |
| **Giriş** | Explorer açılış sayfası olarak Giriş | ❌ Kapalı |
| **Galeri** | Fotoğraf/video galeri görünümü | ❌ Kapalı |
| **Öğeleri seçmek için onay kutularını kullanın** | Dosya seçiminde checkbox | ❌ Kapalı |
| **Sağlayıcı bildirimlerini eşitle** | OneDrive vb. senkron bildirimleri | ✅ Açık |
| **Şununla Aç** | Explorer ilk açıldığında gidilecek yer | **Bu bilgisayar** |

> 💡 **Dosya uzantısı** açık tutmak sahte `.pdf.exe` gibi tuzak dosyaları fark etmeyi kolaylaştırır.

---

### 🛡️ Gizlilik

Microsoft'a giden kullanım ve tanılama verileri.

| Ayar | Ne işe yarar | Benim ayarım |
| ---- | ------------ | ------------ |
| **Konum** | Konum verisi paylaşımı | ❌ Kapalı |
| **Telemetri** | Tanılama ve kullanım verisi | ❌ Kapalı |
| **Müşteri Deneyimini Geliştirme Programı** | Anonim kullanım istatistikleri (CEIP) | ✅ Açık |
| **Uygulama telemetrisi** | Store uygulamalarından veri | ❌ Kapalı |
| **Uygulama izlemeyi başlat** | Başlangıç uygulaması izleme | ❌ Kapalı |
| **Çizim oluşturmayı ve yazmayı geliştirin** | El yazısı/klavye iyileştirme verisi | ❌ Kapalı |
| **Çizim oluşturmayı ve yazmayı kişiselleştirin** | Kişisel yazım profili | ❌ Kapalı |
| **Hata raporlama** | Windows Error Reporting | ✅ Açık |
| **Kilit ekranında kamera** | Kilit ekranından kamera erişimi | ❌ Kapalı |
| **Kamera açma/kapama göstergesi** | Kamera kullanım bildirimi | ❌ Kapalı |
| **Çevrimiçi konuşma tanıma** | Bulut tabanlı ses tanıma | ❌ Kapalı |

---

### 📢 Reklamlar

Windows içi öneri, ipucu ve tanıtım içerikleri - hepsi kapalı.

| Ayar | Ne işe yarar | Benim ayarım |
| ---- | ------------ | ------------ |
| **Kişiye Özel Deneyimler** | Kullanıma göre kişiselleştirilmiş öneriler | ❌ Kapalı |
| **Reklam Kimliği** | Uygulamalara özel reklam kimliği | ❌ Kapalı |
| **Ayarlarda önerilen içerik** | Ayarlar uygulamasında Microsoft önerileri | ❌ Kapalı |
| **Ayarlarda ana sayfa** | Ayarlar açılışında öneri sayfası | ❌ Kapalı |
| **Önerilen bildirimler** | İpucu ve tavsiye bildirimleri | ❌ Kapalı |
| **Kilit ekranı ipuçları** | Kilit ekranında haber/ipucu | ❌ Kapalı |
| **Windows ipuçları ve önerileri** | Sistem geneli ipuçları | ❌ Kapalı |
| **Windows'a hoş geldiniz deneyimi** | Güncelleme/oturum sonrası tanıtım | ❌ Kapalı |
| **Cihazınızın kurulumunu tamamlayın** | Kurulum hatırlatmaları | ❌ Kapalı |

> 💡 Reklam bölümünü tamamen kapatmak Windows deneyimini sadeleştirir; güncelleme bildirimleri Ayarlar → Windows Update'ten gelmeye devam eder.

---

### ⚙️ Sistem

Günlük kullanımı hızlandıran sistem davranışları.

| Ayar | Ne işe yarar | Benim ayarım |
| ---- | ------------ | ------------ |
| **Saniye cinsinden saat** | Görev çubuğu saatinde saniye | ❌ Kapalı |
| **Görevi sonlandır** | Görev çubuğu sağ tık → Görevi sonlandır | ✅ Açık |
| **Pano geçmişi** | `Win + V` ile pano geçmişi | ✅ Açık |
| **Ekran Yazdırma tuşuyla ekran görüntüsü alma** | Print Screen → Ekran Alıntısı Aracı | ✅ Açık |
| **Fare hızlandırma** | İşaretçi hassasiyeti (mouse acceleration) | ✅ Açık |
| **Num Lock varsayılan olarak açık** | Açılışta Num Lock açık | ✅ Açık |
| **Geri Bildirim Hatırlatmaları** | Windows geri bildirim bildirimleri | ❌ Kapalı |
| **Alt+Tab İçeriği** | Alt+Tab'da gösterilecek pencere sayısı | **En yeni 5 sekme** |
| **Dijital Pazarlar Yasası** | AB DMA uyumluluk seçenekleri | ❌ Kapalı |

---

### 🔐 Yetkili Kullanıcı

Güvenlik riski taşıyabilecek gelişmiş ayarlar - dikkatli kullan.

| Ayar | Ne işe yarar | Benim ayarım |
| ---- | ------------ | ------------ |
| **Tam Hakimiyet Modu (God Mode)** | Tüm Windows ayarlarına tek klasörden erişim | ❌ Kapalı |
| **Geliştirici Modu** | Yan yükleme, geliştirici araçları | ❌ Kapalı |
| **Kullanıcı Hesabı Denetimi (UAC)** | Yönetici izni uyarı seviyesi | **Yalnızca değişikliklerde (soluk)** |
| **Kullanıcı seçimi koruma sürücüsü** | Varsayılan uygulama tercihlerini korur | ✅ Açık |

**Spotlight resimleri** - Kilit ekranındaki Windows Spotlight görsellerini klasöre **Çıkart** ile dışa aktarabilirsin.

> ⚠️ **God Mode** ve **Geliştirici Modu** güvenlik yüzeyini genişletir; günlük kullanımda kapalı tutmanı öneririm. UAC'yı tamamen kapatma.

---

## ⚠️ Bilinen Sorunlar ve Çözümleri

| Sorun | Neden Olur | Çözüm |
| ----- | ---------- | ----- |
| Uygulama/servis listesi boş veya eksik | Yetersiz izin | WinToys'u yönetici olarak çalıştır; uygulamayı kapatıp tekrar aç |
| Uygulama kaldırılamıyor | Store vs Win32 farkı | Sarı/mavi renk koduna dikkat et; ⋯ → **Kaldır** dene |
| Sistem yavaşladı veya özellik bozuldu | Yanlış kapatılan hizmet | Hizmeti **Başlat** ile geri aç; gerekirse Sistem Geri Yükleme |
| İzin / erişim hatası | Registry veya sistem koruması | Yönetici olarak çalıştır; antivirüs engelini kontrol et |

---

## 🔗 Faydalı Bağlantılar

- 🌐 [Resmi Web Sitesi](https://bogdan-patraucean.github.io/about/wintoys/)
- 💾 [GitHub Releases](https://github.com/bogdandonduk/WinToys/releases)
- 📖 [Changelog](https://bogdan-patraucean.github.io/about/wintoys/changelog.html)
- ❓ [SSS](https://bogdan-patraucean.github.io/about/wintoys/faq.html)
- 🏪 [Microsoft Store](https://apps.microsoft.com/detail/9P8LTPGCBZXD)

---

## 📝 Notlar

> WinToys'ta 6 sekme vardır (Giriş, Uygulamalar, Hizmetler, Performans, Sağlık, İnce Ayarlar) - hepsi bu rehberde anlatılır. Hizmet, performans, onarım ve ince ayarlarda acele etme; her seçeneğin üzerine gelince açıklama tooltip'i görünür. İnce Ayarlar bölümündeki **Benim ayarım** sütunu kişisel kurulumu yansıtır.

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

*Son güncelleme: 2026-05-25*
