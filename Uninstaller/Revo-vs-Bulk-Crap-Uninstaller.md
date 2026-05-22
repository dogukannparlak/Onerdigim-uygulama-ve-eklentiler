# ⚖️ Revo Uninstaller vs Bulk Crap Uninstaller

> **Kısa Açıklama:** İki popüler kaldırma aracının hızlı karşılaştırması — hangisini ne zaman kullanmalısın?

---

## 📌 Genel Bakış

Windows'un yerleşik kaldırıcısı programı listeden siler; dosya ve kayıt defteri artıkları çoğu zaman kalır. **Revo Uninstaller** tek program odaklı derin temizlik ve Hunter Mode sunar. **Bulk Crap Uninstaller (BCU)** toplu kaldırma, geniş algılama ve ücretsiz açık kaynak yapısıyla öne çıkar. İkisi birbirinin yerine geçebilir; kullanım senaryona göre seçilir.

Detaylı rehberler: [Revo-Uninstaller .md](Revo-Uninstaller%20.md) · [Bulk-Crap-Uninstaller .md](Bulk-Crap-Uninstaller%20.md)

---

## 📊 Hızlı Karşılaştırma

| | Revo Uninstaller | Bulk Crap Uninstaller |
| --- | --- | --- |
| **Fiyat** | Free + Pro (ücretli) | Tamamen ücretsiz |
| **Lisans** | Freeware / ticari | Apache 2.0, açık kaynak |
| **Odak** | Tek program, derin artık tarama | Toplu kaldırma, otomasyon |
| **Arayüz** | Daha sade, yeni kullanıcı dostu | İşlevsel, güç kullanıcı odaklı |
| **Artık temizliği** | Güçlü (Güvenli/Orta/Gelişmiş) | Evet, kaldırma sonrası tarama |
| **Toplu kaldırma** | Yalnızca Pro | Free'de var |
| **Zorla kaldırma** | Pro | Free'de var |
| **Hunter Mode** | Evet | Hayır |
| **Kurulum izleme** | Pro | Hayır |
| **CLI / otomasyon** | Sınırlı | Konsol arayüzü, listeler |

---

## 🔍 Özellik Karşılaştırması

| Özellik | Revo | BCU |
| ------- | ---- | --- |
| Normal uygulamalar | ✅ | ✅ |
| Gizli / korumalı uygulamalar | ⚠️ Sınırlı | ✅ |
| Taşınabilir (portable) yazılımlar | ❌ | ✅ |
| Windows Store (UWP) | ✅ (Pro ile güçlü) | ✅ |
| Steam / Oculus oyunları | ❌ | ✅ |
| Chocolatey paketleri | ❌ | ✅ |
| Windows Özellikleri / Update | ❌ | ✅ |
| Başlangıç yöneticisi | ✅ (Free) | ✅ |
| Sertifika doğrulama | — | ✅ |
| Özel kaldırma listeleri | — | ✅ |

---

## 🎯 Hangisini Seçmeli?

### Revo Uninstaller tercih et

- Ayda birkaç program kaldırıyorsan
- **Hunter Mode** ile simge/pencereden program bulmak istiyorsan
- Daha sade arayüz ve adım adım artık onayı önemliyse
- Pro almayı düşünüyorsan: kurulum izleme, Logs Database, zorla kaldırma

### Bulk Crap Uninstaller tercih et

- Format öncesi veya bloatware temizliğinde **onlarca program** silmek istiyorsan
- **Ücretsiz** toplu kaldırma ve zorla kaldırma gerekiyorsa
- Steam, portable veya Chocolatey paketlerini de yönetmek istiyorsan
- Taşınabilir sürüm veya CLI otomasyonu kullanacaksan

### İkisini birlikte kullan

Mümkün. Revo'yu günlük tek program kaldırma için, BCU'yu nadir toplu temizlik için tutabilirsin. Aynı anda ikisini çalıştırma; kaldırma işlemini sırayla yap.

---

## ⚠️ Ortak Uyarılar

| Risk | Önlem |
| ---- | ----- |
| Kritik sistem dosyası silinmesi | Kaldırmadan önce geri yükleme noktası oluştur |
| Bilinmeyen program | Adını araştır; Windows bileşenlerine dokunma |
| Revo Gelişmiş tarama | Bilmediğin registry girdilerini silme |
| BCU toplu seçim | Seçimleri silmeden önce listeyi gözden geçir |

---

## 🔗 Faydalı Bağlantılar

- 🔴 [Revo Uninstaller](https://www.revouninstaller.com/)
- 🔵 [BCU — SourceForge](https://sourceforge.net/projects/bulk-crap-uninstaller/)
- 🔵 [BCU — Resmi Site](https://www.bcuninstaller.com/)
- 📖 [Revo rehberi](Revo-Uninstaller%20.md)
- 📖 [BCU rehberi](Bulk-Crap-Uninstaller%20.md)

---

## 📝 Notlar

> Çoğu ev kullanıcısı için **Revo Free** veya **BCU** yeterlidir; ikisine de para ödemek gerekmez. Pro özellikleri (Revo kurulum izleme, toplu kaldırma) yalnızca sık ve ileri düzey temizlik yapıyorsan değer katar. BCU için indirme tercihi: [SourceForge](https://sourceforge.net/projects/bulk-crap-uninstaller/).

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
