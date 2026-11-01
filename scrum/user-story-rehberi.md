# User Story Yazım Rehberi

## 1. Temel Format

> **Bir** [kullanıcı rolü] **olarak**, [hedef/ihtiyaç] **istiyorum**, **böylece** [fayda/değer].

Örnek: Bir **müşteri olarak**, siparişimin kargo durumunu görmek istiyorum, böylece teslimat için evde olup olmayacağımı planlayabilirim.

Üç bileşen (3C): **Card** (kısa tanım), **Conversation** (konuşma ve netleştirme), **Confirmation** (kabul ölçütleri).

## 2. İyi Hikaye: INVEST

| Harf | İlke | Soru |
|------|------|------|
| I | Independent (Bağımsız) | Diğerlerinden bağımsız sıralanıp yapılabilir mi? |
| N | Negotiable (Pazarlığa açık) | Ayrıntılar konuşularak netleşiyor mu? |
| V | Valuable (Değerli) | Kullanıcıya/işe değer katıyor mu? |
| E | Estimable (Tahmin edilebilir) | Takım büyüklüğünü tahmin edebiliyor mu? |
| S | Small (Küçük) | Tek sprint içinde bitebilir mi? |
| T | Testable (Test edilebilir) | Kabul ölçütleri net mi? |

## 3. Kabul Ölçütleri

Hikayenin "bitti" sayılması için karşılanması gereken, test edilebilir koşullardır. İki yaygın format:

**Kontrol listesi**
- Kullanıcı sipariş numarasıyla sorgulama yapabilir.
- Durum: Hazırlanıyor, Kargoda, Teslim edildi gösterilir.
- Geçersiz sipariş numarasında anlaşılır hata mesajı gösterilir.

**Given-When-Then (Gherkin tarzı)**

```gherkin
Senaryo: Kargodaki siparişin durumunu görüntüleme
  Diyelim ki "Kargoda" durumunda bir siparişim var
  Eğer sipariş detay sayfasını açarsam
  O zaman kargo firmasını ve tahmini teslim tarihini görmeliyim
```

## 4. Örnek Hikayeler

| Rol | Hikaye | Kabul ölçütü (özet) |
|-----|--------|----------------------|
| Üye | Parolamı unuttuğumda e-posta ile sıfırlama bağlantısı almak istiyorum, böylece hesabıma tekrar girebilirim | Bağlantı 30 dk geçerli; tek kullanımlık; hesap varlığı ifşa edilmez |
| Yönetici | Aylık satış raporunu CSV olarak indirmek istiyorum, böylece Excel'de analiz edebilirim | UTF-8, başlık satırı var, seçilen ay filtrelenir |
| Destek uzmanı | Müşteri talebini kategoriye göre filtrelemek istiyorum, böylece yoğunluğu görebilirim | Kategori çoklu seçim; sonuç 2 saniye altında |

## 5. Büyük Hikayeyi Bölme Yöntemleri

1. **İş akışı adımlarına göre:** "Sipariş ver" → sepet, adres, ödeme, onay.
2. **CRUD'a göre:** oluştur, oku, güncelle, sil.
3. **Kural varyasyonlarına göre:** Farklı ödeme türleri ayrı hikayeler.
4. **Veri/arayüz farklarına göre:** Önce tek rol, sonra diğer roller.
5. **Basit/karmaşık ayrımı:** Önce en basit uçtan uca akış (tracer bullet), sonra iyileştirmeler.
6. **Fonksiyonel olmayan ihtiyaçlara göre:** Önce çalışsın, sonra performans.

Dikey dilimler (arayüz + iş mantığı + veri) yatay katmanlardan (sadece veritabanı) tercih edilir.

## 6. Tahmin

- Göreli tahmin için hikaye puanı (Fibonacci: 1, 2, 3, 5, 8, 13) veya t-shirt boyutları kullanılabilir.
- 13 ve üzeri hikayeler genelde bölünmelidir.
- Planning Poker ile konuşma ve ortak anlayış sağlanır; sayı bir hedef değil, ortak bir araçtır.

## 7. Sık Hatalar

| Hata | Düzeltme |
|------|----------|
| "Veritabanı tablosu oluştur" gibi teknik görev | Kullanıcı değerine dönüştürün veya görev olarak hikaye altına koyun |
| Fayda kısmının olmaması | "Böylece ..." bölümünü doldurun |
| Çok büyük hikaye (epik) | Bölün |
| Belirsiz kabul ölçütü ("hızlı olmalı") | Ölçülebilir hale getirin ("2 saniyenin altında") |
| Çözümü dayatmak | Problem ve değeri anlatın, çözümü takımla konuşun |
