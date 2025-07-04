# Everything

## Everything Nedir?

**Everything**, Windows işletim sistemi için geliştirilmiş, dosya ve klasörleri dosya adına göre **anlık** olarak bulan güçlü bir arama motorudur. Windows’un yerleşik arama özelliğinin aksine, Everything başlangıçta bilgisayarınızdaki tüm dosya ve klasörleri görüntüler (bu nedenle adı “Everything”).

### Ana Avantajları:

- ⚡ **Anlık arama** - Yazarken sonuçlar gerçek zamanlı görünür
- 💾 **Minimal kaynak kullanımı** - Çok az RAM ve disk alanı
- 🔄 **Gerçek zamanlı güncelleme** - Dosya sistemi değişikliklerini otomatik izler
- 🆓 **Tamamen ücretsiz** - Reklam, malware veya spyware içermez
- 🎯 **Yüksek doğruluk** - NTFS dosya sistemi entegrasyonu

---

## Özellikler

### 🚀 Temel Özellikler

- **Anlık indeksleme**: Yeni Windows 10 kurulumu (~120,000 dosya) yaklaşık 1 saniyede indekslenir
- **Gerçek zamanlı izleme**: Dosya sistemi değişiklikleri anlık olarak yansıtılır
- **Boolean operatörler**: AND, OR, NOT işlemleri ile gelişmiş arama
- **Joker karakterler**:  ve `?` karakterleri ile esnek arama
- **İçerik arama**: `content:` fonksiyonu ile dosya içeriği arama

### 📊 Performans Bilgileri

| Dosya Sayısı | İndeksleme Süresi | RAM Kullanımı | Disk Kullanımı |
| --- | --- | --- | --- |
| 120,000 | ~1 saniye | ~14 MB | <9 MB |
| 1,000,000 | ~1 dakika | ~75 MB | ~45 MB |

### 🛠️ Desteklenen Dosya Sistemleri

- **NTFS**: Tam otomatik indeksleme (önerilen)
- **FAT/FAT32/exFAT**: Manuel ekleme gerekli
- **Ağ sürücüleri**: Desteklenir (özel konfigürasyon gerekebilir)

---

## Sistem Gereksinimleri

### NTFS İndeksleme Gereksinimleri

NTFS indeksleme için aşağıdakilerden biri gerekli:
- Everything Servisinin kurulu olması **VEYA**
- Everything’in yönetici olarak çalıştırılması

---

## Kurulum

### 🔽 İndirme ve Kurulum

