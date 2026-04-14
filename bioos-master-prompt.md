# BioOS — Landing Page Master Prompt
# Referans: Yeldra.com layout + BioOS açık tema + BioOS marka kılavuzu

---

## Görev

BioOS adlı Türkçe sağlık optimizasyon platformunun landing page'ini oluştur.
Sayfa yapısı referans görseldeki (Yeldra) ile birebir aynı olacak —
bölüm sırası, hiyerarşi, akış korunacak. Tüm içerik, renkler ve
tipografi BioOS marka sistemine göre uyarlanacak.

---

## Platform

BioOS, kullanıcıların kan tahlili, Tanita vücut ölçümü ve kişisel sağlık
verilerini yükleyebildiği; yapay zeka destekli beslenme planı, egzersiz
programı ve biyobelirteç analizi sunan entegre bir sağlık platformudur.
Her veri birbiriyle konuşur — kan tahlilinden egzersiz planına, uyku
skorundan beslenme önerisine kadar her şey tek ekosistemde çalışır.

---

## Tasarım Hissi

Apple Health'in sadeliği ile premium bir longevity kliniğinin sıcaklığı.
Bilimsel ama soğuk değil. Teknik ama insani.
Açık, nefes alan, güven veren. Hiçbir bölümde koyu zemin kullanılmaz.

---

## Marka Sistemi (Zorunlu — Tailwind default renkleri kesinlikle yasak)

```
Birincil CTA    : #E05C25  Canlı Turuncu — butonlar, vurgular
Sağlık/Başarı  : #2DAA7A  Bio Yeşili — pozitif metrikler, checkmark
Üçüncül Vurgu  : #1A8A82  Longevity Teal
Ana Metin       : #141414  Karbon
Sayfa Zemini    : #FAFAF7  Tuval — tüm sayfa boyunca
Kart Yüzeyi    : #F5F0E6  Sıcak Krem
İkincil Metin   : #6B6560  Taş Gri
Kenarlık        : #D8D2CA
```

### Fontlar (Google Fonts CDN)
```
Başlık/Display : Cormorant Garamond, weight 300, letter-spacing -1px
Body/UI        : DM Sans, weight 300/400/500, line-height 1.7
Veri/Rakamlar  : DM Mono, weight 400/500
```

### Logo
"Bio" + "OS" — OS kısmı #E05C25, Cormorant Garamond weight 300

### Buton Stili
- Primary   : #E05C25 zemin, beyaz metin, border-radius 100px
- Outline   : şeffaf zemin, #141414 kenarlık, border-radius 100px
- Her buton hover, focus-visible ve active state içerecek

---

## Sayfa Yapısı (Yeldra Sırası Korunacak)

---

### 1. NAVBAR
Yeldra'daki gibi: logo sol, linkler + CTA sağ, sticky, backdrop-blur

