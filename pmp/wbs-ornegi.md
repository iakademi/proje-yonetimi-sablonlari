# İş Kırılım Yapısı (WBS) Örneği

WBS, proje kapsamını teslimat odaklı olarak hiyerarşik şekilde alt parçalara ayırır. Aşağıdaki örnek, bir "Kurumsal Web Sitesi Yenileme" projesi içindir ve kurgusaldır.

## 1. WBS Hiyerarşisi

```text
1 Kurumsal Web Sitesi Yenileme
├── 1.1 Proje Yönetimi
│   ├── 1.1.1 Proje başlatma belgesi
│   ├── 1.1.2 Proje yönetim planı
│   ├── 1.1.3 Durum raporlama
│   └── 1.1.4 Proje kapanışı
├── 1.2 Analiz ve Tasarım
│   ├── 1.2.1 Gereksinim analizi
│   ├── 1.2.2 Bilgi mimarisi
│   ├── 1.2.3 Arayüz tasarımı
│   └── 1.2.4 Tasarım onayı
├── 1.3 Geliştirme
│   ├── 1.3.1 Altyapı kurulumu
│   ├── 1.3.2 Şablonların geliştirilmesi
│   ├── 1.3.3 İçerik yönetim modülleri
│   └── 1.3.4 Entegrasyonlar
├── 1.4 İçerik
│   ├── 1.4.1 İçerik envanteri
│   ├── 1.4.2 Metinlerin yazımı
│   └── 1.4.3 İçerik aktarımı
├── 1.5 Test
│   ├── 1.5.1 İşlevsel test
│   ├── 1.5.2 Performans ve güvenlik testi
│   └── 1.5.3 Kullanıcı kabul testi
└── 1.6 Yayına Alma
    ├── 1.6.1 Canlı ortam hazırlığı
    ├── 1.6.2 Geçiş ve yönlendirmeler
    ├── 1.6.3 Kullanıcı eğitimi
    └── 1.6.4 Yayın sonrası destek
```

## 2. WBS Sözlüğü (Örnek Kayıt)

| Alan | Değer |
|------|-------|
| WBS kodu | 1.3.3 |
| Çalışma paketi adı | İçerik yönetim modülleri |
| Tanım | Editörlerin sayfa, haber ve duyuru içeriklerini yönetebileceği modüllerin geliştirilmesi |
| Teslimatlar | Modül kodu, yönetim kılavuzu, birim testleri |
| Kabul ölçütü | Tüm modüllerin kabul test senaryolarını geçmesi |
| Sorumlu | Geliştirme lideri |
| Tahmini efor | 120 saat |
| Süre | 3 hafta |
| Bağımlılıklar | 1.2.4, 1.3.1 |
| Varsayımlar | Tasarım onaylı ve şablonlar hazır |
| Riskler | Gereksinim değişikliği (bkz. R-02) |

## 3. Kurallar

1. **%100 kuralı:** Alt seviyeler, üst seviyenin kapsamının tamamını içermeli, fazlasını içermemelidir.
2. **Teslimat odaklılık:** Mümkün olduğunca isim (nesne) kullanın; fiil yerine çıktıyı tanımlayın.
3. **Karşılıklı dışlama:** Aynı iş iki yerde yer almamalıdır.
4. **Çalışma paketi boyutu:** Tahmin ve takip edilebilir, tipik olarak 8-80 saat veya birkaç gün-iki hafta aralığında.
5. **Tek sorumlu:** Her çalışma paketinin tek bir sahibi olmalıdır.
6. **Kodlama:** Hiyerarşik numaralama (1.2.3) maliyet ve takvim sistemleriyle eşleşmeyi kolaylaştırır.

## 4. WBS'ten Sonraki Adımlar

WBS çalışma paketleri → faaliyetler → sıralama → süre tahmini → takvim. Maliyet hesapları ve sorumluluk atama matrisi (RACI) çalışma paketleri üzerinden kurulur.
