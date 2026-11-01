# Risk Kaydı

Proje Adı: [Proje adı] | Güncelleme tarihi: [GG.AA.YYYY] | Risk sorumlusu: [Ad]

CSV sürümü: [risk-kayit.csv](risk-kayit.csv)

## 1. Puanlama Ölçeği

| Puan | Olasılık | Etki (maliyet / takvim / kalite) |
|------|----------|----------------------------------|
| 1 | Çok düşük (<%10) | Önemsiz |
| 2 | Düşük (%10-30) | Küçük (bütçe <%2, takvim <1 hafta) |
| 3 | Orta (%30-50) | Orta (bütçe %2-5, takvim 1-3 hafta) |
| 4 | Yüksek (%50-70) | Büyük (bütçe %5-10, takvim 3-6 hafta) |
| 5 | Çok yüksek (>%70) | Kritik (bütçe >%10, takvim >6 hafta veya hedef kaybı) |

**Risk skoru = Olasılık x Etki.** 1-6 Düşük, 7-14 Orta, 15-25 Yüksek.

Fırsatlar (pozitif riskler) aynı tabloda "Tür" sütunu ile izlenebilir.

## 2. Risk Kaydı

| ID | Tür | Risk tanımı (neden → olay → etki) | Kategori | Olasılık | Etki | Skor | Yanıt stratejisi | Yanıt aksiyonu | Sahibi | Durum |
|----|-----|------------------------------------|----------|----------|------|------|------------------|-----------------|--------|-------|
| R-01 | Tehdit | Anahtar geliştirici ayrılırsa bilgi kaybı nedeniyle takvim 3 hafta uzayabilir | Kaynak | 3 | 4 | 12 | Azalt | Çift yönlü bilgi paylaşımı, dokümantasyon | PY | Açık |
| R-02 | Tehdit | Gereksinimler netleşmezse yeniden iş çıkar | Kapsam | 4 | 3 | 12 | Azalt | Prototip ve haftalık onay toplantısı | İş analisti | Açık |
| R-03 | Fırsat | Hazır bileşen kullanılırsa geliştirme 2 hafta kısalabilir | Teknik | 2 | 3 | 6 | Geliştir | Kavram kanıtı çalışması | Teknik lider | Açık |

## 3. Yanıt Stratejileri

| Tehdit için | Fırsat için | Açıklama |
|-------------|-------------|----------|
| Önle (Avoid) | Sömür (Exploit) | Belirsizliği ortadan kaldır / kesinleştir |
| Azalt (Mitigate) | Geliştir (Enhance) | Olasılık veya etkiyi değiştir |
| Transfer et (Transfer) | Paylaş (Share) | Sorumluluğu üçüncü tarafa devret / ortak ol |
| Kabul et (Accept) | Kabul et (Accept) | Aktif (yedek akçe) veya pasif |
| Eskale et | Eskale et | Kapsam dışıysa üst yönetime taşı |

## 4. Tetikleyiciler ve Yedek Planlar

| Risk ID | Tetikleyici (erken uyarı) | Yedek plan (fallback) |
|---------|---------------------------|-----------------------|
| R-01 | Önemli kişinin izin/ayrılma bildirimi | Yedek kaynak havuzundan atama |

## 5. Gözden Geçirme Notları

- Risk kaydı **her haftalık durum toplantısında** gözden geçirilir.
- Gerçekleşen riskler "Sorun (Issue)" kaydına dönüştürülür.
- Kapanan riskler silinmez; durum "Kapandı" olarak güncellenir ve alınan dersler kaydedilir.
