# Rafla

**Trendyol'a toplu ürün yükleme aracı.** Ürün listenizi verin; Rafla her ürünün Trendyol kategorisini, zorunlu özelliklerini ve markasını yapay zekâyla seçsin. Siz kontrol edin, tek tuşla mağazanıza yükleyin.

### [⬇ Son sürümü indir (Rafla.exe)](https://github.com/JaxKerya/rafla/releases/latest/download/Rafla.exe)

Windows 10 ve 11'de çalışır. Kurulum gerekmez.

---

## Ne işe yarar?

- **Listenizi okur.** Excel, CSV ya da sitenizin XML beslemesi olur; ikas, ideasoft, Ticimax, WooCommerce ve Shopify beslemeleri desteklenir. Sütunlar otomatik tanınır. Düzenli bir listeniz yoksa hazır şablonu doldurursunuz.
- **Kategori, özellik ve marka seçer.** Trendyol'un binlerce kategorisi arasından doğru olanı yapay zekâ bulur ve zorunlu özellikleri doldurur. Emin olmadığı ürünleri size sorar. 68 ürünlük doğruluk testimizde kategori doğruluğu %91 çıktı.
- **Kontrolü size bırakır.** Güvenilir alanlar yeşil, kontrol isteyenler sarı ya da kırmızı görünür. Birden çok ürünün kategorisini ya da markasını birlikte değiştirebilirsiniz. Yaptığınız düzeltmeleri hatırlar.
- **Fiyat kuralları uygular.** Yüzde ya da sabit kâr ekleyip fiyatı yuvarlar, fiyat aralığına göre farklı kural koyabilirsiniz. Dosyanızdaki fiyat değişmez.
- **Toplu yükler ve takip eder.** Eksik bilgisi olan ürünleri göndermeden önce yakalar. Yüklenen ürünlerin Trendyol onayından geçip geçmediğini gösterir; reddedilenleri sebepleriyle listeler.
- **İsterse başlık ve açıklama yazar.** Trendyol'a uygun başlık ve açıklamayı yapay zekâ yeniden yazar, istediğiniz an eski hâline dönebilirsiniz.

## Nasıl başlarım?

1. `Rafla.exe` dosyasını indirin, bir klasöre koyup çift tıklayın. Uygulama tarayıcınızda açılır.
2. **OpenRouter anahtarı** girin. Yapay zekâ bu anahtarla çalışır; nasıl alınacağı uygulamada 5 adımda anlatılıyor. Eşleştirme 1.000 üründe yaklaşık 1 dolar tutar, bu ücret doğrudan OpenRouter'a ödenir.
3. **Trendyol satıcı bilgilerinizi** girin: Satıcı ID, API anahtarı ve gizli anahtar. Satıcı panelinde *Hesap Bilgilerim → Entegrasyon Bilgileri* sayfasında bulunur.
4. Ürünlerinizi içe aktarın, eşleştirin, kontrol edin, yükleyin.

> **"Windows bilgisayarınızı korudu" uyarısı çıkarsa:** Bu uyarı, yeni yayıncıların imzasız programlarında görünür. **Ek bilgi → Yine de çalıştır** deyin. İndirdiğiniz dosyanın değiştirilmediğini kontrol etmek isterseniz PowerShell'de `Get-FileHash Rafla.exe` yazın. Çıkan özet, [sürüm sayfasındaki](https://github.com/JaxKerya/rafla/releases/latest) SHA-256 özetiyle aynı olmalı.

## Deneme ve lisans

- **Deneme sürümü** tüm özellikleriyle **20 ürüne kadar** ücretsizdir.
- **Lisans** R10.net'teki satış konusundan alınır. Lisans tek bilgisayara bağlıdır ve süresiz çalışır.
- Lisansın güncelleme süresi içinde çıkan yeni sürümler ücretsizdir.

## Verileriniz nerede?

Ürünleriniz, ayarlarınız ve anahtarlarınız yalnızca kendi bilgisayarınızda, `Rafla.exe` dosyasının yanındaki `data` klasöründe durur. Rafla'nın bir sunucusu yoktur. Ürün bilgileri yalnızca eşleştirme için OpenRouter'a, yükleme için Trendyol'a gönderilir. Ayrıntılar [gizlilik politikasında](GIZLILIK.md).

## Güncelleme

Yeni sürüm çıktığında uygulamanın üstünde **"Yeni sürüm var"** duyurusu görünür. Yeni `Rafla.exe` dosyasını indirip eskisinin yerine koymanız yeterli. `data` klasörüne dokunmayın; ürünleriniz, ayarlarınız ve lisansınız orada kalır.

Tüm sürümler ve değişiklikler: [Sürümler](https://github.com/JaxKerya/rafla/releases)

## Destek

Sorun yaşarsanız *Ayarlar → Lisans → Destek dosyasını indir* ile oluşan dosyayı R10.net üzerinden satıcıya gönderin. Dosyada API anahtarlarınız ve lisans anahtarınız yer almaz.
