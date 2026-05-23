# 🛠️ Buster: Captcha Solver for Humans

> **Kısa Açıklama:** reCAPTCHA sesli doğrulamalarını konuşma tanıma ile çözerek zor CAPTCHA ekranlarını geçmene yardımcı olur.

3.1.3 (Nisan 2026) · Chrome, Edge, Firefox · Açık kaynak · Web Araçları

---

## 📌 Genel Bakış

Buster, reCAPTCHA widget'ındaki sesli doğrulama (audio challenge) adımlarını otomatik tamamlamaya çalışır. Görme, bilişsel veya cihaz kısıtları nedeniyle CAPTCHA'larda zorlanan kullanıcılar için tasarlanmıştır. Her CAPTCHA'nın çözüleceği garanti edilmez; teknolojinin sınırları vardır.

---

## ✨ Öne Çıkan Özellikler

- **reCAPTCHA sesli çözüm** - Audio challenge'ı konuşma tanıma ile tamamlamaya çalışır
- **Tek tık kullanım** - reCAPTCHA widget'ının altındaki Buster düğmesine bas
- **İstemci uygulaması (isteğe bağlı)** - Başarı oranını artırmak için Windows, Linux ve macOS desteği
- **Çoklu tarayıcı** - Chrome, Edge ve Firefox
- **Gizlilik odaklı** - Geliştirici kişisel veri toplamadığını belirtir
- **Açık kaynak** - Kod GitHub'da incelenebilir

---

## 📥 İndirme ve Kurulum

### Chrome Web Store

1. [Buster sayfasına git](https://chromewebstore.google.com/detail/buster-captcha-solver-for/mpbjkejclgfgadiemmefgebjfooflfhl)
2. **Chrome'a ekle** butonuna tıkla
3. İzinleri onayla ve kurulumu tamamla
4. CAPTCHA çıkan bir sitede reCAPTCHA widget'ının altında Buster düğmesini gör

> Edge kullanıyorsan Chrome Web Store bağlantısı üzerinden eklenti mağazasına yönlendirilirsin.

### Firefox Add-ons

1. [Buster - Firefox Add-ons](https://addons.mozilla.org/tr/firefox/addon/buster-captcha-solver/) sayfasına git
2. **Firefox'a ekle** butonuna tıkla
3. İzinleri onayla ve kurulumu tamamla

### İstemci uygulaması (isteğe bağlı)

1. Eklenti simgesine tıkla → **Seçenekler**
2. İstemci uygulaması talimatlarını takip et
3. Windows, Linux veya macOS'a kur

---

## ⚙️ İlk Kurulum ve Önerilen Ayarlar

1. **Temel kullanım:** Önce eklenti tek başına dene; yeterli değilse istemci uygulamasını kur.
2. **Sesli challenge erişimi:** Bazı siteler audio challenge'ı gizler; [wiki rehberine](https://github.com/dessant/buster/wiki/Inaccessible-reCAPTCHA-audio-challenge) bak.
3. **Sık kullanım:** Günde birkaçtan fazla reCAPTCHA çözmek geçici engellemeye yol açabilir; mümkün olduğunca az kullan.

> 💡 **İpucu:** Hata ve özellik istekleri için Chrome Web Store yorumları izlenmez; [GitHub Issues](https://github.com/dessant/buster) kullan.

---

## 🚀 Temel Kullanım

### reCAPTCHA geçme

1. CAPTCHA içeren bir siteye git
2. reCAPTCHA widget'ı yüklensin
3. Widget'ın altındaki **Buster** düğmesine tıkla
4. Eklenti sesli doğrulamayı otomatik tamamlamaya çalışır; başarısız olursa tekrar dene veya manuel çöz

---

## ⚠️ Bilinen Sorunlar ve Çözümleri


| Sorun               | Neden Olur                                      | Çözüm                                                                                                              |
| ------------------- | ----------------------------------------------- | ------------------------------------------------------------------------------------------------------------------ |
| CAPTCHA çözülmüyor  | Sesli challenge erişilemiyor veya tanıma hatası | Wiki rehberini kontrol et; istemci uygulamasını kur                                                                |
| Geçici engelleme    | Günde çok fazla reCAPTCHA çözümü                | Bir süre bekle; kullanımı sınırla                                                                                  |
| Audio challenge yok | Site sesli seçeneği gizlemiş olabilir           | [Inaccessible audio challenge wiki](https://github.com/dessant/buster/wiki/Inaccessible-reCAPTCHA-audio-challenge) |


---

## 🔗 Faydalı Bağlantılar

- 🌐 [Geliştirici Sitesi](https://armin.dev/)
- 💾 [GitHub Sayfası](https://github.com/dessant/buster)
- 📖 [Inaccessible reCAPTCHA Audio Challenge (Wiki)](https://github.com/dessant/buster/wiki/Inaccessible-reCAPTCHA-audio-challenge)
- 📦 [Chrome Web Store](https://chromewebstore.google.com/detail/buster-captcha-solver-for/mpbjkejclgfgadiemmefgebjfooflfhl)
- 🦊 [Firefox Add-ons](https://addons.mozilla.org/tr/firefox/addon/buster-captcha-solver/)

---

## 📝 Notlar

> Buster erişilebilirlik ve kullanıcı deneyimi için geliştirilmiştir; her CAPTCHA türünü desteklemez ve %100 başarı garantisi yoktur. Bazı sitelerin kullanım koşulları otomatik CAPTCHA çözümünü yasaklayabilir - yalnızca erişim hakkın olan ve kurallara uygun olduğunu düşündüğün durumlarda kullan. Günde birkaçtan fazla reCAPTCHA çözmek geçici engellemeye yol açabilir; eklenti kullanılsın ya da kullanılmasın bu risk geçerlidir.

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
