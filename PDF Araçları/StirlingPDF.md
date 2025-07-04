# StirlingPDF

# Stirling PDF: Açık Kaynaklı Self-Hosted PDF İşleme Platformu

## 🎯 Özet

Stirling PDF, gizlilik odaklı, açık kaynaklı ve kişisel olarak barındırılan (self-hosted) bir PDF işleme aracıdır. Adobe Acrobat’ın maliyeti ve bulut tabanlı hizmetlerin gizlilik endişelerine çözüm olarak geliştirilmiştir.

### ⭐ **Temel Özellikler**

- **60+ PDF İşlemi**: Kapsamlı araç seti
- **Self-Hosted**: Veriler sunucunuzdan çıkmaz
- **Açık Kaynak**: GNU GPLv3 lisanslı
- **Pipeline Otomasyonu**: İş akışı zincirlemesi
- **API Desteği**: Programlı entegrasyon

### ⚠️ **Önemli Not**

Stirling PDF güçlü bir işleme aracıdır ancak **gerçek içerik düzenleyicisi değildir**. Mevcut metni doğrudan düzenleme özelliği yoktur.

---

# 🏗️ **Kurulum ve Başlangıç**

## 💻 **Basit Kurulum (Başlangıç Kullanıcıları İçin)**

> ✅ Önerilen: Docker bilmiyorsanız veya basit kullanım istiyorsanız
> 

### **Windows Kurulumu**

```
1. GitHub Releases sayfasına gidin
2. "Stirling-PDF-windows.exe" dosyasını indirin
3. İndirilen dosyayı çift tıklayın
4. Kurulum tamamlandıktan sonra masaüstünden başlatın
5. Tarayıcıda otomatik açılacak: http://localhost:8080
```

### **macOS Kurulumu**

```
1. GitHub Releases sayfasına gidin
2. "Stirling-PDF-macos.dmg" dosyasını indirin
3. DMG dosyasını açın ve uygulamayı Applications klasörüne sürükleyin
4. Uygulamayı başlatın
5. Tarayıcıda otomatik açılacak: http://localhost:8080
```

### **Manuel Java Kurulumu (Tüm Platformlar)**

```bash
# Önkoşul: Java 17+ yüklü olmalı
java -version
# JAR dosyasını indirin ve çalıştırın
java -jar Stirling-PDF-X.X.X.jar
# Tarayıcıda açın: 
http://localhost:8080
```

## 🐳 **Docker Kurulumu (Profesyonel/Sunucu Kullanımı)**

> 🎯 Kimler İçin Uygun:
- Geliştiriciler ve sistem yöneticileri
- Sunucu ortamında çalıştırmak isteyenler
- Mikroservis mimarisine entegre etmek isteyenler
- Reverse proxy (Nginx/Traefik) kullanacaklar
- Otomatik backup ve güncelleme isteyenler
> 

> 💡 Docker Avantajları:
- Sistem bağımlılıklarından bağımsızlık
- Kolay güncelleme ve yönetim
- Üretim ortamı için ideal
- Reverse proxy entegrasyonu
- Otomatik restart ve healthcheck
> 

> ⚠️ Gereksinimler: Docker Desktop veya Docker Engine yüklü olmalı
> 

### **Temel Kurulum**

```bash
# En basit kurulum
docker run -d \
--name stirling-pdf \
-p 8080:8080 \
stirlingtools/stirling-pdf:latest

# Tarayıcıda açın:
 [http://localhost:8080](http://localhost:8080/)
```

### **Gelişmiş Docker Kurulumu (Volume ile)**

```bash
# Veri kalıcılığı ile kurulum
docker run -d \
  --name stirling-pdf \
  -p 8080:8080 \
  -v ./stirling-data/tessdata:/usr/share/tessdata \
  -v ./stirling-data/configs:/configs \
  -v ./stirling-data/logs:/logs \
  -v ./stirling-data/customFiles:/customFiles \
  --restart unless-stopped \
  stirlingtools/stirling-pdf:latest
```

### **Docker Compose (Önerilen Üretim Kurulumu)**

```yaml
# docker-compose.yml
version: '3.8'
services:
  stirling-pdf:
    image: stirlingtools/stirling-pdf:latest
    container_name: stirling-pdf
    ports:
      - "8080:8080"
    volumes:
      - ./stirling-data/tessdata:/usr/share/tessdata
      - ./stirling-data/configs:/configs  
      - ./stirling-data/logs:/logs
      - ./stirling-data/customFiles:/customFiles
    environment:
      - DOCKER_ENABLE_SECURITY=false
      - INSTALL_BOOK_AND_ADVANCED_HTML_OPS=false
      - LANGS=en_US
    restart: unless-stopped
    healthcheck:
      test: ["CMD-SHELL", "curl -f http://localhost:8080/ || exit 1"]
      interval: 30s
      timeout: 10s
      retries: 5

# Çalıştırma komutu
# docker-compose up -d
```

### **Farklı Sürümler**

