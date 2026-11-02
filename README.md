Acil İşlem Rehberi
Acil tıp pratiğinde yapılan işlemlerin kayıt sırasında unutulmasını azaltmak için hazırlanmış, tanı ve ICD-10 koduyla aranabilen bir web uygulaması.

Geliştiren: Uzm.Dr.Yasin Yıldız, FTBEM
Özellikler
- Tanı adı veya ICD-10 koduyla işlem hatırlatmalarına ulaşma.
- İşlem adı ve koduyla doğrudan arama.
- İşlem kodu, ham puan ve kaynak açıklamalarını birlikte görüntüleme.
- Branş bazlı kategorizasyon ekindeki Kategori 8 — Acil Tıp İşlemleri için filtreleme.
- Yapılan işlemler için kontrol listesi ve kodları kopyalama.
- Birlikte puanlandırma kısıtları ve alternatif işlem seçimleri için hatırlatmalar.
- Favori işlemleri cihazda saklama.
- Mobil ekranlara uyum ve tek HTML dosyasıyla çevrimdışı kullanım.
İçerik
v1.1: 123 işlem ve 98 tanı/tanı grubu içerir. Branş bazlı kategorizasyon ekinin Kategori 8 bölümündeki 58 işlemin tamamı işaretlenmiştir. Yenidoğan/çocuk kayıtları ayrıca etiketlenmiştir.

İşlem kodları, ham puanlar ve satır açıklamaları sağlanan Genel Tıbbi İşlemler Listesi’nden; Kategori 8 üyeliği branş bazlı kategorizasyon ekinden alınmıştır. Her işlem kartında ilgili kaynak satırı görülebilir.

Tanı–işlem bağlantıları editoryal klinik hatırlatmalardır; resmî ödeme uygunluğu veya zorunlu işlem listesi değildir. Tanıların bir kısmı ICD grubu düzeyindedir; hastaya özgü alt kod HBYS üzerinden seçilmelidir.
Kurulum
1. Uygulama ZIP dosyasını çıkarın.
2. Dosyaları GitHub deponuzun ana dizinine yükleyin. index.html ana dizinde bulunmalıdır.
3. GitHub Pages yayınını dosyaların bulunduğu dal ve dizin için etkinleştirin.
Uygulama statik HTML, CSS ve JavaScript ile çalışır. Derleme, veritabanı veya sunucu tarafı uygulama gerektirmez. Aynı dosyalar standart bir web hostingine veya alt klasöre de yüklenebilir.

acil-islem-rehberi.html dosyası, uygulamanın çevrimdışı kullanılabilen tek dosyalık sürümüdür.
Dosyalar
Dosya	İçerik
index.html	Uygulamanın başlangıç sayfası
style.css	Arayüz ve mobil görünüm stilleri
app.js	Arama, filtreleme, favoriler ve kontrol listesi
data.js	Uygulamanın okuduğu işlem ve tanı verileri
data.json	Aynı verilerin okunabilir JSON kopyası
acil-islem-rehberi.html	Bağımsız, çevrimdışı sürüm
.nojekyll	GitHub Pages için statik yayın dosyası
KURULUM.txt	Kısa kurulum ve veri düzenleme notları


Veri değişikliklerinde uygulamanın data.js dosyasını okuduğunu unutmayın. Yalnız data.json dosyasını değiştirmek arayüzü güncellemez. Tek dosyalık çevrimdışı sürüm de ayrıca güncellenmelidir.
Kullanım ilkeleri
- Yalnız gerçekten yapılan ve belgelenen işlemleri seçin.
- Tanı eşleşmesi, işlemin endike olduğu veya gerçekleştirildiği anlamına gelmez.
- Kategori 8’de bulunmak, işlem satırındaki uygulayıcı, ortam, gün veya seans koşullarını kaldırmaz.
- Kategori 8’de bulunmamak tek başına yetkisizlik veya puanlandırma yasağı anlamına gelmez.
- Gösterilen ham puanlar, net ödeme veya birlikte puanlandırma garantisi değildir. Güncel mevzuat ve kurum tahakkuk kuralları ayrıca değerlendirilmelidir.
- Uygulama HBYS’ye otomatik kayıt yapmaz ve resmî faturalama sistemi değildir.
Gizlilik
Hasta adı, kimlik numarası veya dosya numarası alınmaz. Aramalar ve işlem seçimleri tarayıcıda çalışır. Favoriler cihazda saklanır; yapılan işlem seçimleri sayfa yenilenince silinir.
Kaynaklar
- Kullanıcı tarafından sağlanan Genel Tıbbi İşlemler Listesi ve branş bazlı kategorizasyon eki.
- Sağlık Bakanlığı — Genel Tıbbi İşlemler Yönergesi ve ekleri
- WHO ICD-10 referans tarayıcısı
Geliştiren: Uzm.Dr.Yasin Yıldız, FTBEM
Sürüm: 1.1 · İçerik inceleme tarihi: 2 Kasım 2026
