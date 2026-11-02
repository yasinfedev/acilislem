# Acil İşlem Rehberi

Acil tıp pratiğinde yapılan işlemlerin kayıt sırasında unutulmasını azaltmak için hazırlanmış, tanı ve ICD-10 koduyla aranabilen bir web uygulaması.

**Geliştiren: Uzm.Dr.Yasin Yıldız, FTBEM**

## Özellikler

- Tanı adı veya ICD-10 koduyla işlem hatırlatmalarına ulaşma.
- İşlem adı veya koduyla doğrudan arama.
- İşlem kodu, ham puan ve puanlandırma koşullarını birlikte görüntüleme.
- **Kategori 8 — Acil Tıp İşlemleri** için filtreleme.
- Gerçekleştirilen işlemler için kontrol listesi oluşturma.
- İşlem kodlarını tek tek veya liste halinde kopyalama.
- Alternatif ve birlikte puanlandırılamayan seçimlerde uyarılar.
- Favori işlemleri cihazda saklama.
- Mobil ekranlara uyum.
- Tek HTML dosyasıyla çevrimdışı kullanım.

## İçerik

**Sürüm 1.1**, toplam **123 işlem** ve **98 tanı/tanı grubu** içerir.

Branş bazlı kategorizasyon ekinin **Kategori 8 — Acil Tıp İşlemleri** bölümündeki **58 işlemin tamamı** katalogda işaretlenmiştir. Yenidoğan ve çocuklara özgü kayıtlar ayrıca etiketlenmiştir.

İşlem kodları, ham puanlar ve açıklamalar Genel Tıbbi İşlemler Listesi’nden; Kategori 8 bilgileri ise branş bazlı kategorizasyon ekinden alınmıştır. İşlem kartlarında kaynak satırları görülebilir.

Tanı–işlem bağlantıları klinik hatırlatma amacıyla hazırlanmıştır. Tanıların bir kısmı ICD grubu düzeyindedir; hastaya özgü alt kod HBYS üzerinden seçilmelidir.

## Kullanım

1. Tanı adını veya ICD-10 kodunu arama kutusuna yazın.
2. İlgili tanıyı seçin.
3. Gösterilen işlemlerin kodlarını, puanlarını ve kayıt koşullarını inceleyin.
4. Gerçekleştirdiğiniz işlemleri **“Yaptım”** kutusuyla işaretleyin.
5. Varsa birlikte puanlandırma uyarılarını kontrol edin.
6. İşlem kodlarını kopyalayarak kayıt sırasında kullanın.

İşlem kataloğu üzerinden tanı seçmeden de işlem adı veya koduyla arama yapılabilir.

## GitHub Pages ile kurulum

1. Uygulama ZIP dosyasını çıkarın.
2. İçindeki dosyaları GitHub deponuzun ana dizinine yükleyin.
3. `index.html` dosyasının ana dizinde bulunduğundan emin olun.
4. GitHub Pages yayınını dosyaların bulunduğu dal ve dizin için etkinleştirin.

Uygulama statik HTML, CSS ve JavaScript ile çalışır. Derleme, veritabanı veya sunucu tarafı uygulama gerektirmez. Aynı dosyalar standart bir web hostingine veya alt klasöre de yüklenebilir.

## Dosya yapısı

| Dosya | Açıklama |
| --- | --- |
| `index.html` | Uygulamanın başlangıç sayfası |
| `style.css` | Arayüz ve mobil görünüm stilleri |
| `app.js` | Arama, filtreleme, favoriler ve kontrol listesi |
| `data.js` | Uygulamanın okuduğu işlem ve tanı verileri |
| `data.json` | Verilerin okunabilir JSON kopyası |
| `acil-islem-rehberi.html` | Bağımsız, çevrimdışı sürüm |
| `.nojekyll` | GitHub Pages için statik yayın dosyası |
| `KURULUM.txt` | Kısa kurulum ve veri düzenleme notları |

## Çevrimdışı kullanım

`acil-islem-rehberi.html` dosyası uygulamanın tek dosyalık sürümüdür. İndirildikten sonra internet bağlantısı olmadan tarayıcıda açılabilir.

## Veri güncelleme

Uygulama verileri `data.js` dosyasından okunur. Yalnız `data.json` dosyasını değiştirmek arayüzdeki verileri güncellemez.

Tek dosyalık çevrimdışı sürüm kendi verilerini içerir; diğer dosyalardaki değişiklikler bu sürüme otomatik yansımaz. Güncel işlem listeleri yayımlandığında veriler ve ilgili açıklamalar yeniden gözden geçirilmelidir.

## Kullanım ilkeleri

- Yalnız gerçekten yapılan ve belgelenen işlemler seçilmelidir.
- Tanı eşleşmesi, işlemin endike olduğu veya gerçekleştirildiği anlamına gelmez.
- Tanı–işlem bağlantıları resmî ödeme uygunluğu veya zorunlu işlem listesi değildir.
- Kategori 8’de bulunmak, işlem satırındaki uygulayıcı, ortam, gün veya seans koşullarını kaldırmaz.
- Kategori 8’de bulunmamak tek başına yetkisizlik veya puanlandırma yasağı anlamına gelmez.
- Gösterilen ham puanlar, net ödeme veya birlikte puanlandırma garantisi değildir.
- Güncel mevzuat, genel yönerge ve kurum tahakkuk kuralları ayrıca değerlendirilmelidir.
- Uygulama HBYS’ye otomatik kayıt yapmaz ve resmî faturalama sistemi değildir.

## Gizlilik

Hasta adı, kimlik numarası veya dosya numarası alınmaz.

Arama ve işlem seçimleri tarayıcıda çalışır. Favoriler kullanılan cihazda saklanır. Gerçekleştirilen işlem seçimleri oturum belleğinde tutulur ve sayfa yenilendiğinde silinir.

## Kaynaklar

- Uygulamanın hazırlanmasında kullanılan Genel Tıbbi İşlemler Listesi.
- Branş bazlı kategorizasyon eki.
- [Sağlık Bakanlığı — Genel Tıbbi İşlemler Yönergesi ve ekleri](https://erisilebilir.saglik.gov.tr/TR-119287/genel-tibbi-islemler-yonergesi-ve-ekleri-ile-ozellikli-tibbi-islemler-yonergesi-ve-eki-degisikligi.html)
- [WHO ICD-10 referans tarayıcısı](https://icd.who.int/browse10/2019/en)

---

**Geliştiren: Uzm.Dr.Yasin Yıldız, FTBEM**

**Sürüm:** 1.1  
**İçerik inceleme tarihi:** 2 Kasım 2026