```bash
# Standart sürüm
docker run -d --name stirling-pdf -p 8080:8080 stirlingtools/stirling-pdf:latest

# Fat sürüm (ek fontlar ve özellikler)
docker run -d --name stirling-pdf -p 8080:8080 stirlingtools/stirling-pdf:latest-fat

# Ultra-lite sürüm (minimal)
docker run -d --name stirling-pdf -p 8080:8080 stirlingtools/stirling-pdf:latest-ultra-lite
```

### **Güvenlik Ayarları ile Kurulum**

```bash
# Güvenlik aktif kurulum
docker run -d \
  --name stirling-pdf \
  -p 8080:8080 \
  -e DOCKER_ENABLE_SECURITY=true \
  -e SECURITY_ENABLELOGIN=true \
  -e SECURITY_CSRFDISABLED=false \
  -v ./stirling-data:/usr/share/tessdata \
  stirlingtools/stirling-pdf:latest
```

### 🔧 **Docker Yönetim Komutları**

### **Konteyner Yönetimi**

```bash
# Durumu kontrol et
docker ps -a | grep stirling-pdf

# Logları görüntüle
docker logs stirling-pdf

# Logları canlı takip et
docker logs -f stirling-pdf

# Konteyner içine bağlan
docker exec -it stirling-pdf /bin/bash

# Konteyneri durdur
docker stop stirling-pdf

# Konteyneri başlat
docker start stirling-pdf

# Konteyneri yeniden başlat
docker restart stirling-pdf

# Konteyneri sil
docker rm stirling-pdf

# Image'ı sil
docker rmi stirlingtools/stirling-pdf:latest
```

### **Güncelleme İşlemleri**

```bash
# 1. Mevcut konteyneri durdur
docker stop stirling-pdf

# 2. Konteyneri sil
docker rm stirling-pdf

# 3. Yeni image'ı indir
docker pull stirlingtools/stirling-pdf:latest

# 4. Yeni konteyner başlat
docker run -d \
  --name stirling-pdf \
  -p 8080:8080 \
  -v ./stirling-data:/usr/share/tessdata \
  stirlingtools/stirling-pdf:latest
```

### **Volume Yönetimi**

```bash
# Volume'ları listele
docker volume ls

# Stirling PDF volume'ı oluştur
docker volume create stirling-tessdata
docker volume create stirling-configs

# Volume ile çalıştır
docker run -d \
  --name stirling-pdf \
  -p 8080:8080 \
  -v stirling-tessdata:/usr/share/tessdata \
  -v stirling-configs:/configs \
  stirlingtools/stirling-pdf:latest
```

### 🌐 **Ağ ve Port Yapılandırması**

### **Farklı Port Kullanımı**

```bash
# 8081 portunda çalıştır
docker run -d --name stirling-pdf -p 8081:8080 stirlingtools/stirling-pdf:latest

# Sadece localhost'ta erişim
docker run -d --name stirling-pdf -p 127.0.0.1:8080:8080 stirlingtools/stirling-pdf:latest

# Tüm network interface'lerde erişim
docker run -d --name stirling-pdf -p 0.0.0.0:8080:8080 stirlingtools/stirling-pdf:latest
```

### **Reverse Proxy ile Kullanım (Nginx)**

```
# nginx.conf
server {
    listen 80;
    server_name pdf.example.com;
    
    location / {
        proxy_pass http://127.0.0.1:8080;
        proxy_set_header Host $host;
        proxy_set_header X-Real-IP $remote_addr;
        proxy_set_header X-Forwarded-For $proxy_add_x_forwarded_for;
        proxy_set_header X-Forwarded-Proto $scheme;
    }
}
```

## ⚙️ **Gelişmiş Kurulum Seçenekleri**

### **Kubernetes Deployment (Kurumsal)**

```bash
# Helm ile kurulum
helm repo add stirling-pdf https://stirling-tools.github.io/Stirling-PDF-Charts
helm install stirling-pdf stirling-pdf/stirling-pdf
```

### **Podman (Docker Alternatifi)**

```bash
# Docker yerine Podman kullanımı
podman run -d \
  --name stirling-pdf \
  -p 8080:8080 \
  docker.io/stirlingtools/stirling-pdf:latest
```

### **Systemd Service (Linux)**

```bash
# JAR dosyasını sistemd servisi olarak çalıştırma
sudo nano /etc/systemd/system/stirling-pdf.service

[Unit]
Description=Stirling PDF
After=network.target

[Service]
Type=simple
User=stirling
ExecStart=/usr/bin/java -jar /opt/stirling-pdf/Stirling-PDF.jar
Restart=always

[Install]
WantedBy=multi-user.target

# Servisi aktifleştir
sudo systemctl enable stirling-pdf
sudo systemctl start stirling-pdf
```

## 🛠️ **Ana Özellik Kategorileri**

### 🗂️ **Organize (Belge Düzenleme)**

