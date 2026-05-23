# 🛠️ uBlock Origin

> **Kısa Açıklama:** Açık kaynak, geniş spektrumlu içerik engelleyici; reklam, izleyici ve zararlı domain filtreleme - düşük CPU ve bellek kullanımıyla.

Güncel · Chrome, Edge, Brave, Firefox, Opera · Açık kaynak (GPL-3.0) · Güvenlik ve Gizlilik

---

## 📌 Genel Bakış

uBlock Origin, reklam ve izleyicilerin ötesinde geniş spektrumlu bir içerik engelleyicidir. Filter list tabanlı çalışır; varsayılan listelerle çoğu site için ek ayar gerektirmez. AdBlock gibi "Kabul Edilebilir Reklamlar" programına katılmaz. Brave kullanıcıları için tam sürüm, Manifest V2 desteği sayesinde ek avantaj sunar.

---

## ✨ Öne Çıkan Özellikler

- **Varsayılan filter listeleri** - EasyList, EasyPrivacy, Peter Lowe ve zararlı URL listesi hazır gelir
- **Düşük kaynak kullanımı** - CPU ve bellek açısından verimli çalışır
- **Site bazlı kontrol** - Büyük mavi güç düğmesi ile tek site için aç/kapa
- **Gelişmiş kurallar** - Element engelleme ve özel filter desteği
- **Veri toplamaz** - Geliştirici, kullanıcı verisi toplamadığını belirtir
- **Açık kaynak** - GPL-3.0 lisanslı; kod GitHub'da incelenebilir

---

## 📥 İndirme ve Kurulum

Tarayıcına göre doğru sürümü seç. Chromium tabanlı tarayıcılarda (Chrome vb.) tam sürüm yerine **uBlock Origin Lite** kullanılır.

### Brave - Manifest V2 desteği (tam sürüm, önerilen)

Brave, Google'ın Manifest V3 geçişine karşı seçili Manifest V2 uzantılarını **kendi sunucularında barındırır** ve destekler:

