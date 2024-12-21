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

> project-root/
> |-- index.html
> |-- game.html
> |-- styles/
> | |-- main.css
> |-- scripts/
> | |-- app.js
> | |-- game.js
> |-- assets/

    |-- images/
    |-- sounds/

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
