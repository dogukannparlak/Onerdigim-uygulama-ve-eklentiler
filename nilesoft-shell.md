# 🛠️ Nilesoft Shell

> **Kısa Açıklama:** Windows sağ tık menüsünü özelleştirir; gereksiz öğeleri kaldırır, kendi komutlarını ekler ve menüyü sadeleştirir.

1.9.18 · Windows 7/8/10/11 · Ücretsiz / açık kaynak · Sistem Araçları

---

## 📌 Genel Bakış

Nilesoft Shell, Dosya Gezgini, masaüstü ve görev çubuğundaki bağlam menüsünü metin tabanlı `shell.nss` dosyasıyla yönetir. Windows'un kalabalık sağ tık menüsünden kurtulmak, WinRAR/7-Zip gibi üçüncü parti girişleri düzenlemek veya tek tıkla uygulama/komut eklemek isteyenler için uygundur. Registry düzenlemek yerine okunabilir bir yapılandırma dosyası kullanır.

---

## ✨ Öne Çıkan Özellikler

- **Tam menü kontrolü** — Mevcut öğeleri gizle, sırala veya kaldır
- **Özel komutlar** — Uygulama, web sitesi veya script menüye eklenebilir
- **İç içe menüler** — Alt menü, ayırıcı ve çok sütunlu düzen
- **Win11 uyumu** — Modern ve klasik menü arasında geçiş desteği
- **Hafif çalışma** — Arka planda sürekli açık bir arayüz yok
- **Ücretsiz** — Kişisel ve ticari kullanım için bedava

---

## 📥 İndirme ve Kurulum

> Kurulum için **yönetici izni** gerekir. Kurulum sonunda Explorer'ı yeniden başlatmayı onayla.

### Yöntem 1: Resmi Site — Önerilen

1. [nilesoft.org/download](https://nilesoft.org/download) adresine git
2. **Setup x64** (veya sisteme uygun sürüm) indir
3. `setup.exe`'yi yönetici olarak çalıştır
4. Kurulum sihirbazını tamamla

Varsayılan kurulum yolu: `C:\Program Files\Nilesoft Shell\`

### Yöntem 2: WinGet (Terminal)

```powershell
winget install Nilesoft.Shell
```

> WinGet hata verirse terminali **yönetici olarak** açıp tekrar dene.

### Yöntem 3: UniGetUI

> UniGetUI açıkken arama çubuğuna **Nilesoft Shell** yaz ve kur.

---

## ⚙️ İlk Kurulum ve Önerilen Ayarlar

Kurulumdan sonra:

1. **Çalıştığını kontrol et** — Masaüstünde veya bir dosyada sağ tıkla; Shell menüsü görünmeli
2. **Yapılandırma klasörünü aç** — Görev çubuğunda **Shift + sağ tık** → Shell → **directory**
3. **`shell.nss` yedeği al** — Düzenlemeden önce dosyayı kopyala
4. **Küçük bir değişiklikle başla** — Önce tek menü öğesi ekle veya gizle

| Dosya | Konum | Açıklama |
| ----- | ----- | -------- |
| `shell.nss` | Kurulum klasörü | Ana yapılandırma |
| `imports/` | Kurulum klasörü | İçe aktarılan menü dosyaları |
| `shell.log` | Kurulum klasörü | Hata kayıtları |

> 💡 Yapılandırma dosyaları varsayılan olarak program klasöründedir; `%USERPROFILE%\.nilesoft\` yolu eski veya özel kurulumlarda kullanılabilir.

---

## 🚀 Temel Kullanım

### İlk menü öğesini ekleme

1. `shell.nss` dosyasını Not Defteri veya VS Code ile aç
2. Örnek satırı ekle:

```ini
item(title='Merhaba!' cmd=msg('Selam @user.name'))
```

3. Kaydet
4. **Ctrl + sağ tık** (masaüstü veya görev çubuğunda) ile yapılandırmayı yeniden yükle

### Menüyü yeniden yükleme

- **Ctrl + sağ tık** — Yapılandırmayı yükle
- **Sağ tık + sol tık** — Alternatif yenileme
- Komut satırı: `shell -restart` (Explorer'ı yeniden başlatır)

### Klavye kısayolları

Sağ tık veya **Shift + F10** sırasında:

| Kısayol | İşlev |
| ------- | ----- |
| `Ctrl` + sağ tık | Shell'i etkinleştir ve `shell.nss`'yi yeniden yükle |
| `Win` + sağ tık | Win11 modern menüye öncelik ver |
| `Ctrl + Win` + sağ tık | Shell'i geçici kapat, klasik menüyü kullan |

---

## ⚠️ Bilinen Sorunlar ve Çözümleri

| Sorun | Neden Olur | Çözüm |
| ----- | ---------- | ----- |
| Menü görünmüyor | Kayıt veya sözdizimi hatası | `shell -register -restart` çalıştır; `shell.log` dosyasını kontrol et |
| Değişiklikler yansımıyor | Yapılandırma yenilenmemiş | **Ctrl + sağ tık** ile yeniden yükle |
| WinGet kurulumu başarısız | Yönetici izni yok | Terminali yönetici olarak aç |
| Win11'de farklı menü | Modern bağlam menüsü | `Win + sağ tık` ile modern menü; `Ctrl + Win` ile Shell'i kapat |
| Explorer sorunu | Hatalı `shell.nss` | Yedeği geri yükle veya `shell -unregister -restart` ile kaldır |

---

## 🔗 Faydalı Bağlantılar

- 🌐 [Resmi Web Sitesi](https://nilesoft.org/)
- 📥 [İndirme Sayfası](https://nilesoft.org/download)
- 📖 [Başlangıç Rehberi](https://nilesoft.org/docs/get-started)
- 📖 [Yapılandırma Dokümantasyonu](https://nilesoft.org/docs/configuration)
- 💾 [GitHub Sayfası](https://github.com/moudey/shell)

---

## 📝 Notlar

> Nilesoft Shell sistem genelinde sağ tık menüsüne müdahale eder; StartAllBack, ExplorerBlurMica veya başka bağlam menüsü araçlarıyla çakışma olabilir. Gelişmiş özelleştirme NSS sözdizimi gerektirir — karmaşık menüler için resmi dokümantasyona bak. Resmi siteden indirmek önerilir; üçüncü parti paketlerde istenmeyen yazılım bulunabilir.

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
