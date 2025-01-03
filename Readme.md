# Tombala Oyunu Dokümantasyonu

## Proje Hedefi

Bu proje, tarayıcıda çalışan ve birden fazla kullanıcının bir araya gelerek tombala oynayabileceği bir web uygulaması oluşturmayı amaçlamaktadır. Uygulama HTML, CSS ve JavaScript kullanılarak geliştirilecektir.

---

### Gereksinimler

**1. Teknik Gereksinimler**

HTML: Uygulama yapısını oluşturmak için kullanılacak.

CSS: Görsel tasarım ve stil düzenlemeleri için kullanılacak.

JavaScript: Oyunun mantığını ve dinamik etkileşimlerini sağlamak için kullanılacak.

**2. Temel Fonksiyonellik**

Kullanıcıların bir odaya katılması veya yeni oda oluşturması.

Her oyuncuya rastgele bir tombala kartı dağıtılması.

Sistemin rastgele sayılar çekmesi.

Oyuncuların sayıları işaretleyebilmesi ve "Tombala!" diyebilmesi.

Kazananı belirlemek ve oyunu sonlandırmak.

**3. Ekstra Gereksinimler**

Gerçek zamanlı iletişim (WebSocket ya da benzeri bir çözüm).

Kullanıcı adıyla giriş.

Mobil uyumluluk.

---

### Yapı Planı

1. HTML

Ana Sayfa: Oyun odalarını listeleyen ve yeni oda oluşturma seçeneği sunan bir sayfa.

Oyun Alanı: Tombala oyununu oynayabilmek için gerekli arayüz.

2. CSS

Modern ve minimalist bir tasarım.

Mobil cihazlar için responsive yapı.

3. JavaScript

Oda oluşturma ve katılma işlemleri.

Tombala kartını oluşturma ve doldurma algoritması.

Rastgele sayı çekme sistemi.

Kazanan kontrol mekanizması.

---

### Dosya Yapısı

`project-root/

     |-- index.html

     |-- game.html

     |-- styles/
       |-- main.css
     |-- scripts/
       |-- app.js
       |-- game.js
     |-- assets/
     |-- images/
     |-- sounds/`

---

### Özellikler ve Detaylar

**Ana Sayfa**

- Kullanıcıların mevcut oyun odalarını görebileceği bir liste.

- Yeni oda oluşturma butonu.

- Her oda için şu bilgiler gösterilir:

  - Oda adı

  - Katılımcı sayısı

**Tombala Kartı**

- 5x5 matris yapısı.

- Her oyuncuya rastgele sayılarla doldurulmuş bir kart atanır.

**Oyun Mekaniği**

- Sayılar, bir dizi (1-90) içinden rastgele çekilir.

- Sistemin çektiği sayı herkesin ekranında görünür.

- Oyuncular kartlarındaki sayıları tıklayarak işaretler.

- "Tombala!" butonuna basıldığında, sistem kazananı kontrol eder.

**Gerçek Zamanlı Bağlantı**

- Kullanılacak Teknoloji: WebSocket ya da Firebase Real-Time Database.

- Güncellemelerin anında herkese ulaşması.

---

### Geliştirme Planı

**1. HTML ve CSS Tasarımı:**

- Ana sayfa ve oyun alanını tasarla.

- Kart ve Sayı Çekme Mantığı:

**2. Tombala kartı oluşturma algoritması.**

- Rastgele sayı çekme fonksiyonu.

**3. Gerçek Zamanlı Bağlantı:**

- WebSocket ya da Firebase entegrasyonu.

**4. Test ve Debug:**

- Farklı cihazlarda ve tarayıcılarda test yapılması.

---

#### Notlar

- Projeye başlamadan önce WebSocket kullanımı ve gerçek zamanlı veri işlemleriyle ilgili temel bilgiler edinilmelidir.

- Kullanıcı deneyimini artırmak için ses efektleri ve animasyonlar eklenebilir.

# TASARIM

1. Play buttonu kodlanmayacak sadece oda açılabilecek:

   ![alt text](image.png)
   Navbar'da anasayfa, yeni oyun sekmeleri olacak.

2. Oda açıldıktan sonra görüntüler:
   ![alt text](image-1.png)

3. Kart görünümü:
   ![alt text](image-3.png)

# ÖZELLİKLER:

1. Sesli iletişim kurulabilecek.
2. Yazılı iletişim kurulabilecek.
3. Kart adedi sonradan arttırılacak.
4. Odayı kuran kişinin ekranında sayı belirlemek için çekiliş butonu olacak.
5. Çekilen sayı dönen sayılar içinde sabitlenerek gösterilecek.
6. Kartında sayı olan kişinin ekranında BENDE VAR butonu olacak.
7. 1. çinko, 2. Çinko ve Tombala butonları her kullanıcının ekranında olacak.
8. Oyun bittiğinde listelerin açıklandığı sayfa:
   ![alt text](image-4.png)

9. Kazanan listesi oluşturulması(2. kart eklenirken yapılacak)

10. Tasarımların yapılması
11. proje bittikten sonra React Native ile kodlanması
