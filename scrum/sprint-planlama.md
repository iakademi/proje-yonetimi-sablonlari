# Sprint Planlama Şablonu

| Alan | Bilgi |
|------|-------|
| Takım / Ürün | [Takım adı] / [Ürün adı] |
| Sprint No | [Sprint 12] |
| Tarih aralığı | [GG.AA.YYYY - GG.AA.YYYY] (sprint süresi: [2 hafta]) |
| Katılımcılar | Product Owner, Scrum Master, Geliştiriciler |
| Planlama süresi (üst sınır) | Bir aylık sprint için en fazla 8 saat; daha kısa sprintlerde orantılı |

## 1. Konu 1: Bu Sprint Neden Değerli?

Product Owner, sprint için değer önerisini ve öncelikli ürün hedefiyle ilişkisini açıklar.

**Ürün Hedefi:** [Ürün hedefi]

**Önerilen Sprint Hedefi:** [Tek cümle: Bu sprint sonunda kullanıcı ... yapabilecek.]

## 2. Konu 2: Bu Sprintte Neler Yapılabilir?

Geliştiriciler, geçmiş hızlarını (velocity), kapasitelerini ve Definition of Done'ı dikkate alarak Product Backlog'dan öğe seçer.

### Kapasite

| Geliştirici | Sprintteki iş günü | İzin / toplantı | Kullanılabilir gün |
|-------------|--------------------|------------------|--------------------|
| [Ad 1] | 10 | 1 | 9 |
| [Ad 2] | 10 | 0 | 10 |
| **Toplam** | | | **19** |

Referans: Son 3 sprint hızı: [24, 28, 26] → ortalama [26] hikaye puanı.

### Seçilen Product Backlog Öğeleri

| # | Öğe | Tahmin (puan) | Kabul ölçütleri hazır mı? | Bağımlılık |
|---|-----|---------------|---------------------------|------------|
| 1 | [PBI-101 Kullanıcı girişi] | 5 | Evet | - |
| 2 | [PBI-104 Parola sıfırlama] | 3 | Evet | PBI-101 |
| 3 | [PBI-110 Rapor dışa aktarma] | 8 | Evet | Harici API |
| | **Toplam** | **16** | | |

## 3. Konu 3: Seçilen İşler Nasıl Yapılacak?

Her öğe için en az ilk günlerin işi, görevlere (≤1 gün) bölünür.

| Öğe | Görev | Sahip | Tahmin (saat) |
|-----|-------|-------|---------------|
| PBI-101 | Veritabanı şeması | [Ad] | 4 |
| PBI-101 | API uç noktaları | [Ad] | 8 |
| PBI-101 | Arayüz formu ve testler | [Ad] | 8 |

## 4. Sprint Hedefi (Son Hali)

> [Takımın birlikte kabul ettiği Sprint Hedefi]

## 5. Riskler ve Bağımlılıklar

| Konu | Önlem | Sahip |
|------|-------|-------|
| [Harici API test ortamı henüz hazır değil] | [Mock servis kullan, PO ile takip et] | [Ad] |

## 6. Planlama Kontrol Listesi

- [ ] Sprint Hedefi net ve ölçülebilir
- [ ] Seçilen tüm öğeler Definition of Ready ölçütlerini sağlıyor
- [ ] Kapasite gerçekçi (izin ve toplantılar düşüldü)
- [ ] Sprint Backlog (öğeler + plan) görünür bir yerde
- [ ] Takımın tamamı hedefe ve kapsama güveniyor
