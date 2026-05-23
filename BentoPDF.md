# 🛠️ BentoPDF

> **Kısa Açıklama:** Dosyalarını sunucuya yüklemeden tarayıcıda PDF birleştirme, bölme, sıkıştırma ve dönüştürme yapan gizlilik odaklı araç seti.

2.8.4 · Web (tarayıcı) · Açık kaynak (AGPL) · PDF Araçları

---

## 📌 Genel Bakış

BentoPDF, 50'den fazla PDF aracını tek çatı altında sunan, gizlilik odaklı bir web uygulamasıdır. İşlemler tarayıcında (client-side) gerçekleşir; dosyalar sunucuya yüklenmez. Kayıt, limit veya filigran olmadan ücretsiz kullanılabilir. SumatraPDF gibi salt okuma araçlarının yerine geçmez; PDF düzenleme ve işleme ihtiyaçları için tamamlayıcıdır.

---

## ✨ Öne Çıkan Özellikler

- **Gizlilik odaklı** - Dosyalar cihazında işlenir, sunucuya yüklenmez
- **Kayıt gerekmez** - Anında kullanım, hesap açma yok
- **Ücretsiz ve sınırsız** - Araç limiti veya deneme süresi yok
- **50+ araç** - Birleştir, böl, sıkıştır, dönüştür, şifrele ve daha fazlası
- **Toplu işlem** - Birden fazla PDF'i tek seferde işle
- **Türkçe arayüz** - Dil seçenekleri arasında Türkçe desteği

---

## 📥 İndirme ve Kurulum

### Yöntem 1: Resmi Site ( Önerilen )

Kurulum gerekmez; tarayıcıdan kullanılır.

1. [bentopdf.com](https://www.bentopdf.com/) adresine git
2. İhtiyacın olan aracı seç (ör. Merge PDFs, Compress PDF)
3. Dosyayı sürükle veya seç - işlem tarayıcıda gerçekleşir
4. Sonucu indir

> Chrome, Edge, Firefox ve mobil tarayıcılarda çalışır. Sayfa yüklendikten sonra çevrimdışı kullanım da mümkündür.

### Yöntem 2: Self-Host - İsteğe Bağlı

Kendi sunucunda, şirket ağında veya air-gap ortamda çalıştırmak isteyenler için BentoPDF self-host destekler. Detaylı adımlar için [GitHub deposuna](https://github.com/alam00000/bentopdf) bak.

| Yöntem | Gereksinim | Kısa açıklama |
| ------ | ---------- | ------------- |
| **Kaynak koddan** | Node.js v18+, npm (veya yarn/pnpm) | Repoyu klonla, bağımlılıkları kur, geliştirme veya build al |
| **Docker** | Docker ve Docker Compose | Hazır imaj ile hızlı kurulum; otomatik yeniden başlatma için Compose önerilir |

> Self-host kurulumu, geliştirme ortamı ve Docker komutları için: [github.com/alam00000/bentopdf](https://github.com/alam00000/bentopdf) → **Getting Started**

---

## ⚙️ İlk Kurulum ve Önerilen Ayarlar

1. **Resmi site kullan:** Hassas belgeler için [bentopdf.com](https://www.bentopdf.com/) veya kendi self-host kurulumun tercih et; üçüncü parti kopyalardan kaçın.
2. **Araç seçimi:** Ana sayfadan kategoriye göre araç seç veya arama kutusunu kullan.
3. **Ayarlar (isteğe bağlı):** Simge menüsünden dil, tam genişlik veya kompakt görünüm ayarlanabilir.

> 💡 **İpucu:** SumatraPDF ile birlikte kullan - okuma için SumatraPDF, birleştirme/sıkıştırma/dönüştürme için BentoPDF.

---

## 🚀 Temel Kullanım

### PDF birleştirme örneği

1. [bentopdf.com](https://www.bentopdf.com/) → **Merge PDFs** aracını aç
2. PDF dosyalarını sürükle veya seç
3. Sıralamayı ayarla → işlemi başlat
4. Birleştirilmiş PDF'i indir

### Araç kategorileri (özet)

| Kategori | Örnek araçlar |
| -------- | ------------- |
| **Organize** | Birleştir, böl, sayfa düzenle, döndür |
| **Edit** | Not ekle, redaksiyon, filigran, form doldur |
| **Convert** | Resim/Office → PDF, PDF → resim/metin, OCR |
| **Secure** | Şifrele, sıkıştır, imzala, metadata temizle |

---

## ⚠️ Bilinen Sorunlar ve Çözümleri


| Sorun | Neden Olur | Çözüm |
| ----- | ---------- | ----- |
| İşlem yavaş | Çok büyük veya çok sayıda PDF | Dosyayı parçala; daha az dosyayla dene |
| Tarayıcı donuyor | Bellek limiti | Sekmeyi kapat, tarayıcıyı yenile; daha küçük dosyalar kullan |
| Office dönüşümü başarısız | Karmaşık belge veya tarayıcı kısıtı | Basit dosyayla test et; farklı tarayıcı dene |


---

## 🔗 Faydalı Bağlantılar

- 🌐 [Resmi Web Sitesi](https://www.bentopdf.com/)
- 💾 [GitHub Sayfası](https://github.com/alam00000/bentopdf)
- 📖 [Dokümantasyon](https://github.com/alam00000/bentopdf#documentation)

---

## 📝 Notlar

> BentoPDF web tabanlıdır; çoğu kullanıcı için [bentopdf.com](https://www.bentopdf.com/) yeterlidir. Self-host seçenekleri (Node.js, Docker) yukarıdaki **Yöntem 2** bölümünde özetlenmiştir. Bazı gelişmiş özellikler harici WASM modüllerini (CDN üzerinden) yükleyebilir. AGPL-3.0 lisanslıdır; ticari kapalı kaynak kullanım için lisans koşullarını incele.

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
