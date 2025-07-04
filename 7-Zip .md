# 7-Zip

---

## 🎯 Genel Bakış

### Araç Hakkında

7-Zip, Igor Pavlov tarafından geliştirilen ücretsiz ve açık kaynaklı bir dosya arşivleyicidir. Yüksek sıkıştırma oranları, güçlü AES-256 şifreleme desteği ve geniş format yelpazesi ile öne çıkar. Windows, Linux ve macOS platformlarında çalışır.

### Temel Özellikler

- ✅ **Yüksek Sıkıştırma Oranı**: 7z formatında %30-70 daha iyi sıkıştırma
- ✅ **Çok Format Desteği**: 60+ arşiv formatını okuyabilir
- ✅ **Güçlü Şifreleme**: AES-256 bit şifreleme desteği
- ✅ **Ücretsiz ve Açık Kaynak**: Reklamsız ve güvenilir
- ✅ **Düşük RAM Kullanımı**: Hafıza dostu çalışma
- ✅ **Komut Satırı Desteği**: Otomasyon ve toplu işlemler

## 🚀 Kurulum ve Başlangıç

### Kurulum Yöntemleri

### 1️⃣ Resmi Web Sitesinden İndirme (Önerilen)

1. https://www.7-zip.org adresine gidin
2. İşletim sisteminize uygun sürümü seçin:
    - **64-bit Windows**: `7z2301-x64.exe`
    - **32-bit Windows**: `7z2301.exe`
3. İndirilen dosyayı çalıştırın ve kurulum talimatlarını takip edin

### 2️⃣ Winget ile Kurulum

```
winget install 7zip.7zip
```

### 3️⃣ Chocolatey ile Kurulum

```
choco install 7zip
```

### ⚠️ Kurulum Notları

**✅ ÖNERİLER**:
- Windows File Explorer entegrasyonu için “Associate 7-Zip with file extensions” seçeneğini işaretleyin
- Sistem PATH’ine ekleme seçeneğini aktif edin
- Düzenli güncellemeleri takip edin

## 🖥️ Komut Satırı Kullanımı

### 📋 Temel Komut Yapısı

```
7z <komut> <anahtarlar> <arşiv> <dosyalar>
```

### 🔧 Ana Komutlar

| Komut | Açıklama | Örnek |
| --- | --- | --- |
| **a** | Arşiv oluştur/ekle | `7z a backup.7z *.txt` |
| **x** | Tam yol ile çıkar | `7z x backup.7z` |
| **e** | Çıkar (yol olmadan) | `7z e backup.7z` |
| **l** | İçeriği listele | `7z l backup.7z` |
| **t** | Arşivi test et | `7z t backup.7z` |
| **u** | Güncelle | `7z u backup.7z newfile.txt` |
| **d** | Sil | `7z d backup.7z oldfile.txt` |

### ⚙️ Önemli Anahtarlar

| Anahtar | Açıklama | Örnek |
| --- | --- | --- |
| **-t{type}** | Arşiv formatı | `-tzip`, `-t7z` |
| **-mx{level}** | Sıkıştırma seviyesi | `-mx9` (ultra) |
| **-p{password}** | Şifre | `-pmypassword` |
| **-y** | Tüm sorulara evet | Otomasyon için |
| **-o{dir}** | Çıkarma dizini | `-oc:\extract` |
| **-r** | Alt klasörler dahil | Recursive işlem |

### 💡 Pratik Örnekler

### Şifreli Arşiv Oluşturma:

```
7z a -p secret.7z documents\
```

### Split Arşiv Oluşturma:

```
7z a -v100m backup.7z folder\
```

### Test ve Onarım:

```
7z t backup.7z
7z x backup.7z -y
```

### Toplu İşlem:

```
for %f in (*.zip) do 7z x "%f" -o"%~nf"
```

## 💻 Temel İşlemler

### 🗂️ Dosya Sıkıştırma

