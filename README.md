# Rafla

**Mağazanızı denetler, yeni ürünlerinizi doğru yükler.** Rafla, Trendyol mağazanızdaki kara listedeki ve yanlış kategorideki ürünleri sebepleriyle bulur. Yeni ürünleriniz için kategoriyi, zorunlu özellikleri ve markayı yapay zekâyla seçer, ihlal riski olanları yüklemeden önce uyarır. Siz kontrol edin, tek tuşla mağazanıza yükleyin.

Windows 10 ve 11'de çalışır. Kurulum gerekmez. Sürümler bu deponun [Sürümler](https://github.com/JaxKerya/rafla/releases) sayfasında yayımlanır.

---

## Ne işe yarar?

### Mağaza denetimi

- **Kara listedeki ve kilitli ürünleri sebepleriyle listeler.** Yanlış marka, satış belgesi eksik, orijinallik şüphesi… Her sebebin ne anlama geldiği ve ne yapmanız gerektiği Türkçe yazar.
- **Yanlış kategorideki ürünleri bulur.** Yapay zekâ ürünlerinizin kategorisini bilmeden tahmin eder; %90 ve üzeri güvenle farklı bir kategori önerdiği ürünler ayrıca gösterilir.
- **Mağazanızda hiçbir şeyi değiştirmez.** Ürünler salt okunur olarak getirilir. Mağaza denetimi deneme sürümünde de sınırsızdır.

### Yeni ürün yükleme

- **Listenizi okur.** Excel, CSV ya da sitenizin XML beslemesi olur; ikas, ideasoft, Ticimax, WooCommerce ve Shopify beslemeleri desteklenir. Sütunlar otomatik tanınır. Düzenli bir listeniz yoksa hazır şablonu doldurursunuz.
- **Kategori, özellik ve marka seçer.** Trendyol'un binlerce kategorisi arasından doğru olanı yapay zekâ bulur ve zorunlu özellikleri doldurur. Emin olmadığı ürünleri size sorar. 68 ürünlük doğruluk testimizde kategori doğruluğu %91 çıktı.
- **Kontrolü size bırakır.** Güvenilir alanlar yeşil, kontrol isteyenler sarı ya da kırmızı görünür. Birden çok ürünün kategorisini ya da markasını birlikte değiştirebilirsiniz. Yaptığınız düzeltmeleri hatırlar.
- **Fiyat kuralları uygular.** Yüzde ya da sabit kâr ekleyip fiyatı yuvarlar, fiyat aralığına göre farklı kural koyabilirsiniz. Dosyanızdaki fiyat değişmez.
- **İhlal riskini önceden söyler.** Marka alanında mağaza ya da perakendeci adı, başlığın başka bir markayla başlaması, geçersiz barkod gibi Trendyol'un kara listeye aldığı durumları yüklemeden önce uyarır.
- **Mağazanızdan öğrenir.** Onaylı ürünlerinize benzeyen yeni ürünlerde onların kategorisini aday olarak kullanır; mağazada zaten olan barkodu tekrar yüklemez.
- **Toplu yükler ve takip eder.** Eksik bilgisi olan ürünleri göndermeden önce yakalar. Yüklenen ürünlerin Trendyol onayından geçip geçmediğini gösterir; reddedilenleri sebepleriyle listeler.
- **İsterse başlık ve açıklama yazar.** Trendyol'a uygun başlık ve açıklamayı yapay zekâ yeniden yazar, istediğiniz an eski hâline dönebilirsiniz.

## Nasıl başlarım?

1. [Sürümler](https://github.com/JaxKerya/rafla/releases) sayfasından `Rafla.exe` dosyasını indirin, bir klasöre koyup çift tıklayın. Uygulama tarayıcınızda açılır.
2. **Trendyol satıcı bilgilerinizi** girin: Satıcı ID, API anahtarı ve gizli anahtar. Satıcı panelinde *Hesap Bilgilerim → Entegrasyon Bilgileri* sayfasında bulunur.
3. **Mağazam** sekmesinden mağazanızı taratın; sorunlu ürünler sebepleriyle listelenir.
4. **OpenRouter anahtarı** girin. Yanlış kategori kontrolü ve eşleştirme bu anahtarla çalışır; nasıl alınacağı uygulamada 5 adımda anlatılıyor. Eşleştirme 1.000 üründe yaklaşık 1 dolar tutar, bu ücret doğrudan OpenRouter'a ödenir.
5. Yeni ürünlerinizi içe aktarın, eşleştirin, kontrol edin, yükleyin.

> **Dosyayı doğrulama:** İndirdiğiniz dosyanın değiştirilmediğini kontrol etmek için PowerShell'de `Get-FileHash Rafla.exe` yazın. Çıkan özet, sürüm notlarındaki SHA-256 özetiyle aynı olmalı.

## Deneme ve lisans

- **Mağaza denetimi** deneme sürümünde sınırsız ve ücretsizdir.
- **Ürün yükleme** deneme sürümünde **20 ürüne kadar** ücretsizdir.
- **Lisans** R10.net'teki satış konusundan alınır. Lisans tek bilgisayara bağlıdır ve süresiz çalışır.
- Lisansın güncelleme süresi içinde çıkan yeni sürümler ücretsizdir.

## Verileriniz nerede?

Ürünleriniz, ayarlarınız ve anahtarlarınız yalnızca kendi bilgisayarınızda, `Rafla.exe` dosyasının yanındaki `data` klasöründe durur. Rafla'nın bir sunucusu yoktur. Ürün bilgileri yalnızca eşleştirme için OpenRouter'a, yükleme için Trendyol'a gönderilir. Ayrıntılar [gizlilik politikasında](GIZLILIK.md).

## Güncelleme

Yeni sürüm çıktığında uygulamanın üstünde **"Yeni sürüm var"** duyurusu görünür. Yeni `Rafla.exe` dosyasını indirip eskisinin yerine koymanız yeterli. `data` klasörüne dokunmayın; ürünleriniz, ayarlarınız ve lisansınız orada kalır.

Tüm sürümler ve değişiklikler: [Sürümler](https://github.com/JaxKerya/rafla/releases)

## Destek

Sorun yaşarsanız *Ayarlar → Lisans → Destek dosyasını indir* ile oluşan dosyayı R10.net üzerinden satıcıya gönderin. Dosyada API anahtarlarınız ve lisans anahtarınız yer almaz.
