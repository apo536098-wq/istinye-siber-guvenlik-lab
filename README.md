# 🛡️ İstinye Üniversitesi - Bilişim Güvenliği İnteraktif Öğrenme & Simülasyon Platformu

İstinye Üniversitesi Bilişim Güvenliği Teknolojisi ve ilgili mühendislik bölümlerinin müfredatındaki teknik ve teorik dersleri tek bir görsel, interaktif ve pratik simülasyon platformunda birleştiren web tabanlı bir siber güvenlik laboratuvarıdır.

---

## 📌 İçindekiler ve Modül Açıklamaları

Proje bünyesinde müfredatta yer alan 8 temel ders alanı ve 1 değerlendirme quizi bulunmaktadır:

### 1. 🧱 Güvenlik Duvarı (Firewall) Çözümleri

**Açıklama:** Ağ topolojisi üzerinde dinamik paket akışı simülasyonu.

**Özellikler:**
- Port bazlı (HTTP, HTTPS, SSH, RDP, FTP) ACL (Access Control List) kural yönetimi (ALLOW / DENY).
- Normal ağ trafiği ve SYN Flood (DDoS) saldırı simülasyonu.
- Anlık engellenen (dropped) ve geçen (passed) paket istatistikleri.

### 2. 💻 Güvenlik Web Geliştirme (Secure Web Development)

**Açıklama:** OWASP Top 10 zafiyetlerinin canlı kod ve girdi düzeyinde analizi.

**Özellikler:**
- **SQL Injection (SQLi) Lab:** Savunmasız SQL sorgusu ile Prepared Statement (parametrik sorgu) güvenlik farklarının gösterimi.
- **XSS (Cross-Site Scripting) Lab:** Stored/Reflected XSS payload çalıştırma ve HTML Sanitization / `htmlspecialchars` filtreleme testi.

### 3. 🎯 İleri Sızma Testleri (Penetration Testing)

**Açıklama:** Web tabanlı simüle edilmiş Kali Linux terminal ortamı.

**Özellikler:**
- Keşif ve tarama komutları (`nmap`, `nikto`).
- İstismar araçları (`msfconsole` - Metasploit Framework).
- İnteraktif terminal komut satırı deneyimi.

### 4. ☁️ Bulut Bilişim Sistemleri (Cloud Computing & Containers)

**Açıklama:** AWS/Azure mimarileri ve Docker konteyner yönetimi.

**Özellikler:**
- Dinamik Nginx ve Postgres Docker container deployment simülasyonu.
- AWS EC2 Auto-scaling ve ALB (Application Load Balancer) yük testi görselleştirmesi.

### 5. 🌐 Bilgisayar Ağları & Subnetting

**Açıklama:** Ağ katmanları ve IP adresi hesaplama araçları.

**Özellikler:**
- **Canlı IPv4 Subnet Calculator:** CIDR (/24, /25, /26, vb.) girişleri için Network IP, Broadcast IP ve kullanılabilir Host aralığı hesaplama.
- OSI 7 Katmanı ve protokol haritalama kılavuzu.

### 6. 🔑 Matematik & Kriptoloji (Cryptography)

**Açıklama:** Şifreleme algoritmaları ve ayrık matematiksel altyapı.

**Özellikler:**
- İnteraktif Sezar Şifrelemesi (Shift Key kaydırmalı canlı şifreleme/çözme).
- RSA Asimetrik Şifreleme asal sayı ve modüler aritmetik ($C = M^e \pmod n$) açıklama paneli.

### 7. 🐍 Temel Programlama & Algoritmalar

**Açıklama:** Siber güvenlik betikleri ve kod yürütme görselleştiricisi.

**Özellikler:**
- Python `socket` kütüphanesi ile yazılmış Port Tarayıcı (Port Scanner) kodu.
- Canlı "Run Script" butonu ile konsol çıktısı (Execution Log) simülasyonu.

### 8. 🌍 Şehir, Medeniyet & Uluslararası Örgütler

**Açıklama:** Siber hukuk ve küresel güvenlik kuruluşları.

**Özellikler:**
- NATO CCDCOE ve Tallinn Kılavuzu (Tallinn Manual) siber savaş hukuku detayları.
- INTERPOL Cybercrime küresel operasyon tanımları.

### 9. 🎓 Ders Değerlendirme & Sınav Quizi

**Açıklama:** Üniversite vize/final sınav formatına uygun çoktan seçmeli test modülü. Anlık puanlama ve cevap geri bildirimi sunar.

---

## 🚀 Projeyi Yerelde Çalıştırma (Local Setup)

Bu proje Single-File (tek dosya) mimarisiyle geliştirildiği için herhangi bir `node_modules` veya backend sunucusu kurulumu gerektirmez.

1. Depoyu klonlayın:

   ```bash
   git clone https://github.com/KULLANICI_ADI/istinye-siber-guvenlik-lab.git
   ```

2. Proje klasörüne girin:

   ```bash
   cd istinye-siber-guvenlik-lab
   ```

3. `index.html` dosyasını çift tıklayarak herhangi bir modern web tarayıcısında (Chrome, Firefox, Edge, Safari) açın.

---

## 📤 GitHub'a Yükleme ve Yayınlama (Step-by-Step Guide)

### 1. Adım: GitHub Deposu Oluşturma

1. GitHub'a giriş yapın.
2. Sağ üstteki **+** simgesine tıklayıp **New repository** seçeneğini seçin.
3. **Repository name:** `istinye-siber-guvenlik-lab` yazın.
4. Gizliliği **Public** seçin ve **Create repository** butonuna basın.

### 2. Adım: Kodları Bilgisayarınızdan Yükleme

Terminal veya Komut Satırını (CMD/Git Bash) açıp dosyanızın bulunduğu klasörde şu komutları sırasıyla çalıştırın:

```bash
# 1. Git deposunu başlatın
git init

# 2. Tüm dosyaları ekleyin
git add .

# 3. İlk commit'i oluşturun
git commit -m "feat: Istinye Siber Guvenlik Lab platformu ilk sürüm"

# 4. Ana dalı 'main' olarak ayarlayın
git branch -M main

# 5. Kendi GitHub depo bağlantınızı ekleyin (KULLANICI_ADI yerine kendi adınızı yazın)
git remote add origin https://github.com/KULLANICI_ADI/istinye-siber-guvenlik-lab.git

# 6. Kodları GitHub'a yükleyin
git push -u origin main
```

### 3. Adım: GitHub Pages ile Ücretsiz Yayınlama (Live Link)

1. GitHub'da oluşturduğunuz deponun **Settings** (Ayarlar) sekmesine gidin.
2. Sol menüden **Pages** seçeneğine tıklayın.
3. **Branch** kısmından `main` dalını seçin ve **Save** (Kaydet) butonuna tıklayın.
4. 1-2 dakika içinde siteniz `https://KULLANICI_ADI.github.io/istinye-siber-guvenlik-lab/` adresinde ücretsiz ve canlı olarak yayınlanacaktır!

---

## 🛠️ Kullanılan Teknolojiler

- **HTML5 / ES6+ JavaScript:** Modüler fonksiyonel mimari ve DOM manipülasyonu.
- **Tailwind CSS (CDN):** Modern, responsive ve dark-mode uyumlu siber temalı tasarım.
- **Font Awesome & Lucide Icons:** Vektörel güvenlik ikonu seti.

---

## 📝 Lisans

Bu proje MIT Lisansı altında korunmaktadır. Eğitim amaçlı serbestçe kullanılabilir.