### Sağ Tık Menüsü ile Hızlı Sıkıştırma:

| Seçenek | Açıklama | Kullanım Senaryosu |
| --- | --- | --- |
| **Add to “filename.7z”** | 7z formatında sıkıştır | En yüksek sıkıştırma |
| **Add to “filename.zip”** | ZIP formatında sıkıştır | Uyumluluk için |
| **Add to archive…** | Detaylı ayarlarla sıkıştır | Özelleştirme gerekli |

### 7-Zip File Manager ile Sıkıştırma:

1. **7-Zip File Manager**’ı açın
2. Sıkıştırılacak dosyaları seçin
3. **Add** butonuna tıklayın
4. Sıkıştırma ayarlarını yapılandırın:

| Ayar | Açıklama | Önerilen Değer |
| --- | --- | --- |
| **Archive Format** | Arşiv formatı | 7z (en iyi sıkıştırma) |
| **Compression Level** | Sıkıştırma seviyesi | Normal (varsayılan) |
| **Split to volumes** | Bölümlere ayırma | Büyük dosyalar için |

### 📁 Dosya Açma/Çıkarma

### Sağ Tık Menüsü ile Hızlı Çıkarma:

| Seçenek | Açıklama | Sonuç |
| --- | --- | --- |
| **Extract Here** | Mevcut konuma çıkar | Dosyalar aynı klasöre |
| **Extract to “foldername”** | Yeni klasöre çıkar | Düzenli çıkarma |
| **Extract files…** | Detaylı ayarlarla çıkar | Hedef seçimi |

### Çıkarma Ayarları:

| Ayar | Açıklama | Kullanım |
| --- | --- | --- |
| **Extract to** | Hedef klasör | Dosya organizasyonu |
| **Overwrite mode** | Üzerine yazma | Mevcut dosyalar için |
| **Path mode** | Yol yapısı | Klasör hiyerarşisi |

### 🔍 Arşiv İçeriğini Görüntüleme

7-Zip arşivleri Windows Explorer’da klasör gibi görüntülenebilir:

- **Çift tıklama**: Arşivi 7-Zip File Manager’da aç
- **Enter tuşu**: Seçili dosyayı geçici olarak çıkar ve aç
- **F3 tuşu**: İç görüntüleyici ile dosyayı göster

## ⚙️ Gelişmiş Özellikler

### 🔄 Çok Parçalı Arşivler

Büyük dosyaları bölmek için:

1. **Split to volumes** seçeneğini işaretleyin
2. Parça boyutunu belirleyin:

| Boyut | Kullanım Alanı |
| --- | --- |
| **1.44 MB** | Floppy disk (eski) |
| **650 MB** | CD |
| **4.7 GB** | DVD |
| **25 GB** | Blu-ray |
| **Özel** | USB, email limit |

### 🧩 Solid Arşivleme

Solid arşivleme benzer dosyaları daha iyi sıkıştırır:

**Avantajları:**
- ✅ Daha yüksek sıkıştırma oranı
- ✅ Benzer dosyalar için ideal

**Dezavantajları:**
- ❌ Tek dosya çıkarma yavaş
- ❌ Corrupt olma riski yüksek

## 🔐 Şifreleme ve Güvenlik

### 🛡️ Şifreleme Yöntemleri

7-Zip iki şifreleme algoritması destekler:

| Algoritma | Anahtar Boyutu | Güvenlik |
| --- | --- | --- |
| **AES-256** | 256 bit | ⭐⭐⭐⭐⭐ |
| **ZipCrypto** | 96 bit | ⭐⭐ |

### 🗃️ Dosya Adı Şifreleme

7z formatında dosya adları da şifrelenebilir:

1. **Add to archive** seçeneğini kullanın
2. **Encryption** bölümünde:
    - **Encrypt file names** seçeneğini işaretleyin
    - Bu durumda arşiv içeriği görünmez