1. Brave'de adres çubuğuna `brave://settings/extensions/v2` yaz
2. **uBlock Origin'i etkinleştir** anahtarını aç
3. Gerekirse [Chrome Web Store - uBlock Origin](https://chromewebstore.google.com/detail/ublock-origin/cjpalhdlnbpafiamejdnhcphjbkeiagm) üzerinden kurulumu tamamla

> Brave, bu MV2 uzantılarını barındırır ancak içerik, güvenlik veya davranışlarını incelemez veya doğrulamaz. Detay için [resmi uBlock Origin sayfasına](https://ublockorigin.com/) bak.

### Chromium tabanlı tarayıcılar - uBlock Origin Lite

Chrome ve diğer Chromium tabanlı tarayıcılarda MV3 nedeniyle **uBlock Origin Lite** (uBOL) kullanılır:

1. [uBlock Origin Lite - Chrome Web Store](https://chromewebstore.google.com/detail/ublock-origin-lite/ddkjiahejlhfcafbddmgiahcphecmpfh) sayfasına git
2. **Chrome'a ekle** butonuna tıkla
3. İzinleri onayla ve kurulumu tamamla

> Lite sürümü MV3 uyumludur; tam sürüme kıyasla bazı gelişmiş özellikler sınırlı olabilir. Daha fazla filter listesi için eklenti ayarlarından (dişli simgesi) ek kurallar açılabilir.

### Firefox - tam sürüm

1. [uBlock Origin - Firefox Add-ons](https://addons.mozilla.org/en-US/firefox/addon/ublock-origin/) sayfasına git
2. **Add to Firefox** butonuna tıkla
3. Kurulumu onayla

### Microsoft Edge - tam sürüm

1. [uBlock Origin - Edge Add-ons](https://microsoftedge.microsoft.com/addons/detail/ublock-origin/odfafepnkmbhccpbejgmiehpchacaeak) sayfasına git
2. **Al** butonuna tıkla
3. Kurulumu onayla

### Opera - tam sürüm

1. [uBlock Origin - Opera Add-ons](https://addons.opera.com/en/extensions/details/ublock/) sayfasına git
2. **Download Opera** / eklentiyi kur adımlarını takip et
3. Opera tarayıcısında kurulumu tamamla

### Manuel kurulum (gelişmiş)

Güncel sürümler ve geliştirici build'leri için [GitHub Releases](https://github.com/gorhill/uBlock/releases) sayfasına bak.

---

## ⚙️ İlk Kurulum ve Önerilen Ayarlar

1. **Varsayılan filtreleri açık bırak:** İlk kurulumdaki listeler çoğu kullanıcı için yeterlidir.
2. **Brave kullanıcıları:** `brave://settings/extensions/v2` sayfasında uBlock Origin'in etkin olduğunu doğrula.
3. **Chrome / Chromium kullanıcıları:** [uBlock Origin Lite](https://chromewebstore.google.com/detail/ublock-origin-lite/ddkjiahejlhfcafbddmgiahcphecmpfh) kur; tam sürüm bu tarayıcılarda desteklenmez.
4. **Tek engelleyici kullan:** AdBlock gibi başka bir reklam engelleyiciyle birlikte kurma; çakışma ve site bozulmalarına yol açabilir.
5. **Bozulan siteler:** Büyük mavi güç düğmesi ile o site için geçici olarak devre dışı bırak.

> 💡 **İpucu:** `ublock.org` sitesi uBlock Origin ile **ilgisizdir**. Resmi kaynak [ublockorigin.com](https://ublockorigin.com/) ve geliştirici Raymond Hill'dir.

---

## 🚀 Temel Kullanım

### Günlük gezinme

Kurulumdan sonra çoğu sitede otomatik çalışır. Ekstra işlem gerekmez; reklamlar ve izleyiciler filter listeleriyle engellenir.

### Site bazlı izin verme

1. Sorunlu sitedeyken uBlock Origin simgesine tıkla
2. Büyük mavi **güç düğmesine** bas (site için devre dışı)
3. Sayfayı yenile

### Tarayıcı farkları

| Tarayıcı | Sürüm | Kurulum |
| -------- | ----- | ------- |
| **Brave** | Tam uBlock Origin (MV2) | `brave://settings/extensions/v2` + Chrome Web Store |
| **Chrome / Chromium** | uBlock Origin Lite (MV3) | [Chrome Web Store - Lite](https://chromewebstore.google.com/detail/ublock-origin-lite/ddkjiahejlhfcafbddmgiahcphecmpfh) |
| **Firefox** | Tam uBlock Origin | [Firefox Add-ons](https://addons.mozilla.org/en-US/firefox/addon/ublock-origin/) |
| **Edge** | Tam uBlock Origin | [Edge Add-ons](https://microsoftedge.microsoft.com/addons/detail/ublock-origin/odfafepnkmbhccpbejgmiehpchacaeak) |
| **Opera** | Tam uBlock Origin | [Opera Add-ons](https://addons.opera.com/en/extensions/details/ublock/) |


---

## ⚠️ Bilinen Sorunlar ve Çözümleri


| Sorun                            | Neden Olur                                            | Çözüm                                                     |
| -------------------------------- | ----------------------------------------------------- | --------------------------------------------------------- |
| Site düzgün açılmıyor            | Filter listesi sayfa öğelerini de engelliyor olabilir | O site için büyük güç düğmesi ile geçici kapat            |
| YouTube reklamları engellenmiyor | Filter güncellemesi gecikebilir                       | Eklentiyi güncelle; listelerin güncel olduğunu kontrol et |
| Chrome'da sınırlı özellik        | MV3 nedeniyle Lite sürümü kullanılır                  | [uBlock Origin Lite](https://chromewebstore.google.com/detail/ublock-origin-lite/ddkjiahejlhfcafbddmgiahcphecmpfh) kur; tam sürüm için Brave/Firefox dene |


---

## 🔗 Faydalı Bağlantılar

- 🌐 [Resmi Web Sitesi](https://ublockorigin.com/)
- 📦 [uBlock Origin Lite - Chrome Web Store](https://chromewebstore.google.com/detail/ublock-origin-lite/ddkjiahejlhfcafbddmgiahcphecmpfh) (Chromium tabanlı tarayıcılar)
- 📦 [uBlock Origin - Chrome Web Store](https://chromewebstore.google.com/detail/ublock-origin/cjpalhdlnbpafiamejdnhcphjbkeiagm) (Brave MV2)
- 🦊 [Firefox Add-ons](https://addons.mozilla.org/en-US/firefox/addon/ublock-origin/)
- 🔷 [Microsoft Edge Add-ons](https://microsoftedge.microsoft.com/addons/detail/ublock-origin/odfafepnkmbhccpbejgmiehpchacaeak)
- 🎭 [Opera Add-ons](https://addons.opera.com/en/extensions/details/ublock/)
- 💾 [GitHub Releases](https://github.com/gorhill/uBlock/releases)
- 🦁 Brave MV2 ayarları: `brave://settings/extensions/v2`

---

## 📝 Notlar

> uBlock Origin bir "ad blocker" değil, geniş spektrumlu içerik engelleyicidir. Chromium tabanlı tarayıcılarda (Chrome vb.) **uBlock Origin Lite** kullanılır; tam sürüm için Brave (MV2 desteği), Firefox, Edge veya Opera tercih edilebilir. Filter listesi bakımcılarına destek olmayı düşünebilirsin - proje bağış kabul etmez.

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