| Araç | Açıklama |
| --- | --- |
| **PDF Multi Tool** | Birden fazla işlemi tek seferde |
| **Merge** | Çoklu PDF birleştirme |
| **Split** | Sayfa/boyut/kriterle bölme |
| **Extract Pages** | Belirli sayfaları çıkarma |
| **Rotate/Crop** | Sayfa döndürme ve kırpma |

### 📄 **Convert (Dönüştürme)**

| Kategori | Desteklenen Formatlar |
| --- | --- |
| **PDF’ye** | Office, Image, HTML, URL, Markdown |
| **PDF’den** | Word, Excel, PowerPoint, Image, RTF, CSV |
| **Özel** | PDF/A (arşiv), HTML, XML |

### 🔐 **Security (Güvenlik)**

| Araç | Açıklama |
| --- | --- |
| **Digital Signature** | Sertifika ile imzalama |
| **Password Protection** | Şifreleme/şifre kaldırma |
| **Redaction** | Manuel/otomatik karartma |
| **Watermark** | Filigran ekleme |
| **Sanitize** | Metadata temizleme |

### 👁️ **View & Edit (Görüntüleme ve Düzenleme)**

| Araç | Açıklama |
| --- | --- |
| **OCR** | Taranmış belgeleri metne çevirme |
| **Image Operations** | Resim ekleme/çıkarma |
| **Metadata** | Belge bilgilerini düzenleme |
| **Compare** | İki PDF’yi karşılaştırma |
| **Page Numbers** | Sayfa numarası ekleme |

### ⚙️ **Advanced (Gelişmiş)**

| Araç | Açıklama |
| --- | --- |
| **Pipeline** | Otomatik iş akışı zinciri |
| **Compress** | Dosya boyutu küçültme |
| **Auto Rename** | İçeriğe göre yeniden adlandırma |
| **Repair** | Bozuk PDF onarımı |
| **Split by Chapters** | Bölüm işaretlerine göre bölme |

## 🔧 **Pipeline: Güçlü Otomasyon Özelliği**

### 📋 **Pipeline Nedir?**

Birden çok PDF işlemini otomatik olarak zincirleme sistemi. Tek tıkla karmaşık iş akışları gerçekleştirme.

### 🎯 **Örnek Pipeline Senaryoları**

### **Belge Güvenlik Pipeline**

```yaml
1. OCR (metin tanıma)
2. Redact (hassas bilgileri karartma)
3. Watermark (filigran ekleme)
4. Password (şifreleme)
5. Compress (sıkıştırma)
```

### **Arşiv Hazırlama Pipeline**

```yaml
1. Merge (birleştirme)
2. PDF/A Convert (arşiv formatı)
3. Metadata Cleanup (veri temizleme)
4. Compress (boyut küçültme)
```

## 🔒 **Gizlilik ve Güvenlik**

### 🛡️ **Veri Gizliliği**

- **Yerel İşleme**: Dosyalar sunucunuzdan çıkmaz
- **Geçici Depolama**: İşlem sonrası otomatik silme
- **Self-Hosted**: Tam kontrol sizde
- **Açık Kaynak**: Kod şeffaflığı

### 🔐 **Güvenlik Özellikleri**

- Docker izolasyonu
- HTTPS desteği
- Kullanıcı kimlik doğrulama (gelişmiş sürümlerde)
- Audit log kayıtları

## 🆚 **Rekabet Karşılaştırması**

| Özellik | Stirling PDF | Adobe Acrobat | iLovePDF |
| --- | --- | --- | --- |
| **Barındırma** | Self-hosted | Masaüstü/Bulut | Bulut |
| **Gizlilik** | ✅ Maksimum | ⚠️ Orta | ❌ Düşük |
| **Fiyat** | Ücretsiz | Freemium | Freemium |
| **Otomasyon** | ✅ Pipeline/API | ❌ Sınırlı | ❌ Yok |
| **Toplu İşlem** | ✅ Sınırsız | ✅ Var | ⚠️ Sınırlı |
| **İçerik Düzenleme** | ❌ Yok | ✅ Tam | ❌ Yok |

## 📈 **Performans ve Sınırlamalar**

### ✅ **Güçlü Yönler**

- Sınırsız dosya boyutu/sayısı
- Yüksek performanslı toplu işlem
- Zengin özellik seti (60+ araç)
- Güçlü otomasyon yetenekleri

### ⚠️ **Bilinen Sınırlamalar**

- **İçerik Düzenleme Yok**: Mevcut metni değiştirme yok
- **Teknik Kurulum**: Docker/sistem yönetimi bilgisi gerekli
- **Öğrenme Eğrisi**: Gelişmiş özellikler için zaman gerekli
- **Mobil Deneyim**: Web arayüzü mobilde optimal değil

## 📚 **Kaynak ve Destek**

### 🔗 **Resmi Bağlantılar**

- **GitHub**: [github.com/Stirling-Tools/Stirling-PDF](https://github.com/Stirling-Tools/Stirling-PDF)
- **Docker Hub**: `stirlingtools/stirling-pdf`