- Sol  : BioOS logosu
- Orta : "Nasıl Çalışır" · "Özellikler" · "Blog"
- Sağ  : "Giriş Yap" (link) + "Ücretsiz Başla" (#E05C25 buton)
- Zemin: #FAFAF7, ince alt kenarlık #D8D2CA

---

### 2. HERO — Dashboard Mockup Üstte

Yeldra'daki gibi: tam genişlik, ortada büyük dashboard ekran görüntüsü mockup'ı.
Mockup kartı (#F5F0E6 zemin, #D8D2CA kenarlık, 16px radius, hafif shadow):

Sol panel — sidebar navigasyon mockup:
  Dashboard · Kan Tahlili · Beslenme · Egzersiz · Grafikler

Orta panel — 3 metrik kartı yan yana:
  Kart 1: "KAD"        72 ms    ↑ Optimal   (#2DAA7A)
  Kart 2: "Uyku"       91/100              (#E05C25)
  Kart 3: "VO2 Max"    58.4               (#1A8A82)
  Tüm rakamlar DM Mono

Alt panel — çizgi grafik (son 8 hafta, #E05C25 çizgi)

Sağ panel — kan tahlili listesi:
  🟢 B12        890 pg/mL   İyi
  🟡 D Vitamini  42 ng/mL   Normal
  🔴 Demir       68 µg/dL   Düşük

---

### 3. BAŞLIK + ALT BAŞLIK + CTA

Yeldra'daki gibi: mockup'ın altında, sol hizalı metin bloğu

Üst etiket (DM Mono, 11px, #6B6560, letter-spacing 3px):
"BİYOLOJİK İŞLETİM SİSTEMİ"

Ana başlık (Cormorant Garamond 300, ~52px, letter-spacing -1px):
"Biyolojini anla,
hayatını tasarla."

Alt başlık (DM Sans 400, 18px, #6B6560, line-height 1.7):
"Kan tahlilinden beslenme planına, egzersizden uzun ömre —
yapay zeka ile kişiselleştirilmiş sağlık optimizasyonu.
Tüm veriler birbiriyle konuşur."

Sağda kısa açıklama metni (#6B6560, DM Sans):
"BioOS, sağlık verilerini anlamlı eyleme dönüştürür.
Hangi besinlerden kaçınacağını, hangi egzersizleri
yapacağını ve neden yapacağını bilimsel olarak gösterir."

CTA butonu: "Ücretsiz Hesap Oluştur" → #E05C25

---

### 4. NASIL ÇALIŞIR — 3 Adım (Yeldra 01/02/03 Formatı)

Yeldra'daki gibi: dikey akış, büyük numara sol tarafta, içerik sağda.
Her adımda checkmark listesi ve sonuç cümlesi.

**01. Verini Yükle**
Checkmark'lar (#2DAA7A):
✓ Kan tahlili sonuçlarını PDF veya manuel olarak gir
✓ Tanita veya benzeri cihaz ölçümlerini ekle
✓ Geçmiş sağlık bilgilerini, ilaç ve takviyelerini tanımla
✓ Sakatlık veya kısıtlamalarını sisteme bildir

Sonuç: "BioOS tüm verilerini birleştirerek benzersiz
biyolojik profilini oluşturur."

**02. AI Analiz Eder**
Checkmark'lar:
✓ Biyobelirteçlerin referans aralıklarla karşılaştırılır
✓ Eksiklikler, riskler ve öncelikler tespit edilir
✓ Beslenme ve takviye ihtiyaçları hesaplanır
✓ Egzersiz kapasiten ve kısıtlamaların değerlendirilir

Sonuç: "Saat içinde, sana özel kapsamlı bir sağlık
analizi hazır olur."

**03. Planını Takip Et**
Checkmark'lar:
✓ Haftalık güncellenen kişisel beslenme planı
✓ Sakatlık geçmişine göre özelleştirilmiş egzersiz programı
✓ Hangi değerlerin neden kritik olduğunu öğren
✓ Canlı grafiklerle ilerlemeyi haftalık izle

Sonuç: "Verilerini platforma bağladıkça sistem
sürekli öğrenir ve planı geliştirir."

---

### 5. HEDEF KİTLE KARTLARI (Yeldra'daki 2 Kart Formatı)

Yeldra'da "Indépendants avancés" ve "Accompagnants business" gibi
iki ayrı kart var. BioOS için:

**Kart 1 — Performans Odaklı** (#F5F0E6 zemin, #D8D2CA kenarlık)
Başlık: "Sporcu ve Performans Meraklıları"
Alt: "VO2 Max'ını artırmak, toparlanmayı hızlandırmak
ve pik performansa ulaşmak isteyenler için."

Sol: Ne Sunar
✓ Egzersiz kapasitesi ve toparlanma analizi
✓ Antrenman öncesi/sonrası beslenme rehberi
✓ Uyku kalitesi ve HRV optimizasyonu
✓ Takviye ve hidrasyon protokolleri

Sağ: Kullanıcı faydası
"Haftalık antrenmandan %23 daha fazla verim
aldığını raporlayan kullanıcılar."

Buton: "Keşfet" → #E05C25

**Kart 2 — Genel Sağlık** (#FAFAF7 zemin, #D8D2CA kenarlık)
Başlık: "Sağlığını Uzun Vadede Yönetmek İsteyenler"
Alt: "Kan değerlerini anlamak, yaşam kalitesini artırmak
ve erken önlem almak isteyenler için."

Sol: Ne Sunar
✓ Kapsamlı kan tahlili yorumlama
✓ Kişiselleştirilmiş beslenme ve diyet planı
✓ Vitamin ve mineral eksikliği tespiti
✓ Doktora gitmeden önce ne sormalısın rehberi

Sağ: Kullanıcı faydası
"Kullanıcıların %78'i ilk 30 günde en az bir
kritik eksikliği fark ettiğini bildiriyor."

Buton: "Başla" → outline

---

### 6. İSTATİSTİKLER (Yeldra +50% / 1h Formatı)

Yeldra'daki gibi: büyük rakamlar, altında açıklama, yan yana

  **+40%**
  Kullanıcıların ilk 3 ayda raporladığı
  enerji ve performans artışı

  **15 dk**
  İlk analizin tamamlanma süresi.
  Kan tahlilini yükle, planın hazır.

  **%91**
  Haftalık beslenme planına uyum
  oranı — otomatik güncelleme sayesinde

---

### 7. TESTİMONYALLAR (Yeldra Formatı)

Yeldra'daki gibi: büyük alıntı sol, avatar + isim sağ.
Karışık: bazı uzun form, bazı kısa istatistik bazlı.

**Testimonyal 1** (uzun format):
"Yıllardır yorgunluk ve konsantrasyon sorunuyla yaşıyordum.
Doktorlar 'değerlerin normal' diyordu. BioOS analizi ferritin
düzeyimin optimal aralığın altında olduğunu ve D vitamini
emilimimin yetersiz kaldığını gösterdi. 6 hafta içinde fark
ettim. Bu platform gerçekten hayat değiştiriyor."
— Ayşe K., İstanbul

**Testimonyal 2** (istatistik format):
**%34**
"VO2 Max değerimde 12 haftada bu artışı sağladım.
BioOS'un egzersiz ve beslenme entegrasyonu olmadan
bu mümkün olmazdı."
— Mert T., İzmir

**Testimonyal 3** (uzun format):
"Diyetisyen ve kişisel antrenörle çalışıyordum ama verilerim
hiç bir arada değerlendirilmiyordu. BioOS her şeyi tek
platforma taşıdı. Artık antrenörüme BioOS raporumu
gönderiyorum, çok daha verimli çalışıyoruz."
— Selin A., Ankara

---

### 8. SSS (Yeldra Accordion Formatı)

Yeldra'daki gibi: accordion/açılır kapanır sorular, ince kenarlık

S: Kan tahlilimi nasıl yükleyebilirim?
S: Hangi cihazlar destekleniyor?
S: Verilerim güvende mi?
S: Doktorum yerine mi geçiyor?
S: Planım ne sıklıkla güncelleniyor?

---

### 9. SON CTA BÖLÜMÜ

Büyük başlık (Cormorant Garamond 300, ~48px):
"Biyolojinin seni sınırlamasına
izin verme."

Alt metin: "Ücretsiz başla, kredi kartı gerekmez."
Buton: "Ücretsiz Hesap Oluştur" → #E05C25

---

### 10. FOOTER

- Sol  : BioOS logosu + "Biyolojik İşletim Sistemi" (DM Mono, küçük)
- Orta : Gizlilik · Kullanım Koşulları · İletişim · Blog
- Alt  : "© 2026 BioOS · Yüksek Performans Mimarı İlker · Melbourne"
- Zemin: #F5F0E6, üst kenarlık #D8D2CA

---

## Teknik Gereksinimler

- Tek index.html dosyası, tüm stiller inline
- Tailwind CSS CDN
- Google Fonts CDN (Cormorant Garamond + DM Sans + DM Mono)
- Chart.js CDN — hero grafiği ve dashboard için
- Placeholder görseller: https://placehold.co/
- Accordion/SSS için vanilla JS
- Tüm içerik Türkçe
- Mobile-first, tam responsive
- Koyu arka plan hiçbir bölümde kullanılmaz

## Bileşen Kuralları

- Kartlar      : #F5F0E6 zemin · 1px #D8D2CA kenarlık · 12-16px radius
- Metrikler    : DM Mono · #2DAA7A pozitif · #E05C25 dikkat
- Bölüm label  : DM Mono · 10-11px · letter-spacing 3px · uppercase · #6B6560
- Adım numaraları: Cormorant Garamond · 300 weight · büyük · #E05C25
- Checkmark    : #2DAA7A renk · SVG veya unicode ✓
- Shadow       : Flat shadow-md yasak · color-tinted, düşük opacity kullan

---

## Kalite Standardı

Screenshot al → marka kurallarıyla karşılaştır → düzelt → tekrar screenshot.
En az 2 tur. "AI çıktısı" değil, gerçekten tasarlanmış hissi vermeli.
Yeldra'nın bölüm akışı korunmalı, BioOS'un sıcaklığı hissedilmeli.
