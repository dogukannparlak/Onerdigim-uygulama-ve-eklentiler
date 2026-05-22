# 🛠️ 7-Zip

> **Kısa Açıklama:** Yüksek sıkıştırma oranı ve geniş format desteği sunan ücretsiz, açık kaynaklı dosya arşivleyici.

Güncel · Windows, Linux, macOS · Açık kaynak (LGPL) · Sistem Araçları

---

## 📌 Genel Bakış

7-Zip, Igor Pavlov tarafından geliştirilen ücretsiz bir arşiv yöneticisidir. Windows'un yerleşik ZIP desteğine kıyasla daha yüksek sıkıştırma (özellikle 7z formatında), AES-256 şifreleme ve 60'tan fazla arşiv formatını açma imkânı sunar. Reklamsızdır ve düşük bellek kullanır.

---

## ✨ Öne Çıkan Özellikler

- **Yüksek sıkıştırma** — 7z formatında güçlü oran; ZIP/RAR/TAR ve daha fazlasını açar
- **AES-256 şifreleme** — Arşivlere parola koruması
- **Explorer entegrasyonu** — Sağ tık menüsünden sıkıştır/çıkar
- **Komut satırı** — `7z` ile otomasyon ve toplu işlem
- **Ücretsiz ve açık kaynak** — Reklamsız, güvenilir
- **Düşük RAM** — Hafif çalışma

---

## 📥 İndirme ve Kurulum

### Yöntem 1: Resmi Site ( Önerilen )

1. [7-zip.org](https://www.7-zip.org/) adresine git
2. **Download** bölümünden **64-bit Windows x64** kurulum dosyasını indir
3. İndirilen `.exe` dosyasını çalıştır ve kurulum sihirbazını takip et
4. Kurulumda **Associate 7-Zip with file extensions** seçeneğini işaretle

> 32-bit sistem kullanıyorsan sitedeki 32-bit sürümü seç.

### Yöntem 2: WinGet (Terminal)

```powershell
winget install 7zip.7zip
```

### Yöntem 3: UniGetUI

> UniGetUI açıkken arama çubuğuna **7-Zip** yaz ve kur.

### Yöntem 4: Chocolatey

```powershell
choco install 7zip
```

---

## ⚙️ İlk Kurulum ve Önerilen Ayarlar

1. **Dosya ilişkilendirme:** `.7z`, `.zip`, `.rar` gibi uzantıları 7-Zip ile aç (kurulumda veya 7-Zip → Tools → Options → System).
2. **PATH (isteğe bağlı):** Komut satırından `7z` kullanmak için kurulumda PATH'e ekleme seçeneğini aç.
3. **Varsayılan format:** En iyi sıkıştırma için `.7z`; paylaşım/uyumluluk için `.zip` tercih et.

> 💡 **İpucu:** Şifreli arşivlerde **AES-256** kullan; eski ZipCrypto zayıftır.

---

## 🚀 Temel Kullanım

### Sağ tık ile sıkıştırma

1. Dosya veya klasöre sağ tıkla
2. **7-Zip** → **Add to "dosya.7z"** (en iyi sıkıştırma) veya **Add to "dosya.zip"** (uyumluluk)
3. Detaylı ayar için **Add to archive…** → format, seviye ve parola belirle

### Sağ tık ile çıkarma

1. Arşiv dosyasına sağ tıkla
2. **7-Zip** → **Extract Here** (mevcut klasöre) veya **Extract to "klasör** (yeni klasöre)

### Komut satırı (temel)

```powershell
7z a yedek.7z C:\Belgeler\proje\    # Arşiv oluştur
7z x yedek.7z -oC:\cikti\            # Çıkar
7z t yedek.7z                        # Arşivi test et
```

---

## ⚠️ Bilinen Sorunlar ve Çözümleri


| Sorun              | Neden Olur                   | Çözüm                                                                                |
| ------------------ | ---------------------------- | ------------------------------------------------------------------------------------ |
| Arşiv açılmıyor    | Bozuk dosya veya eksik parça | `7z t arsiv.7z` ile test et; split arşivde tüm parçaların olduğundan emin ol         |
| Sağ tık menüsü yok | İlişkilendirme kapalı        | 7-Zip → Tools → Options → System → ilişkilendirmeyi aç                               |
| Yanlış parola      | Hatalı şifre                 | Parolayı kontrol et; AES-256 ile oluşturulmuş arşivlerde büyük/küçük harf duyarlıdır |


---

## 🔗 Faydalı Bağlantılar

- 🌐 [Resmi Web Sitesi](https://www.7-zip.org/)
- 📥 [İndirme Sayfası](https://www.7-zip.org/download.html)
- 📖 [Komut Satırı Kılavuzu](https://www.7-zip.org/faq.html)

---

## 📝 Notlar

> 7-Zip salt arşivleme aracıdır; bulut yedekleme veya senkronizasyon sunmaz. Paylaşılan arşivlerde `.zip` daha evrensel kabul görür; kişisel yedeklerde `.7z` daha iyi sıkıştırır. Şifre unutulursa arşiv kurtarılamaz — parolayı güvenli bir yerde sakla.

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