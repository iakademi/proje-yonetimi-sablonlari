# Proje Yönetimi Şablonları (PMP ve Scrum)

![Lisans: MIT](https://img.shields.io/badge/Lisans-MIT-green)
![PMP](https://img.shields.io/badge/PMP-%C5%9Eablonlar-0a66c2)
![Scrum](https://img.shields.io/badge/Scrum-Agile-2ea44f)
![Dil: Türkçe](https://img.shields.io/badge/Dil-T%C3%BCrk%C3%A7e-red)

Geleneksel (PMP tarzı) ve çevik (Scrum) proje yönetimi için kullanıma hazır Türkçe şablonlar ve sınav hazırlık çalışma planları.

## Hakkında

Bu depo; proje başlatma belgesi, paydaş ve risk kayıtları, WBS, iletişim planı ve değişiklik talebi gibi **PMP** süreçlerine uygun şablonları; sprint planlama, daily scrum, sprint review, retrospektif şablonları ile user story ve Definition of Done rehberlerini içerir. Ayrıca PMP ve PSM sınavlarına hazırlanmak için genel bir çalışma planı sunar.

Şablonlar genel proje yönetimi pratiklerine dayanır; PMI, Scrum.org veya başka bir kuruluşun telifli içeriğini barındırmaz. Güncel kapsam ve kurallar için ilgili kuruluşların resmi kaynaklarına başvurun.

## İçindekiler

- [Başlarken](#başlarken)
- [Şablon Listesi](#şablon-listesi)
- [Klasör Yapısı](#klasör-yapısı)
- [Katkıda Bulunma](#katkıda-bulunma)
- [Lisans](#lisans)
- [İ-Akademi Hakkında](#i-akademi-hakkında)

## Başlarken

1. Depoyu klonlayın veya ihtiyacınız olan şablonu kopyalayın:
   ```bash
   git clone https://github.com/iakademi/proje-yonetimi-sablonlari.git
   ```
2. Şablonu projenizin dokümantasyon klasörüne kopyalayıp `[köşeli parantez]` içindeki alanları kendi bilgilerinizle doldurun.
3. CSV kayıtlarını Excel, Google Sheets veya LibreOffice ile açabilirsiniz (UTF-8 kodlaması; Excel'de "Veri > Metinden/CSV'den" ile içe aktarın).

## Şablon Listesi

### PMP (`pmp/`)

| Şablon | Açıklama |
|--------|----------|
| [Proje Başlatma Belgesi](pmp/proje-baslatma-belgesi.md) | Projeyi yetkilendiren temel belge |
| [Paydaş Kaydı](pmp/paydas-kayit.md) / [CSV](pmp/paydas-kayit.csv) | Paydaş analizi ve etkileşim stratejisi |
| [Risk Kaydı](pmp/risk-kayit.md) / [CSV](pmp/risk-kayit.csv) | Risk tanımlama, puanlama ve yanıt planı |
| [WBS Örneği](pmp/wbs-ornegi.md) | İş kırılım yapısı ve sözlüğü |
| [İletişim Planı](pmp/iletisim-plani.md) | Kim, neyi, ne zaman, nasıl |
| [Değişiklik Talebi](pmp/degisiklik-talebi.md) | Entegre değişiklik kontrolü formu |

### Scrum (`scrum/`)

| Şablon | Açıklama |
|--------|----------|
| [Sprint Planlama](scrum/sprint-planlama.md) | Sprint hedefi ve backlog seçimi |
| [Daily Scrum](scrum/daily-scrum.md) | Günlük toplantı notu |
| [Sprint Review](scrum/sprint-review.md) | Increment sunumu ve geri bildirim |
| [Retrospektif](scrum/retrospektif.md) | Süreç iyileştirme oturumu |
| [User Story Rehberi](scrum/user-story-rehberi.md) | INVEST, kabul kriterleri, örnekler |
| [Definition of Done](scrum/definition-of-done.md) | Örnek DoD ve DoR |

### Sınav Hazırlık (`sinav-hazirlik/`)

- [PMP Çalışma Planı](sinav-hazirlik/pmp-calisma-plani.md)
- [PSM Çalışma Planı](sinav-hazirlik/psm-calisma-plani.md)

## Klasör Yapısı

```text
proje-yonetimi-sablonlari/
├── README.md
├── LICENSE
├── pmp/               # Geleneksel proje yönetimi şablonları
├── scrum/             # Scrum olay ve artefakt şablonları
└── sinav-hazirlik/    # PMP ve PSM çalışma planları
```

## Katkıda Bulunma

Katkılarınızı memnuniyetle karşılıyoruz.

1. Depoyu fork edin.
2. Yeni bir dal oluşturun: `git checkout -b iyilestirme/konu-adi`
3. Değişikliklerinizi açık commit mesajlarıyla kaydedin.
4. Dalınızı gönderin ve bir Pull Request açın.

Hata bildirimi veya öneri için [Issues](../../issues) bölümünü kullanabilirsiniz. Genel kurallar için organizasyonun [CONTRIBUTING.md](https://github.com/iakademi/.github/blob/main/CONTRIBUTING.md) dosyasına bakın.

## Lisans

Bu proje [MIT Lisansı](LICENSE) ile lisanslanmıştır.

## İ-Akademi Hakkında

[İ-Akademi](https://iakademi.com), İstanbul merkezli bir BT eğitim merkezidir. Microsoft/Office/Power Platform, Cisco, siber güvenlik, yazılım, PMP/Scrum/Agile ve Windows Server/Active Directory alanlarında eğitimler sunar; Pearson VUE ve Kryterion yetkili sınav merkezidir.

Web sitesi: <https://iakademi.com>
