# nilesoft-shell

# 🎯 Genel Bakış

---

### Araç Hakkında

**Nilesoft Shell**, Windows Dosya Gezgini için güçlü bir bağlam menüsü (sağ tık menüsü) yöneticisidir. Bu araç, standart Windows sağ tık menüsünü tamamen özelleştirmenize, yeni özel komutlar eklemenize ve mevcut menü öğelerini değiştirmenize veya kaldırmanıza olanak tanır.

### Ana Avantajları

- 🎨 **Tam Özelleştirme**: Menü görünümünü istediğiniz gibi tasarlayın
- ⚡ **Hafif ve Hızlı**: Minimal sistem kaynağı kullanımı
- 🛠️ **Güçlü Komut Desteği**: Uygulama başlatma, dosya işlemleri, sistem komutları
- 🌐 **Web Entegrasyonu**: Favori web sitelerinizi menüye entegre edin
- 🔧 **Sistem Yönetimi**: Üçüncü taraf menü öğelerini kontrol edin
- 📁 **Evrensel Destek**: Dosyalar, klasörler, masaüstü ve görev çubuğu için
- 🎯 **İfade Sistemi**: Yerleşik fonksiyonlar ve değişkenler
- 🔍 **Arama ve Filtreleme**: Menü öğelerini organize edin

---

## 🚀 Kurulum ve Başlangıç

### Kurulum

### Resmi Web Sitesinden İndirme

```
📥 Resmi İndirme:
1. https://nilesoft.org/download adresine gidin
2. En son sürümü seçin (v1.9.8+)
3. Setup dosyasını indirin
4. Yönetici olarak çalıştırın
```

## ⚙️ İlk Yapılandırma

### Kurulum Sonrası Adımlar

```
🚀 İlk Kurulum Kontrolleri:
1. ✅ Shell menüsünün çalıştığını kontrol edin
2. ✅ Varsayılan yapılandırma dosyasını inceleyin
3. ✅ Yedek oluşturun
4. ✅ Temel özelleştirmeleri yapın
```

### Varsayılan Dosya Konumları**(olmayabilir siz oluşturun)**

| Dosya | Konum | Açıklama |
| --- | --- | --- |
| **shell.nss** | `%USERPROFILE%\.nilesoft\shell\` | Ana yapılandırma |
| **imports.nss** | `%USERPROFILE%\.nilesoft\shell\` | İçe aktarılan menüler |
| **default.nss** | `%PROGRAMFILES%\Nilesoft\Shell\` | Varsayılan ayarlar |
| **themes.nss** | `%USERPROFILE%\.nilesoft\shell\` | Tema tanımları |

## 🛠️ Sorun Giderme

### ❌ Yaygın Sorunlar ve Çözümleri

### 1. Menü Görünmüyor

```bash
# Çözüm adımları:1. Shell servisinin çalışıp çalışmadığını kontrol edin
2. Yapılandırma dosyasında sözdizimi hatası var mı kontrol edin
3. Shell'i yeniden başlatın:   
- shell.exe -r (restart)   
- shell.exe -reload
```

### 2. Yönetici İzni Sorunları

```bash
# UAC sorunları için:
1. Shell'i yönetici olarak çalıştırın
2. UAC'ı geçici olarak devre dışı bırakın
3. Kullanıcı hesabı ayarlarını kontrol edin
```