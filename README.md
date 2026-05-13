# High Quack - 2D Denge ve Kule İnşa Oyunu

Bu proje, HTML5 Canvas ve saf JavaScript kullanılarak geliştirilmiş, fizik tabanlı bir 2D kule inşa etme oyunudur. Projenin amacı, herhangi bir oyun motoru  veya fizik kütüphanesi kullanmadan katı cisim dinamiğini ve çarpışma algılamasını sıfırdan implemente etmektir.

## Esinlenen Oyunlar
### Oyun Linki
- https://suumpmolk.itch.io/blueprint-bob
### Oyun Adı
- Blueprint Bob

🔗 **[OYUNU CANLI OLARAK OYNAMAK İÇİN BURAYA TIKLAYIN](https://hkepir.github.io/web-2Dgame/)**

---

## Oyunun Hedefi ve Zorluk Mekaniği 
**Hedef:** Oyuncunun temel amacı, vinç yardımıyla blokları üst üste dizerek ekranın belirli bir yüksekliğinde bulunan "Hedef Çizgisine" ulaşmak ve ardından ana karakterimizi bu kulenin en tepesine çıkartarak 3 saniye boyunca dengede kalmasını sağlamaktır.
**Zorluk (Challenge):**
* Blokların ağırlık merkezleri asimetriktir, bu yüzden yanlış hizalamalar tork yaratarak kulenin devrilmesine yol açar.
* 90 saniyelik kısıtlı bir inşa süresi vardır.
* Karakter kuleye tırmanırken ekstra bir ağırlık ve momentum yaratır; bu da önceden stabil görünen kulenin son anda yıkılmasına neden olabilir.

---

## Kontroller
Oyun bilgisayar üzerinden klavye ve mouse etkileşimi ile oynanmaktadır:
* **Sol Tık (Mouse):** İnşa (Planlama) ekranında 4 birimlik blok çizmek için kullanılır.
* **Space (Boşluk Tuşu):** Sallanan vinçteki bloğu aşağı bırakır.
* **A ve D Tuşları (veya Sol/Sağ Oklar):** Karakteri sağa ve sola yürütür.
* **W Tuşu (veya Yukarı Ok / Space):** Karakteri zıplatır.

---

##  Oyun İçi Görüntüler

### 1. Blok Tasarım ve Kule İnşa Aşaması
![Kule Insa Ekrani](./yapı_olusturma.png) 
*(Yukarıdaki parantez içine 1. görselin dosya yolunu yazmalısın. Örn: oyundan_kare1.jpg)*

### 2. Karakterin Kuleye Tırmanış Aşaması
![Karakter Denge Ekrani](./karakter_hareket.png)
*(Yukarıdaki parantez içine 2. görselin dosya yolunu yazmalısın. Örn: oyundan_kare2.jpg)*

---

##  Teknik Gereksinimler ve Altyapı
Bu proje, dersin gereksinimleri doğrultusunda aşağıdaki özellikleri barındırmaktadır:
- **Canvas Implementasyonu:** Tüm oyun döngüsü ve fiziksel çizimler HTML5 <canvas> üzerinde sorunsuz bir "Game Loop" ile çalışmaktadır.
- **Ses ve Müzik:** Oyun boyunca arka planda çalan ambiyans müziği ve aksiyona (zıplama, blok düşme çarpışmaları) bağlı ses efektleri sisteme entegre edilmiştir.
- **Kod İçi Dokümantasyon:** JavaScript dosyasının içindeki fizik hesaplamaları, çarpışma algoritmaları ve genel oyun mekanikleri Türkçe yorum satırlarıyla detaylıca açıklanmıştır.

---
# Kullanılan Kaynaklar ve Asset Credits

## Görseller

### Karakter ve Oyun İllüstrasyonları
- Kaynak Sahibi: Sümeyye Designer
- Platform: Instagram
- Profil:
  https://www.instagram.com/sumeyyedesigner?igsh=MTA3dW01dWw3Nmh1Yw==
- Kullanım Durumu:
  Görseller, içerik sahibinden izin alınarak projede kullanılmıştır.

---

## Ses Dosyaları

### Oyun Ses Efektleri
- Kaynak: Pixabay Sound Effects
- Web Sitesi:
  https://pixabay.com/sound-effects/
- Kullanım Alanı:
  Oyun içi efekt sesleri ve etkileşim sesleri.

  ---

## Faydalanılan Video Kaynakları ve Github Hesapları

### Video Kanalları
- The Nature of Code
- Code Explained - Create Tetris Game Using JavaScript and HTML5 | JavaScript Project For Beginners
- Coding Math

### Github Hesapları
- https://github.com/liabru/matter-js/blob/master/examples/mixed.js
- https://github.com/xi/trickytowers?ysclid=mp49gzpotw452697405

---

## Ek Bilgi
Bu projede kullanılan tüm görsel ve işitsel içerikler yalnızca eğitim ve akademik proje amacıyla kullanılmıştır.
