# Karakter Tabanlı Hayatta Kalma Simülatörü

Bu proje, C programlama dili ile geliştirilmiş metin tabanlı bir hayatta kalma simülasyonudur. Oyuncu komutlar aracılığıyla karakteri yönetir ve çeşitli senaryolarla etkileşime girer. Uygulama, C dilinin temel yapılarını (koşullar, döngüler, fonksiyonlar, aritmetik işlemler, mantıksal operatörler ve switch-case) uygulamalı olarak göstermek amacıyla hazırlanmıştır.

---

## Projenin Amacı

Bu projenin temel amacı, C dilindeki temel kontrol yapılarını gerçekçi bir senaryo üzerinden uygulamak ve kullanıcı etkileşimiyle çalışan bir simülasyon geliştirmektir. Oyuncu;

- Avlanma  
- Sığınak arama  
- Dinlenme  
- Tehlike dalgası simülasyonu  
- Şifreli kapıdan geçme  
- Envanteri görüntüleme  

gibi işlemleri tek karakterlik komutlar ile gerçekleştirir.

---

## Kullanılan Temel C Yapıları

Bu proje aşağıdaki programlama yapılarını içerir:

- Switch–case yapısı  
- If–else karar mekanizmaları  
- Mantıksal operatörler (&&, ||)  
- Aritmetik işlemler  
- For döngüsü (tehlike dalgası)  
- Do–while döngüsü (şifre doğrulama sistemi)  
- Fonksiyonlar  
- Rastgele sayı üretimi (rand, srand)

---

## Komut Listesi

| Komut | Açıklama |
|-------|----------|
| A | Avlan |
| S | Sığınak ara |
| R | Envanter ve durum göster |
| E | Dinlen |
| F | Tehlike dalgasını simüle et |
| P | Şifreli engeli geç |
| X | Çıkış |

---

## Oyun Mekanikleri

### Avlan (A)
Enerji azalır, hava ve dikkat durumuna göre yemek bulunabilir veya yaralanma gerçekleşebilir.

### Sığınak Arama (S)
Orman veya mağara durumuna göre sığınak güvenliği artabilir veya düşebilir.

### Durum Gösterme (R)
Sağlık, enerji, yemek miktarı ve sığınak seviyesi ekrana yazdırılır.

### Dinlenme (E)
Sağlık ve enerji belirli miktarlarda artar.

### Tehlike Dalgası (F)
Beş adımlık bir tehlike seviyesi artışı simüle edilir. Belirli eşiklerde hasar verilir.

### Şifreli Kapı (P)
Doğru şifre olan 1234 girilene kadar döngü devam eder. Yanlış girişlerde ipucu verilir:  
"Sifre ardışık sayilardan oluşuyor."

### Çıkış (X)
Oyun sonlanır ve son durum gösterilir.

---

## Ekran Çıktısı Örnekleri

### Başlangıç:
Karakter Tabanli Hayatta Kalma Simulasyonuna Hos Geldiniz!
Baslangic Durumu -> Saglik: 100 Enerji: 80 Yemek: 2 Siginak: 0

shell
Kodu kopyala

### Avlanma:
Avlanmaya ciktin... Enerjin 10 azaldi. (Yeni enerji: 70)
Hava guzel ve dikkatlisin. Av sansin yuksek!
Bir av yakaladin! Yemek +1 (Toplam yemek: 3)

shell
Kodu kopyala

### Tehlike Dalga Simülasyonu:
Adim 3 -> Tehlike seviyesi: 6
Yuksek tehlike! Bir miktar hasar aldın.

shell
Kodu kopyala

### Şifreli Kapı:
Sifreyi gir (4 haneli): 0000
Yanlis sifre! Kapı acilmadi.
Ipucu: Sifre ardışık sayilardan olusuyor.

yaml
Kodu kopyala

---

## Derleme ve Çalıştırma

Linux / macOS:
gcc main.c -o simulasyon
./simulasyon

scss
Kodu kopyala

Windows (MinGW):
gcc main.c -o simulasyon
simulasyon.exe

yaml
Kodu kopyala

---

## Dosya Yapısı

main.c → Programın ana kaynak kodu
README.md → Proje açıklama dosyası

yaml
Kodu kopyala

---

## Geliştirici Notu

Program, eğitim amaçlı geliştirilmiştir. Kod yapısı fonksiyonel temellere dayanır, okunabilirlik ve bölümlere ayrılabilirlik gözetilmiştir.

---

## Lisans

Bu proje eğitim amaçlı hazırlanmıştır ve özgürce kullanılabilir.
