# Definition of Done (DoD) ve Definition of Ready (DoR) Örnekleri

**Definition of Done**, bir Increment'in "bitmiş" sayılması için gereken kalite standartlarının ortak anlayışıdır. Kuruluşun standardı varsa takım ona uyar; yoksa Scrum Takımı kendi DoD'unu oluşturur. DoD'a uymayan öğe sprint sonunda Increment'e dahil edilmez ve Product Backlog'a döner.

## 1. Örnek DoD: Kullanıcı Hikayesi Düzeyi

- [ ] Kabul ölçütlerinin tamamı karşılandı
- [ ] Kod, takım standartlarına uygun yazıldı ve en az bir takım üyesi tarafından gözden geçirildi (code review)
- [ ] Birim testleri yazıldı ve geçiyor; yeni kod için hedef kapsama düzeyi karşılandı
- [ ] Gerekli entegrasyon/otomasyon testleri çalıştı ve geçti
- [ ] Statik kod analizinde yüksek/kritik bulgu yok
- [ ] Güvenlik kontrolleri yapıldı (girdi doğrulama, yetkilendirme, bağımlılık taraması)
- [ ] Performans beklentileri doğrulandı (varsa)
- [ ] Erişilebilirlik ve tarayıcı/cihaz uyumluluğu kontrol edildi (arayüz için)
- [ ] Teknik ve kullanıcı dokümantasyonu güncellendi
- [ ] Ana dala birleştirildi ve CI hattı başarıyla tamamlandı
- [ ] Test (staging) ortamına dağıtıldı
- [ ] Product Owner öğeyi inceledi ve kabul etti

## 2. Örnek DoD: Sprint / Release Düzeyi

- [ ] Tüm seçilen öğeler hikaye düzeyi DoD'u karşılıyor
- [ ] Regresyon testleri geçti
- [ ] Bilinen kritik hata yok; kalan hatalar Backlog'a alındı ve önceliklendirildi
- [ ] Sürüm notları hazırlandı
- [ ] Geri alma (rollback) planı mevcut
- [ ] Canlıya alma kontrol listesi tamamlandı
- [ ] İzleme ve uyarılar yeni özellikler için güncellendi
- [ ] Sprint Review'da gösterilebilir bir Increment mevcut

## 3. Örnek DoR (Hazır Olma Ölçütleri)

DoR, Scrum Rehberi'nde zorunlu bir artefakt değildir; takımların Backlog öğelerini sprinte almadan önce kullandığı yardımcı bir kontrol listesidir.

- [ ] Hikaye "rol / ihtiyaç / fayda" formatında ve anlaşılır
- [ ] Kabul ölçütleri yazılı ve test edilebilir
- [ ] Takım tarafından tahmin edildi, boyutu tek sprinte sığıyor
- [ ] Bağımlılıklar (başka takım, harici servis) biliniyor ve yönetiliyor
- [ ] Tasarım/UX girdileri hazır (gerekiyorsa)
- [ ] Product Owner ile kapsam netleştirildi

## 4. DoD Gözden Geçirme

- DoD, retrospektiflerde gözden geçirilir; takım olgunlaştıkça sıkılaştırılır.
- DoD maddeleri görünür bir yerde (pano, wiki) bulunmalı.
- Maddelerin çoğu otomatikleştirilebilir olmalıdır (CI hattı, otomatik testler, lint).

## 5. Sık Sorulan Sorular

| Soru | Cevap |
|------|-------|
| DoD'u kim belirler? | Kuruluş standardı varsa o; yoksa Scrum Takımı |
| DoD sprint içinde değiştirilebilir mi? | Retrospektifte kararlaştırılıp sonraki sprintte uygulanması önerilir |
| Kısmen biten iş sayılır mı? | Hayır. Biten ya da bitmeyen vardır; yarım işin kısmi kredisi yoktur |
| Takım birden çok ise? | Ortak Increment üzerinde çalışan takımlar ortak bir DoD'u paylaşmalıdır |
