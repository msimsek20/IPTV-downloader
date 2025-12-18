# Xstream Web Downloader (GitHub Pages)

Basit, tarayıcı tabanlı, sunucusuz IPTV (Xstream Codes API) VOD ve Dizi indirme yöneticisi.

Bu araç tamamen tarayıcı üzerinde çalışır (Client-Side). Kullanıcı adı, şifre veya izleme geçmişiniz hiçbir sunucuya gönderilmez, sadece tarayıcınızın yerel hafızasında (LocalStorage) tutulur.

## 🚀 Özellikler

- **Tek HTML Dosyası:** Kurulum gerektirmez.
- **VOD & Dizi Tarayıcı:** Kategorilere göre filtreleme ve arama.
- **İndirme Kuyruğu:** İstediğiniz içerikleri listeye ekleyin, topluca indirin.
- **Zamanlayıcı:** Belirlenen saatte indirmeyi otomatik başlatma (Sayfa açık kalmalı).

## ⚠️ Önemli Uyarılar (Çalıştırmak İçin Okuyun)

Bu proje GitHub Pages üzerinde çalıştığı için tarayıcı güvenlik önlemlerine (CORS ve Mixed Content) takılır. Çalışması için aşağıdakileri yapmalısınız:

### 1. CORS Hatası Çözümü
Tarayıcılar, bir web sitesinden başka bir adrese (IPTV sunucunuza) istek atılmasını güvenlik nedeniyle engeller. Bunu aşmak için tarayıcınıza bir eklenti kurmalısınız:
- **Chrome/Edge/Brave:** "Allow CORS: Access-Control-Allow-Origin" eklentisini mağazadan indirin.
- Kullanmadan önce eklentiyi **Aktif (ON)** duruma getirin.

### 2. HTTPS vs HTTP Sorunu
GitHub Pages **HTTPS** (Güvenli) protokolü kullanır. Eğer IPTV sağlayıcınızın linki **HTTP** ile başlıyorsa (çoğu öyledir), tarayıcı "Güvenli sayfada güvensiz içerik" uyarısı verir ve bağlantıyı reddeder.
- **Çözüm:** Tarayıcınızın adres çubuğundaki kilit simgesine tıklayıp "Site Ayarları"ndan "Güvenli olmayan içeriğe izin ver" (Insecure Content: Allow) seçeneğini işaretleyin.

## 🔧 Kurulum

1. Bu projeyi Fork'layın veya indirin.
2. Kodda herhangi bir değişiklik yapmanıza gerek yoktur.
3. GitHub Repository ayarlarından **Pages** sekmesine gidin.
4. `Branch: main` seçip kaydedin.
5. Size verilen linke (ör: `[https://msimsek20.github.io/IPTV-downloader/]`) gidin.

## 📝 Kullanım

1. Sayfayı açın ve CORS eklentisini açtığınızdan emin olun.
2. Sol panelden Host (`http://domain:port`), Kullanıcı Adı ve Şifrenizi girin.
3. **Bağlan** butonuna basın.
4. Sağ panelden kategori seçip listeyi yükleyin.
5. **"+"** butonuna basarak kuyruğa ekleyin.
6. Kuyruk hazır olduğunda **"Şimdi Başlat"** diyerek indirmeleri tetikleyin (Tarayıcı çoklu dosya indirme izni isteyebilir, izin verin).