1. [Voidtools resmi sitesinden](https://www.voidtools.com/) Everything’i indirin
2. Kurulum dosyasını çalıştırın
3. **Lite versiyonu** seçenekleri:
    - Normal versiyon: Tüm özellikler dahil
    - Lite versiyon: ETP/FTP sunucu, HTTP sunucu ve IPC özellikleri kaldırılmış

### ⚙️ İlk Kurulum Ayarları

### Önerilen Ayarlar:

```
Tools → Options → General:
☑️ Store settings and data in %APPDATA%\Everything
☑️ Everything Service
☐ Run as administrator
```

Bu ayarlar:
- UAC (Kullanıcı Hesabı Denetimi) uyarılarını engeller
- Servis olarak çalışarak sürekli erişim sağlar
- Standart kullanıcı olarak güvenli çalışma

---

## Kullanım Rehberi

### 🔍 Temel Arama

Arama kutusuna yazmaya başladığınızda sonuçlar anında görünür:

```
# Örnekler:
document        # "document" içeren tüm dosyalar
*.pdf           # Tüm PDF dosyaları
photo 2023      # Hem "photo" hem "2023" içeren dosyalar
```

### 📁 Konum Bazlı Arama

Belirli bir konumda arama yapmak için:

```
downloads\ .mp3          # Downloads klasöründeki MP3 dosyaları
c:\users\yourname\ .txt  # Kullanıcı klasöründeki TXT dosyaları
```

**Alternatif**: `Search → Match Path` seçeneğini etkinleştirin:

```
downloads .mp3   # Match Path aktifken
```

---

## Arama Teknikleri

### 🔤 Boolean Operatörleri

### AND (Varsayılan)

```
photo vacation    # Hem "photo" hem "vacation" içeren dosyalar
```

### OR (|)

```
.jpg | .png | .gif    # JPG, PNG veya GIF dosyaları
report | document     # "report" VEYA "document" içeren dosyalar
```

### NOT (!)

```
!temp             # "temp" içermeyen dosyalar
photo !backup     # "photo" içeren ama "backup" içermeyen dosyalar
```

### 🃏 Joker Karakterler

### Asterisk (*) - Çoklu karakter

```
e*g              # "e" ile başlayıp "g" ile biten dosyalar
*.??             # 2 karakterli uzantısı olan dosyalar
report*2023      # "report" ile başlayıp "2023" içeren dosyalar
```

### Soru işareti (?) - Tek karakter

```
photo?.jpg       # photo1.jpg, photoA.jpg gibi
test??.txt       # test01.txt, testAB.txt gibi
```

### 📝 Dosya Türü Arama

```
# Ses dosyaları
*.mp3 | *.wav | *.flac

# Video dosyaları
*.mp4 | *.avi | *.mkv

# Resim dosyaları
*.jpg | *.png | *.gif | *.bmp

# Doküman dosyaları
*.pdf | *.doc | *.docx | *.txt
```

### 🔍 İçerik Arama

```
content:password     # İçeriğinde "password" geçen dosyalar
content:"API key"    # İçeriğinde "API key" geçen dosyalar
```

⚠️ **Not**: İçerik arama indekslenmez, bu yüzden yavaştır.

### 📏 Boyut Arama

```
size:>1GB           # 1 GB'dan büyük dosyalar
size:<100MB         # 100 MB'dan küçük dosyalar
size:500KB..2MB     # 500 KB ile 2 MB arası dosyalar
```

### 📅 Tarih Arama

```
# Oluşturulma tarihi
created:today
created:yesterday
created:thisweek
created:2023

# Değiştirilme tarihi
modified:today
modified:lastyear

# Erişim tarihi
accessed:thismonth
```

---

## Gelişmiş Özellikler

### 🎛️ Filtreler

Everything’de önceden tanımlı filtreler:

```
# Ana filtreler
Everything    # Tüm dosyalar (varsayılan)
Audio        # Ses dosyaları
Video        # Video dosyaları
Picture      # Resim dosyaları
Document     # Doküman dosyaları
```

### 🔧 Özel Filtreler Oluşturma

```
Tools → Options → Filters → Add...

# Örnek: Geliştirme dosyaları filtresi
Name: Dev Files
Search: *.js | *.css | *.html | *.php | *.py
```

### 📊 Sıralama Seçenekleri

```
# Sıralama kriterleri
Ctrl+1    # İsme göre
Ctrl+2    # Boyuta göre
Ctrl+3    # Türe göre
Ctrl+4    # Değiştirilme tarihine göre
Ctrl+5    # Oluşturulma tarihine göre
```

---

## Everything Toolbar

Everything Toolbar, Everything’in işlevselliğini Windows görev çubuğuna entegre eden açık kaynak bir projedir.

### 📦 Kurulum

1. [GitHub sayfasından](https://github.com/srwi/EverythingToolbar) en son sürümü indirin
2. MSI dosyasını çalıştırarak kurun
3. Görev çubuğında sağ tıklayıp **Toolbars → EverythingToolbar** seçin

### ✨ Özellikler

- 🔍 **Görev çubuğı entegrasyonu**: Doğrudan görev çubuğundan arama
- ⌨️ **Klavye kısayolları**: Hızlı erişim için özelleştirilebilir
- 🎨 **Tema desteği**: Windows tema ile uyumlu
- 🔧 **Özelleştirilebilir**: Genişlik, pozisyon ve davranış ayarları

### ⌨️ Varsayılan Kısayollar

```
Win + Alt + S     # Everything Toolbar'a odaklan
Escape           # Arama kutusunu temizle
Enter            # İlk sonucu aç
Ctrl + Enter     # Klasörü aç
```

### ⚙️ Yapılandırma

```
# Toolbar ayarları
- Genişlik: Piksel cinsinden ayarlanabilir
- Placeholder metin: Özelleştirilebilir
- Otomatik tamamlama: Etkinleştirilebilir
- Sonuç sayısı: Gösterilecek maksimum sonuç
```

---

## Sık Sorulan Sorular

### ❓ Genel Sorular

**S: Everything ne kadar güvenlidir?**
C: Everything tamamen güvenlidir. Malware, spyware veya adware içermez. Açık kaynak topluluk tarafından incelenir.

**S: Everything kapalıyken yapılan değişiklikler kaçırılır mı?**
C: Hayır. NTFS USN Journal sayesinde Everything kapalıyken bile değişiklikler sistem tarafından kaydedilir.

**S: Neden Everything Windows arama özelliğinden daha hızlı?**
C: Everything sadece dosya adlarını indeksler, içeriklerini değil. NTFS Master File Table’ı doğrudan okur.

### 🔧 Teknik Sorular

**S: UAC uyarılarından nasıl kurtulabilirim?**
C: Everything Service’i yükleyin ve “Run as administrator” seçeneğini kapatın:

```
Tools → Options → General:
☑️ Everything Service
☐ Run as administrator
```

**S: FAT/FAT32 diskleri nasıl indekslerim?**
C: Manuel olarak eklemeniz gerekir:

```
Tools → Options → Folders → Add...
```

**S: Ağ sürücüleri neden görünmüyor?**
C: Everything’i standart kullanıcı olarak çalıştırmayı deneyin:

```
Tools → Options → General:
☑️ Everything Service
☐ Run as administrator
```

---

## Performans ve Optimizasyon

### ⚡ Hızlandırma İpuçları

1. **SSD kullanın**: Özellikle Everything veritabanı için
2. **NTFS kullanın**: FAT32’den çok daha hızlı
3. **Servis modunu kullanın**: Sürekli çalışır durumda
4. **Gereksiz klasörleri hariç tutun**: Temp, cache klasörleri gibi

```
# Hariç tutulacak klasörler örneği
Tools → Options → Exclude:
C:\Windows\Temp\
C:\Users\*\AppData\Local\Temp\
C:\$Recycle.Bin\
```

### 📈 İndeksleme Optimizasyonu

```
# NTFS volumes için otomatik ayarlar
Tools → Options → NTFS:
☑️ Include in database
☑️ Monitor changes
☑️ Enable USN Journal on volume
```

---