# LabTakip

Laboratuvar ekipmanı rezervasyon, arıza ve bakım takip sistemi.
BMT-315 Yazılım Mühendisliği dönem projesi, Gazi Üniversitesi Bilgisayar Mühendisliği (2026-27 Güz, 2. şube).

## Platformlar
- **Masaüstü uygulaması:** C#
- **Mobil uygulama**
- **Ortak veritabanı ve API:** masaüstü ve mobil uygulama aynı veriye bu katman üzerinden erişir

## Klasör yapısı
```
LabTakip/
├── docs/       Proje önerisi, fizibilite raporu, UML ve ER diyagramları
├── database/   Tablo oluşturma ve örnek veri SQL scriptleri
├── src/        Kaynak kod (Visual Studio solution burada)
│   ├── LabTakip.Core/      Ortak modeller (Ekipman, Rezervasyon, ArizaKaydi, Bakim, Kullanici)
│   ├── LabTakip.Api/       Web API
│   ├── LabTakip.Desktop/   Masaüstü uygulaması
│   └── LabTakip.Mobile/    Mobil uygulama
└── tests/      Testler
```

## Ekip
| Üye | Görev |
|-----|-------|
| Akif Akçay | |
| | |
| | |
| | |
| | |

## Çalışma düzeni
- `main`: yalnızca çalışan, teslim edilebilir kod. Doğrudan push yapılmaz.
- `develop`: geliştirmelerin birleştirildiği dal.
- Her iş için `develop`'tan yeni dal açılır, örneğin `feature/rezervasyon-ekrani`, `fix/giris-hatasi`.
- İş bitince `develop`'a Pull Request açılır, en az bir kişi kontrol ettikten sonra birleştirilir.
- Çalışmaya başlamadan önce mutlaka **Fetch / Pull** yapılır.
- Commit mesajları kısa ve ne yapıldığını anlatan Türkçe cümleler olur: `Ekipman listesi ekranı eklendi`.

## Kurulum
1. Repoyu GitHub Desktop veya Visual Studio ile klonlayın.
2. `src/LabTakip.sln` dosyasını Visual Studio ile açın.
3. Veritabanı kurulumu için `database/` klasöründeki scriptleri sırayla çalıştırın.
