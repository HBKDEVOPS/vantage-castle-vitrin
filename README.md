<p align="center">
  <img src="screenshots/vitrin-hero.gif" alt="Vantage Castle: Panom, Harita, Emtialar ve Emtia Ağı ekranlarından hareketli bir tur" width="100%">
</p>

# Vantage Castle

[English](README.en.md)

Web sitesi: [vantagecastle.com](https://vantagecastle.com)

**Emtia fiyatları bir şirketin marjına nasıl yansır? Tek ekranda, her sayının kaynağıyla.**

Vantage Castle, BIST şirketlerinin girdi emtia maliyetini çıktı fiyatıyla aynı eksene koyar ve yanına şirketin açıkladığı gerçekleşen brüt marjı yerleştirir. Bir şirketin hammadde sepeti pahalandı mı, sattığı ürünün fiyatı bunu karşıladı mı: ikisi yan yana görünür. Projeksiyon sayfasındaki hesabı **Emtia Marj Motoru** yapar: şirketin finansallarına, emtialarına ve girdi–çıktısına bakar, brüt marjın bir sonraki bilançoda nereye gelebileceğini bilanço açıklanmadan önce hesaplar ve kayda geçirir; gerçekleşen değer gelince yanına eklenir. Bu bir hesaptır; hisse fiyatı ya da yatırım yönü bildirmez ve yatırım tavsiyesi değildir. Motorun nasıl çalıştığı [Emtia Marj Motoru](#emtia-marj-motoru) bölümünde anlatılır.

Ürünün sol menüsü şu sırayladır; bu belgedeki ekranlar da aynı sırayla verilir:

- **Panom.** Kendi takip ekranınız; pencereleri siz seçersiniz.
- **Değişimler** (alt başlığı **Bülten**). Seçtiğiniz tarihten beri ne değişti; haftalık bülten.
- **Şirketler.** Yedi sekme: şirket detayları ve marj akışı, çeyreklik veriler, ızgara ve dört ölçüye göre sıralama.
- **Projeksiyon.** Emtia hareketinin brüt marja aritmetik etkisi; beş görünüm. Bir hesaptır, yön iddiası değildir.
- **Sektörler** (alt başlığı **Eşleşme matrisi**). Sektör marjları, sektöre bağlı emtialar ve girdi eşleşmesi.
- **Emtia** (alt başlığı **Emtia Ağı**). Emtia fiyatları ve hangi emtianın hangi sektörlerle bağlı olduğu.
- **Harita** (alt başlığı **Tedarik Zinciri**). Dünya haberleri ve şirketlerin girdi emtialarının Türkiye'ye geliş yolları.
- **KAP.** Bildirim listesi.
- **Veri.** Kaynak, Veri kalitesi ve Terimler.
- **Ayarlar.** Dil, görünüm, menü ve başlangıç sayfası.

**Tarama** sayfası (tüm şirketler tek tabloda) sol menüde yer almaz; genel arama kutusunda sayfa olarak bulunur.

Bu depo bir vitrindir: kod ve veri içermez. Sayfa görüntüleri ürünün maskeli kipinde alınmıştır: hisse fiyatı, KAP bildirimleri, bilanço tabloları, haber başlıkları, elektrik (EPİAŞ) ve geçiş noktası (PortWatch) değerleri ile hesap bilgileri görüntüye girmez; yerinde "—" ya da boşluk durur. Arayüz Türkçedir; İngilizce seçeneği Ayarlar'dadır ve çeviri sürmektedir. [Kaynak: ürünün Ayarlar sayfası, 17.11.2026]

## İçindekiler

- [Ne yapar](#vantage-castle)
- [Ekranlar](#ekranlar): [Panom](#panom) · [Değişimler](#değişimler) · [Bülten](#bülten) · [Şirketler](#şirketler) · [Projeksiyon](#projeksiyon) · [Sektörler](#sektörler) · [Eşleşme matrisi](#eşleşme-matrisi) · [Emtia](#emtia) · [Takip edilen emtialar](#takip-edilen-emtialar) · [Ayrıca izlenen emtialar](#ayrıca-izlenen-emtialar) · [Emtia Ağı](#emtia-ağı) · [Harita](#harita) · [Tedarik Zinciri](#tedarik-zinciri) · [KAP](#kap) · [Kaynak](#kaynak) · [Veri kalitesi](#veri-kalitesi) · [Terimler](#terimler) · [Ayarlar](#ayarlar) · [Tarama](#tarama) · [Ana sayfa](#ana-sayfa) · [Giriş](#giriş) · [Kaydol](#kaydol) · [Hakkımızda](#hakkımızda)
- [Emtia Marj Motoru](#emtia-marj-motoru)
- [Yöntem](#yöntem)
- [Dürüst bulgular](#dürüst-bulgular)
- [Mimari](#mimari)
- [Ekip](#ekip)
- [Ne yapmaz](#ne-yapmaz)
- [Durum](#durum)
- [Lisans ve atıflar](#lisans-ve-atıflar)

Yöntem, bulgular, mimari ve ekip bölümlerinde kısa bir özet vardır; tam metin "Ayrıntılar" kutusunun içindedir ve [docs](docs/) klasöründe de durur.

## Ekranlar

Sayfalar ürünün sol menüsündeki sırayla verilir; görüntülerin dosya numaraları (01, 02, …) bu sırayı izlemez. Görüntülerde hisse fiyatı, KAP bildirimleri, bilanço tabloları, haber başlıkları, elektrik (EPİAŞ) ve geçiş noktası (PortWatch) değerleri ile hesap bilgileri bulunmaz; yerinde "—" ya da boşluk durur. Bu bölümdeki sayfa tanımları ürünün canlı hâliyle 17.11.2026'da karşılaştırıldı; sayıları canlı değerlerdir ve değişir, bu yüzden yazılmadı.

Üstteki çubukta her sayfada bir veri tazelik şeridi durur: "Çekim … Emtia (resmi seri): n güncel, m gecikmede". Emtia serilerinden kaçının güncel, kaçının gecikmede olduğunu gösterir. [Kaynak: ürünün üst çubuğu, canlı, 17.11.2026]

### Panom

Kendi takip ekranınız; pencereleri siz seçersiniz. Favori şirketler (Yıldızlılar), emtia grafiği, ısı takvimi, kur (TL karşısında) ve bültenler varsayılan düzende tek panoda durur. Üstte Düzenim, Bildirimler, Pencere ekle ve Düzen düğmeleri bulunur. Düzeninizi kaydedersiniz; Alt+1–9 ile düzenler arasında geçersiniz. Şirketlerden, emtialardan ve sayfalarınızdan pencere seçersiniz; yeni pencere ilk boş yere gelir. Aşağıdaki görüntüdeki düzen varsayılan değil, örnek bir düzendir.

![Panom: emtia listeleri, fiyat grafiği, emtia kartı ve ısı takvimi](screenshots/01-panom.png)

### Değişimler

Seçtiğiniz tarihten beri ne değişti, tek sayfada. Üstte beş aralık düğmesi (Son girişim, Bugün, 7 gün, 30 gün, 90 gün) ve bir tarih seçici bulunur; ilk ziyarette son 30 gün gösterilir. Sayfa hesap yapmaz, değişenleri kutular hâlinde dizer; hiçbir şeyin değişmediği kutu çizilmez. Kutular: Bilançolar (brüt ve net marj; net marjı hasılatı aşan şirketler ayrıca), Emtia fiyatları (dolar), Bilanço hesap kayıtları, KAP bildirimleri, Kur (TL karşısında), Olağandışı emtia hareketleri, Sektörlere göre brüt marj ve Bültenler. Altta "Veri güncelliği" ve "Değişmeyenler" satırları durur; kur kutusunda kaynağı (TCMB EVDS) yazar. [Kaynak: ürünün Değişimler sayfası, canlı, 17.11.2026]

![Değişimler sayfası, 90 günlük aralık: emtia fiyatları, olağandışı hareketler, kur ve bültenler](screenshots/05-degisimler.png)

### Bülten

Değişimler'in alt başlığıdır. Haftalık bülten: dönemde açıklanan bilançolar, şirketlerin güncel brüt ve net marjı, emtia hareketleri, şirketlerin girdi etkisi ve emtia–şirket etki matrisi, Projeksiyon kayıtları, yeni bildirimler ve yaklaşan bilanço takvimi tek sayfada. Sayfada Haftalık ve Olağandışı sekmeleri, hafta seçici ve PDF indirme düğmesi bulunur. Sayısal ölçümler otomatik üretilir; yayımlanan bülten sonradan değişmez, düzeltme yeni sayıyla yapılır. Bülten "Yatırım tavsiyesi değildir" uyarısını taşır. Görüntüde marjlar ve sayılar "—" görünür. [Kaynak: ürünün Bülten sayfası, canlı, 17.11.2026]

![Bülten sayfası: haftalık bülten özeti, marj tablosu, emtia hareketleri ve emtia–şirket etki matrisi; sayılar "—"](screenshots/06-bulten.png)

### Şirketler

Sayfanın yedi sekmesi vardır; solda sektöre göre gruplanmış şirket listesi şirket seçici olarak durur ([Kaynak: ürünün Şirketler sayfası, canlı ve ön yüz kaynağı, 17.11.2026]):

1. **Şirket detayları.** Seçili şirketin sayfası: marj akışı, girdi ve çıktı endeksi, girdi fiyatları, Projeksiyon özeti ve mali tablo tek sayfada. Hisse fiyatı, hacim, KAP ve bilanço değerleri görüntüde "—" görünür.
2. **Çeyreklik veriler.** Şirketlerin çeyrek çeyrek değerleri. Ölçü seçilir (brüt marj, FAVÖK, FAVÖK marjı, net kâr marjı, net borç/FAVÖK), oransal ya da hacimsel gösterim ve değer ya da değişim seçilir; liste yıldızlı şirketlere ya da kendi listelerinize süzülür.
3. **Izgara.** Her şirket için küçük bir kart: brüt marjın son çeyrek değişimi (puan) ve son 12 çeyreğin çizgisi.
4. **Brüt marj, FAVÖK marjı, Borçluluk, Net kâr marjı.** Dört sekme, şirketleri seçilen ölçüye göre sıralayan grafiktir; ölçüyü açıklayanlar düzeye göre, henüz açıklamayanlar altta gri dizilir. Borçluluk, net borcun son dört çeyrek FAVÖK'üne oranıdır.

![Şirketler sayfasının Izgara sekmesi: her şirket için brüt marj kartı; değerler "—"](screenshots/03-sirketler-izgara.png)

![Şirketler sayfası: marj akışı, girdi ve çıktı endeksi, girdi fiyatları, Projeksiyon özeti ve mali tablo; değerler "—"](screenshots/03-sirketler.png)

Marj akışı: çıktının fiyatı 100 alınır; girdi kalemleri ayrı şeritler olarak soldan akar, her şeridin yanında sepet içindeki payı yazar. Şeritler girdi sepetinde birleşir, çıktıdan sepetin payı çıkınca kalan marj farkı kutusuna gider. Faiz ve kur gibi makro büyüklükler sepetin dışında ayrı bir koridorda durur; "Operasyon" şeridi katsayıyla yansımayan maliyeti gösterir. "Bugün" görünümü son kaydı gösterir; "Ya şöyle olursa" görünümünde bir girdi kaleminin değişimini siz verirsiniz ve akış aynı hesapla yeniden çizilir (çıktı fiyatı sabitken). Sepet payı şirketin KAP'ta yayımladığı finansal rapordaki brüt marjdan, kalem ağırlıkları ürünün hesap kuralından gelir ([Yöntem §1 ve §4](#yöntem)). Akıştaki sayılar şirketin KAP'ta yayımladığı brüt marjdan türediği için görüntüde "—" görünür; şeritlerin kalınlığı yalnız düzeni gösterir.

![Şirketler sayfasının Marj akışı paneli: girdi kalemleri, girdi sepeti ve marj farkı; sayılar "—"](screenshots/03-sirketler-marj-akisi.png)

Akışın sırası, değer taşımayan bir şemada: önceki marja emtia girdi etkisi ve emtia çıktı etkisi eklenir, sonuç hesap marjıdır. Girdi etkisindeki 90 günlük pencere örnektir (ürünün ayarlarında pencere 30, 90 ve 180 gündür; ayrıntı [Yöntem §5](#yöntem)).

![Marj akışı şeması](diagrams/marj-akisi.png)

### Projeksiyon

Emtia hareketinin brüt marja aritmetik etkisini "diğer her şey sabit kalırsa" varsayımıyla hesaplar; sayfanın üstündeki uyarı bunun bir hesap olduğunu ve yön iddiası taşımadığını söyler. Hesabı [Emtia Marj Motoru](#emtia-marj-motoru) yapar. Sayfanın beş görünümü vardır; sayfanın üstünde şirket seçici ve çeyrek etiketi bulunur; görüntülerde sayılar "—" görünür.

**Emtia.** Her şirket için iki yöntemin bloğu ayrı durur: "Emtia fiyatından" ve "Şirket finansallarından · ön kayıtlı yöntem". İkinci blokta "Senaryo hesabı (orta)", "Bant (alt – üst)" ve "Hesaplanan brüt marj" satırları, ölçülemeyen şirket-çeyrekte ise nedeni ("ölçülemedi: …") yazar. Altta marj akışı (önceki marj, iki etki, hesap marjı) ve "Sebepler: sayı akışı" bölümü adım adım dökümü verir: girdi etkisi ve çıktı etkisi.

![Projeksiyon, Emtia görünümü: marj akışı ile girdi ve çıktı etkisinin adım adım dökümü](screenshots/07-projeksiyon-emtia.png)

**Makro.** Kur ve enflasyonun brüt marja etkisi; henüz hesapta değildir, ekran bunu "henüz hesapta değil" diye yazar.

![Projeksiyon, Makro görünümü: kur ve enflasyon etkisi henüz hesapta değil](screenshots/07-projeksiyon-makro.png)

**Operasyonel.** Hacim, kapasite ve hedge etkisi; henüz hesapta değildir, ekran bunu "henüz hesapta değil" diye yazar.

![Projeksiyon, Operasyonel görünümü: hacim, kapasite ve hedge etkisi henüz hesapta değil](screenshots/07-projeksiyon-operasyonel.png)

**Senaryo hesabı.** Girdi sepeti ve çıktı sepeti için değişimi siz verirsiniz (kaydırıcı ya da yüzde kutusu); diğer her şey sabit kalır ve marj akışı aynı hesapla yeniden çizilir.

![Projeksiyon, Senaryo hesabı görünümü: girdi ve çıktı sepeti için kaydırıcılar, marj akışı ve adım adım döküm](screenshots/07-projeksiyon-senaryo.png)

**Gerçekleşen.** Bilanço açıklayan şirketlerde önceki kayıtlı hesabı gerçekleşen marjla yan yana koyar; "Hesap türü" sütunu hesabın hangi yöntemden geldiğini yazar. Kaydı olmayan şirkette model çıktısı yoktur ve referans olarak son çeyreğin gerçekleşen marjı gösterilir ([Referans marj](#emtia-marj-motoru)). Demo kipinde bu görünüm menüde listelenmez.

![Projeksiyon, Gerçekleşen görünümü: bilanço açıklayan şirketlerde kayıtlı hesap ile gerçekleşen marj yan yana; değerler "—"](screenshots/07-projeksiyon-gerceklesen.png)

### Sektörler

Sektör seçilince sektör brüt marjı (1Y, 3Y, 5Y ya da tümü), sektördeki şirketlerin brüt marj değişiminin dağılımı, sektör içi brüt marj ve sektöre bağlı emtialar görülür. Normal kipte marj panelleri çalışır; depodaki maskeli karede marj panelleri "henüz hesapta değil" der, sektör–emtia matrisi durur. Matriste sayı, o emtiayı sepetinde taşıyan şirket sayısıdır; koyuluk, sektördeki şirketlere oranıdır. Demo kipinde bu marj sayfası listelenmez. [Kaynak: ürünün Sektörler sayfası, canlı, 17.11.2026]

![Sektörler sayfası: sektör seçici, marj panelleri ve sektöre bağlı emtia matrisi](screenshots/08-sektorler.png)

### Eşleşme matrisi

Sektörler'in alt başlığıdır. Her şirketin her girdisinin doğrudan mı, yoksa vekil (proxy) bir seriyle mi eşlendiğini tek tabloda gösterir. Satırlar şirketlerdir (borsa kodu ve sektör), sütunlar emtialardır; üstteki üç sayaç tam eşleşmiş (vekil yok), en az bir vekil eşleşmesi olan ve hiç girdi verisi bulunmayan şirketleri sayar. Sektör ve emtia seçicileri ile "Tümü", "Sadece doğrudan" ve "Sadece proxy" düğmeleri tabloyu süzer. Yıldız vekil eşleşme, "—" veri yok demektir. Görüntüde sayaçlardaki ve hücrelerdeki sayılar "—" görünür; tablo yatay kaydığı için karede yalnız sol kısmı vardır. [Kaynak: ürünün Eşleşme matrisi sayfası]

![Eşleşme matrisi: şirketler satırda, emtialar sütunda; yıldız vekil eşleşme; sayılar "—"](screenshots/08-eslesme-matrisi.png)

### Emtia

Emtia fiyatları, seçili serinin grafiği, kaynağı ve birimiyle. Sayfada emtia kartı şeridi, sektöre göre gruplanmış emtia listesi, çoklu seçim, seçili serinin grafiği, ısı takvimi ve ufuk grafiği bulunur. Fiyatlar resmî serilerdir: çoğu aylık, bazıları düzensiz aralıklıdır (emtia kartında ve grafik başlığında serinin sıklığı yazar); ayrıca günlük takip edilen seriler de vardır. [Kaynak: ürünün Emtialar sayfası, canlı, 17.11.2026]

![Emtia sayfası: emtia kartı şeridi, emtia listesi, bütan grafiği, ısı takvimi ve ufuk grafiği](screenshots/04-emtia.png)

### Takip edilen emtialar

Yukarıdaki Emtia sayfasının listesinde **82 emtia** bulunur; liste aşağıda iki tabloya ayrılır. İlk tablo, kaynağı bu belgenin [Lisans ve atıflar](#lisans-ve-atıflar) bölümünde gösterilen **29 emtiayı** içerir: enerji 7, metaller 5, tarım 5, kimya ve gübre 7, diğer hammadde 5; bu tabloda her emtianın Türkçe ve İngilizce adı, grubu ve kaynağı yazar. İkinci tablo ([Ayrıca izlenen emtialar](#ayrıca-izlenen-emtialar)) geri kalan **53 emtiayı** içerir: enerji 13, metaller 16, tarım 14, kimya ve gübre 7, diğer hammadde 3. Grup editöryel bir sınıflandırmadır, hesaba katılmaz. [Kaynak: ürünün emtia listesi, 17.11.2026; sayılar iki tablodaki satır sayılarıdır, 29 + 53 = 82]

| Emtia (Türkçe) | Commodity (İngilizce) | Grup | Kaynak |
|---|---|---|---|
| Bütan | Butane | Enerji | FRED, Federal Reserve Bank of St. Louis (EIA ve BLS serileri) |
| Fuel oil | Fuel oil | Enerji | FRED, Federal Reserve Bank of St. Louis (EIA ve BLS serileri) |
| İthal kömür (Newcastle) | Imported coal (Newcastle) | Enerji | FRED, Federal Reserve Bank of St. Louis (IMF serileri) |
| Jet yakıtı | Jet fuel | Enerji | FRED, Federal Reserve Bank of St. Louis (EIA ve BLS serileri) |
| LPG (Propan) | LPG (propane) | Enerji | FRED, Federal Reserve Bank of St. Louis (EIA ve BLS serileri) |
| Petrokok | Petroleum coke (petcoke) | Enerji | FRED, Federal Reserve Bank of St. Louis (EIA ve BLS serileri) |
| Uranyum | Uranium | Enerji | FRED, Federal Reserve Bank of St. Louis (IMF serileri) |
| Hurda çelik | Steel scrap | Metaller | FRED, Federal Reserve Bank of St. Louis (EIA ve BLS serileri) |
| Kalay | Tin | Metaller | FRED, Federal Reserve Bank of St. Louis (IMF serileri) |
| Kurşun | Lead | Metaller | FRED, Federal Reserve Bank of St. Louis (IMF serileri) |
| Nikel | Nickel | Metaller | FRED, Federal Reserve Bank of St. Louis (IMF serileri) |
| Çinko | Zinc | Metaller | FRED, Federal Reserve Bank of St. Louis (IMF serileri) |
| Arpa/malt | Barley / malt | Tarım | FRED, Federal Reserve Bank of St. Louis (EIA ve BLS serileri) |
| Kahve (Robusta) | Coffee (Robusta) | Tarım | FRED, Federal Reserve Bank of St. Louis (IMF serileri) |
| Palm yağı | Palm oil | Tarım | The World Bank, Commodity Price Data (The Pink Sheet) |
| Pirinç | Rice | Tarım | FRED, Federal Reserve Bank of St. Louis (IMF serileri) |
| Çiğ süt | Raw milk | Tarım | Ulusal Süt Konseyi |
| DAP (gübre) | DAP (diammonium phosphate, fertiliser) | Kimya ve gübre | The World Bank, Commodity Price Data (The Pink Sheet) |
| Fosfat kayası | Phosphate rock | Kimya ve gübre | The World Bank, Commodity Price Data (The Pink Sheet) |
| Karbon siyahı | Carbon black | Kimya ve gübre | FRED, Federal Reserve Bank of St. Louis (EIA ve BLS serileri) |
| Mürekkep | Ink | Kimya ve gübre | FRED, Federal Reserve Bank of St. Louis (EIA ve BLS serileri) |
| Potas | Potash (potassium chloride) | Kimya ve gübre | The World Bank, Commodity Price Data (The Pink Sheet) |
| Tuz | Salt | Kimya ve gübre | FRED, Federal Reserve Bank of St. Louis (EIA ve BLS serileri) |
| Üre (gübre) | Urea (fertiliser) | Kimya ve gübre | The World Bank, Commodity Price Data (The Pink Sheet) |
| Doğal kauçuk | Natural rubber | Diğer hammadde | FRED, Federal Reserve Bank of St. Louis (IMF serileri) |
| Kereste (sert, Japonya) | Hardwood sawnwood (Japan) | Diğer hammadde | FRED, Federal Reserve Bank of St. Louis (IMF serileri) |
| Kereste (yumuşak) | Softwood lumber | Diğer hammadde | FRED, Federal Reserve Bank of St. Louis (IMF serileri) |
| Selüloz / atık kağıt | Pulp / recovered paper | Diğer hammadde | FRED, Federal Reserve Bank of St. Louis (EIA ve BLS serileri) |
| Yün (Fine) | Wool (fine) | Diğer hammadde | FRED, Federal Reserve Bank of St. Louis (IMF serileri) |

Kaynak sütunu, [Lisans ve atıflar](#lisans-ve-atıflar) bölümündeki atıf adlarıyla aynıdır. [Kaynak: ürünün emtia listesi, 17.11.2026]

### Ayrıca izlenen emtialar

Bu emtiaların fiyat verisinin lisansı inceleniyor; bu depoda fiyatları gösterilmez.

| Emtia (Türkçe) | Commodity (İngilizce) | Grup |
|---|---|---|
| Benzin · New York Limanı | Gasoline · New York Harbor | Enerji |
| Brent ham petrol · Küresel (Brent) | Brent crude oil · Global (Brent) | Enerji |
| Doğalgaz · ABD (Henry Hub) | Natural gas · U.S. (Henry Hub) | Enerji |
| Doğalgaz · Avrupa (TTF) | Natural gas · Europe (TTF) | Enerji |
| Elektrik (Türkiye PTF) | Electricity (Türkiye day-ahead price / PTF) | Enerji |
| Ham petrol · Çin | Crude oil · China | Enerji |
| Ham petrol · Orta Doğu (Dubai) | Crude oil · Middle East (Dubai) | Enerji |
| Kok · Çin | Coke · China | Enerji |
| Kok kömürü · Çin | Coking coal · China | Enerji |
| Kömür · Güney Afrika (Richards Bay) | Coal · South Africa (Richards Bay) | Enerji |
| LNG · Japonya (ithalat / CIF) | LNG · Japan (import / CIF) | Enerji |
| Motorin · New York Limanı | Diesel · New York Harbor | Enerji |
| WTI ham petrol · ABD (WTI) | WTI crude oil · U.S. (WTI) | Enerji |
| Altın · Uluslararası | Gold · International | Metaller |
| Alümina · Çin | Alumina · China | Metaller |
| Alüminyum · Çin | Aluminium · China | Metaller |
| Alüminyum · Uluslararası | Aluminium · International | Metaller |
| Bakır · ABD | Copper · U.S. | Metaller |
| Bakır · Çin | Copper · China | Metaller |
| Çinko · Çin | Zinc · China | Metaller |
| Demir cevheri · Çin | Iron ore · China | Metaller |
| Demir cevheri · Uluslararası | Iron ore · International | Metaller |
| Ferrosilikon · Çin | Ferrosilicon · China | Metaller |
| Gümüş · Uluslararası | Silver · International | Metaller |
| Nikel · Çin | Nickel · China | Metaller |
| Paladyum · Çin | Palladium · China | Metaller |
| Platin · Uluslararası | Platinum · International | Metaller |
| Silikomangan · Çin | Silicomanganese · China | Metaller |
| Soğuk haddelenmiş çelik (ABD ÜFE) | Cold-rolled steel (U.S. PPI) | Metaller |
| Ayçiçek yağı · AB (FOB Rotterdam) | Sunflower oil · EU (FOB Rotterdam) | Tarım |
| Buğday · ABD (HRW) | Wheat · U.S. (HRW) | Tarım |
| Buğday · ABD (SRW) | Wheat · U.S. (SRW) | Tarım |
| Buğday · Türkiye | Wheat · Türkiye | Tarım |
| Kahve (Arabica) · Uluslararası | Coffee (Arabica) · International | Tarım |
| Kakao | Cocoa | Tarım |
| Karkas et (dana) | Beef carcass | Tarım |
| Mısır · ABD | Corn · U.S. | Tarım |
| Mısır nişastası · Çin | Corn starch · China | Tarım |
| Soya · ABD | Soybeans · U.S. | Tarım |
| Soya küspesi · Çin | Soybean meal · China | Tarım |
| Soya küspesi · Uluslararası | Soybean meal · International | Tarım |
| Soya yağı · Çin | Soybean oil · China | Tarım |
| Şeker | Sugar | Tarım |
| MEG · Çin | Ethylene glycol (MEG) · China | Kimya ve gübre |
| Metanol · Çin | Methanol · China | Kimya ve gübre |
| Paraksilen · Çin | Paraxylene · China | Kimya ve gübre |
| Polietilen · Çin | Polyethylene · China | Kimya ve gübre |
| Polipropilen · Çin | Polypropylene · China | Kimya ve gübre |
| PTA · Çin | PTA (purified terephthalic acid) · China | Kimya ve gübre |
| Soda külü · Çin | Soda ash · China | Kimya ve gübre |
| Kereste · Malezya (seraya / meranti) | Sawnwood · Malaysia (seraya / meranti) | Diğer hammadde |
| Kontrplak · Tokyo spot | Plywood · Tokyo spot | Diğer hammadde |
| Pamuk · Uluslararası | Cotton · International | Diğer hammadde |

### Emtia Ağı

Emtia'nın alt başlığıdır. Hangi emtia hangi sektörlerle bağlı, tek ağ görüntüsünde. Bağlar şirketlerin girdi sepetinden gelir; sepet ağırlıklarının çoğu varsayımdır ([Yöntem §1 ve Sınırlar](#yöntem)).

![Emtia Ağı: emtialar üst katta, şirketler alt katta; kesikli çizgiler vekil eşleşme](screenshots/09-emtia-agi.png)

### Harita

Dünya haberleri, şirketlerin emtia maruziyetine bağlanır. Bir haber hangi emtiayı etkiliyorsa, o emtiayı girdi sepetinde taşıyan şirketler haritada yan yana görünür. Oklar haberin anlattığı ilişkinin yönüdür; etki iddiası değildir. Sayfada zaman düğmeleri (Son 24 saat, 7 gün, 30 gün), "Açıklamayı yapan" süzgeci, haber listesi ve kriz dosyaları bulunur. Görüntüde haber başlıkları yerine "—" görünür; harita, haber kümeleri, oklar, geçiş noktaları ve kriz dosyaları durur.

![Harita sayfası: haber kümeleri, ilişki okları, geçiş noktaları ve kriz dosyaları](screenshots/02-harita.png)

### Tedarik Zinciri

Harita'nın alt başlığıdır. Seçili şirketin girdi emtialarının Türkiye'ye hangi menşe ülkelerden, hangi güzergâh ve geçiş noktalarından geldiği. Sayfa sekiz adımlı bir anlatımdır: 1 Şirket, 2 Girdiler, 3 Yerli ve ülke, 4 Yollar, 5 Geçişler, 6 Bir ülke, 7 Bir nokta, 8 Geçiş payı; görüntüler (örnek: Ereğli) beşinci adımı, "Yolda hangi geçişler var, günde kaç gemi geçiyor?" sorusunu gösterir. Sayfa Türkiye geneli ithalatı gösterir; şirketin kendi tedarikçisi anlamına gelmez ve payların çoğu "yaklaşık" etiketi taşır. Kutu boyları girdinin sepet payı ile ithalat içi paya göredir; sepet ağırlıklarının çoğu varsayımdır ([Yöntem §1](#yöntem)). [Kaynak: ürünün Tedarik Zinciri sayfasındaki açıklama metni]

![Tedarik Zinciri sayfası, Ereğli, 5. adım Geçişler: güzergâh haritası, katmanlı ağ ve şirketin kendi beyanı paneli](screenshots/10-tedarik-zinciri.png)

**Güzergâh haritası.** Şematik bir deniz haritası: menşe ülkelerden Türkiye'ye giden çizgiler (demir cevheri ve bitümlü kömür ayrı renkte) ve aradaki geçiş noktaları (Cebelitarık, Süveyş, Bab el-Mandeb, Türk Boğazları). Çizgiler şematiktir, gerçek seyir değildir; yerli üretim ve kara ya da boru hattı ithalatı haritada çizilmez, ağda ayrı kol olarak durur. Haritanın altındaki tabloda geçiş noktalarının günlük geçiş sayıları (IMF PortWatch medyanı) yer alır; depodaki karede bu sayılar "—" görünür.

![Güzergâh haritası ve geçiş noktaları tablosu; geçiş sayıları "—"](screenshots/10-tedarik-guzergah.png)

**Katmanlı ağ.** Akış şirket, girdi, yerli kol ile menşe ülke ve geçiş noktası sütunlarında verilir; bir bağın ya da düğümün üzerine gelince ne taşıdığı yazar ve haritada o yol vurgulanır.

![Katmanlı ağ: şirket, girdi, yerli kol ve menşe ülke, geçiş noktası sütunları](screenshots/10-tedarik-ag.png)

**Şirketin kendi beyanı.** Sayfanın altındaki bu panel, şirketin kendi belgesindeki tedarikçi ülke ve kendine yetme beyanını Türkiye geneli verisinden ayrı gösterir; iki taraf birbirinden hesaplanmaz. Depodaki karede bu panelin alanları "—" görünür.

### KAP

KAP bildirimlerinin zaman aralığına (1H, 1A, 3A, 6A, 1Y, tümü), şirkete, sektöre ve bildirim tipine göre süzülebildiği liste sayfası ("Hangi şirket ne bildirdi, ne zaman?"). Maskeli kipte bildirim gösterilmez; liste boştur ve bu yüzden depoda KAP için görüntü yoktur. Demo kipinde bu sayfa menüde listelenmez. [Kaynak: ürünün KAP sayfası, canlı, 17.11.2026]

### Kaynak

Veri menüsünün ilk sayfasıdır: "Veriler nereden geliyor?" Her serinin kurumu, lisansı ve son gözlemi bu sayfadadır; bir satıra tıklayınca serinin künyesi açılır (kod, atıf, bağlantı ve veri zinciri). Bölümler: Özet, Emtia ve makro seriler, Döviz kurları, Çıktı proxy'leri, Şirket verisi, Harita katmanları, Eşleşme gerekçeleri ve Karar geçmişi. Liste Excel'e aktarılabilir. Sayfa hiçbir hesap yapmaz, yalnız kayıtlı bilgiyi gösterir. Menüdeki adı "Kaynak"tır. Sayfanın görüntüsü bu depoya alınmadı. Kaynaklar sayfasında kaynak adları ve atıflar listelenir. [Kaynak: ürünün Kaynak sayfası, canlı, 17.11.2026]

### Veri kalitesi

Hangi şirketin verisi hesaba yetiyor? Her şirketin verisi taramadan geçer: kalanlar hesaba girer, uyarılılar notla girer, elenenler girmez, yalnız çıktısı izlenenler ayrı işaretlenir; her şirketin girdi kapsamı yanında yazar. Sayfa Özet (kalan, uyarılı, elenen sayaçları), Şirketler (sektöre ve duruma göre süzülen tablo), Veri tazeliği ve gecikmeler, Doğrulama ve Ajan çalışmaları bölümlerinden oluşur. [Kaynak: ürünün Veri kalitesi sayfası, canlı, 17.11.2026]

![Veri kalitesi sayfası: şirket başına veri durumu ve girdi kapsamı](screenshots/12-veri-kalitesi.png)

### Terimler

Ekrandaki sözcüklerin kısa tanımları; sayfada terim arama kutusu ve terim listesi bulunur, bir terime tıklayınca hesabı ve okuma notu açılır. [Kaynak: ürünün Terimler sayfası, canlı, 17.11.2026]

![Terimler sayfası: terim sözlüğü ve kısa tanımlar](screenshots/12-terimler.png)

### Ayarlar

Dil (Türkçe ya da English; seçilince sayfa yeniden yüklenir ve tercih cihazda saklanır), sayfa ölçeği, hareketi azaltma, emtia şeridinde yalnız favoriler, menü ve başlangıç sayfası (girişte açılacak sayfa ve menüde görünen başlıklar), grafik ışıklandırması, parola değiştirme ve tercihleri sıfırlama. İngilizce arayüzün çevirisi sürmektedir. [Kaynak: ürünün Ayarlar sayfası, 17.11.2026]

### Tarama

Sol menüde yer almaz; genel arama kutusunda sayfa olarak bulunur. Bütün şirketler tek tabloda: 90 günlük girdi ve çıktı değişimi, fiyat–maliyet farkı (90 günlük değişim, 5 yıllık tarihsel konum, hareket büyüklüğü) ve veri durumu ("şirkete özgü ölçüm" ya da "paylaşımlı proxy"); özdeş seri paylaşan şirketler gruplanır. Sektör süzgeci, "Yalnız yeni şirketler" düğmesi, liste süzme kutusu ve "Bu süzgeci kaydet" düğmesi vardır; üstte girdi ve çıktı 90 günlük ortalaması ile kalan, uyarılı ve elenen sayaçları durur. Görüntüde değerler "—" görünür. [Kaynak: ürünün Tarama sayfası, canlı, 17.11.2026]

![Tarama sayfası: şirketler için girdi, çıktı ve fiyat–maliyet farkı sütunları ve veri durumu; değerler "—"](screenshots/19-tarama.png)

### Ana sayfa

Ürünün herkese açık ana sayfası: ne ölçtüğünü, sayfaların kısa turunu ve sık sorulan soruları anlatır. Görüntü tam sayfa boyundadır (yaklaşık 11 MB), bu yüzden satır içi gösterilmez: [screenshots/13-anasayfa.png](screenshots/13-anasayfa.png).

### Giriş

Hesaplı kullanıcıların giriş sayfası; görüntüde form boştur.

![Giriş sayfası: e-posta ve parola alanları boş](screenshots/14-giris.png)

### Kaydol

Hesap başvuru sayfası: başvuru yönetici onayına gider; sayfa hesapla nelerin açıldığını ve nelerin açılmadığını yazar. Görüntüde form boştur.

![Kaydol sayfası: başvuru formu boş; hesapla açılanlar ve açılmayanlar](screenshots/15-kaydol.png)

### Hakkımızda

Ürünün ne olduğu, ne yaptığı, ne yapmadığı ve veriye nasıl yaklaştığı dört kutuda.

![Hakkımızda sayfası: Vantage Castle nedir, ne yapar, ne yapmaz, veriye nasıl yaklaşır](screenshots/17-hakkimizda.png)

## Emtia Marj Motoru

Projeksiyon sayfasındaki her sayıyı Emtia Marj Motoru hesaplar. Motor, bir şirketin brüt marjının bir sonraki bilançoda emtia hareketleri ve şirketin kendi yapısı ışığında nereye gelebileceğini bilanço açıklanmadan önce hesaplar ve kayda geçirir; gerçekleşen değer gelince kaydın yanına eklenir. Bu bir hesaptır: hisse fiyatı ya da yatırım yönü hakkında bir şey söylemez, hakem değildir ve yatırım tavsiyesi değildir. [Kaynak: ürünün Projeksiyon sayfası ve ekibin yöntem belgesi; belge bu depoda yer almaz]

### Ne hesaplar, ne hesaplamaz

Motor tek bir soruyu yanıtlar: "Bilinen emtia hareketi, diğer her şey sabit kalırsa, şirketin brüt marjını kaç puan oynatır?" Sayfanın üstündeki uyarı bunu söyler: "Bu bir hesaptır, yön iddiası değildir." Hacim, şirketin izlenmeyen maliyet kalemleri ve fiyat geçişkenliği sabit kabul edilir. Motor hisse fiyatını ya da bir işlem hükmünü hiçbir yerde üretmez. [Kaynak: ürünün Projeksiyon sayfası, 17.11.2026]

### Üç girdi

Motor üç şeye bakar:

1. **Şirketin finansalları.** KAP'ta yayımlanan üç aylık hasılat, satışların maliyeti ve brüt kâr; stok devir süresi; enflasyon muhasebesinin (TMS 29) etkisi.
2. **Şirketin emtiaları.** Şirketin girdi sepetindeki emtiaların resmî seri fiyatları. Fiyatlar stok devir süresi kadar geriden okunur: bugünkü fiyat hareketi bilançoya ancak stok eridikçe yansır.
3. **Girdi–çıktı.** Girdi sepetinin fiyatı ile şirketin sattığı ürüne en yakın çıktı fiyat serisi yan yana konur; ikisi arasındaki fark hesapta çıktı etkisini oluşturur.

[Kaynak: ürünün Projeksiyon sayfası, "Sebepler: sayı akışı" bölümü, 17.11.2026; ekibin yöntem belgesi]

### İki yöntem, tek ekran

Projeksiyon·Emtia sayfası her şirket için iki yöntemin sonucunu ayrı bloklarda gösterir: **"Emtia fiyatından"** ve **"Şirket finansallarından"** (ekranda "ön kayıtlı yöntem" notuyla). Ekranda iki blok ayrı ayrı görünür. Ekibin yöntem belgesi, hangisinin ana sayı olarak gösterileceğini sektör başına önceden yazılmış bir seçim kuralına bağlar. Bu seçim kuralı 2026'nın dördüncü çeyreğinden itibaren planlıdır ve ekranda henüz görünmez. [Kaynak: ürünün Projeksiyon·Emtia ve Gerçekleşen sayfaları, 17.11.2026; ekibin yöntem belgesi]

### "Emtia fiyatından" yöntemi

Önceki marjdan hesap marjına giden yolu adım adım gösterir; ekranın "Sebepler" bölümündeki sıra şöyledir:

- **Girdi tarafı.** Girdi sepetinin fiyat değişimi → stok gecikmesi (emtia değişiminin penceresini kaydırır; ayrı bir marj terimi değildir) → maliyet katsayısı (girdi sepeti değişiminin maliyete ne kadar yansıdığı) → maliyete yansıyan değişim → çıktı yansıtma oranı (maliyet değişiminin satış fiyatına ne kadar yansıdığı) → satış gelirine yansıyan değişim → brüt marja girdi etkisi.
- **Çıktı tarafı.** Çıktı sepeti (çıktı fiyat serisi, çoğu şirkette TÜİK Yİ-ÜFE'nin ilgili alt kalemi) ile girdi sepeti arasındaki fark → brüt marja çıktı etkisi.
- **Sonuç.** Önceki çeyreğin marjı + girdi etkisi + çıktı etkisi = hesap marjı. Sayfanın "Marj akışı" şeması aynı sırayı çizer.

Bu yöntemin tabanı önceki çeyrektir. [Kaynak: ürünün Projeksiyon·Emtia sayfası, 17.11.2026; ekibin yöntem belgesi]

### "Şirket finansallarından" yöntemi

Bu yöntem şirketin kendi geçmiş finansal davranışından yola çıkar:

- **Taban.** Aynı çeyreğin geçen yıl değeri; böylece mevsimsellik hesaba karışmaz.
- **Reel girdi şoku.** Girdi sepetinin fiyat değişimi, aynı pencerede tüketici fiyat endeksindeki değişimden arındırılır ve stok gecikmesi kadar geriden okunur.
- **İki katsayı.** Girdi tepkisi (reel şokun maliyete yansıması) ile satış yansıtması (reel maliyet değişiminin reel satışa yansıması) şirketin kendi geçmiş çeyreklerinden kestirilir. Katsayıları kuran geçmiş, ön kayıtta dondurulmuş bir tarihte biter ve ileri kayıtta değişmez.
- **Üç kol.** Alt kol satışa hiç yansıma olmadığını, orta kol şirketin geçmiş davranışını, üst kol şirketin geçmişteki yüksek yansıma gözlemlerini varsayar. Ekranda "Senaryo hesabı (orta)" ve "Bant (alt – üst)" satırları olarak görünür; bant üç kolun en küçüğü ile en büyüğüdür. Ekibin yöntem belgesi bu üç sonuca "senaryo kolları" der; ekrandaki adlar "Senaryo hesabı (orta)" ve "Bant (alt – üst)" olduğu için bu belge ekrandaki adı kullanır.
- **Aralık dışı.** Hesaplanan girdi şoku katsayıyı kuran geçmiş aralığın dışında kalırsa değer kırpılmaz ve değiştirilmez; ekran "aralık dışı" yazar ve yalnız bandı gösterir.
- **Ölçülemedi.** Veri yetmiyorsa motor sayı uydurmaz; nedenini yazar: "kapsam düşük", "geçmiş yetersiz", "taban doğrulanmadı", "girdi tepkisi ölçülemiyor", "benzer durum yok" ya da "girdi serisi yok". Bu şirket-çeyrekler listeden çıkarılmaz, ölçülemedi olarak sayılır.
- **Çıktı kontrolü.** Finansaldan çıkan satış değişimi ile piyasadaki çıktı fiyat değişimi karşılaştırılır ve "piyasayla aynı", "piyasanın önünde" ya da "piyasanın gerisinde" yazılır. Bu kontrol hesaba girmez; satış tutarı hacim ve ürün karışımını da içerdiği için "yaklaşık", seri şirketi dolaylı temsil ediyorsa "vekil" etiketi taşır.

İç değerlendirmede ölçüt yöndür; ekranda doğru ya da yanlış yön sayımı, oran ya da başarı cümlesi yoktur. [Kaynak: ekibin ön kayıtlı yöntem belgesi; ürünün Projeksiyon·Emtia sayfası, 17.11.2026]

### Ayrıştırma: iç araştırma yöntemi (üründe henüz yok)

Ekibin yöntem belgesi, bilanço açıklandıktan sonra şirketin gerçek brüt marj değişiminin parçalara ayrılmasını anlatır: emtia ve hammadde, satış fiyatı ve ürün karması, hacim, kur, enflasyon muhasebesi (TMS 29), stok etkisi ve diğer giderler. Bu bir iç araştırma yöntemidir; üründe henüz yoktur ve hiçbir ekranda ayrıştırma görünmez. Yöntem belgesi yürütme emri değildir: yürütme ayrı bir istek ve insan kararıyla başlar. Belgeye göre parçalar KAP'taki finansal raporun dipnotlarında açıkça okunabilen büyüklüklerden kurulur; hacim (adet) ise şirketin ara dönem faaliyet raporundan ya da KAP'taki satış adedi açıklamasından alınır ve fiyat bunlardan türetilir, çünkü finansal tablo adet vermez. Her şirketin ara dönem faaliyet raporunda çeyreklik adet verip vermediği doğrulanmamıştır. Okunamayan parça uydurulmaz, "kalan" satırına yazılır. Sıra baştan donmuştur: önce hacim, sonra fiyat, sonra maliyet. Resmî taban ile ayrıştırma tabanı arasındaki fark ayrı "taban farkı" satırı olarak yazılır; kalana karıştırılmaz. Ayrıştırma betimleyicidir: "sapma şundan geldi" hükmü vermez. [Kaynak: ekibin yöntem belgesi v1.3, §5, §6, §9, §10 ve açık nokta §11.2; belge bu depoda yer almaz]

### Referans marj bugün ekranda; aralık ve yedek kural planlı (ekranda henüz yok)

**Bugün ekranda: referans marj.** Bir şirket-çeyrek için model çıktısı yoksa ekran model çıktısı olmadığını yazar ve referans olarak şirketin KAP'ta en son açıklanmış üç aylık gerçekleşen brüt marjını gösterir (Projeksiyon·Gerçekleşen). Bu referans hiçbir yöntemin sayısı sayılmaz ve hiçbir ölçüme girmez. [Kaynak: ürünün Projeksiyon·Gerçekleşen sayfası, 17.11.2026; ekibin yöntem belgesi]

**Planlı, ekranda henüz yok: aralık.** Ekibin yöntem belgesi ve aralık eki, 2026'nın dördüncü çeyreğinden itibaren her şirket ve her yöntem için ana sayının iki yanına tek bir yarı genişlik q eklenmesini planlar: [ana sayı − q, ana sayı + q]. q, o yöntemin kendi geçmiş mutlak hatalarından hesaplanacaktır (bölünmüş konformal yöntem; kapsama %80 (tasarım tercihi)); şirkete ya da sektöre özgü elle genişlik, kırpma ve yöntemler arasında hata havuzlama yoktur. Geçmişi az olan yöntemde aralığın "örnek n=…: kaba" etiketiyle gelmesi planlanır. Kapsama güvencesi hataların aynı dağılımdan geldiği varsayımına dayanır; bu varsayım ölçülmemiştir. Bugünkü ekranda bu aralık, q ve bu etiket yoktur: yalnız "Bant (alt – üst)" satırı görünür; bu bant yukarıda anlatıldığı gibi üç kolun en küçüğü ile en büyüğüdür, geçmiş hatalardan hesaplanan bir aralık değildir. [Kaynak: ekibin yöntem belgesi ve aralık eki v1.0, yürürlük 2026 Ç4; formül: Angelopoulos ve Bates, arXiv 2107.07511; ürünün Projeksiyon·Emtia sayfası, 17.11.2026]

**Planlı, ekranda henüz yok: yedek kural.** Belgeye göre seçim kuralının seçtiği yöntem bir şirket-çeyrek için sonuç üretmediyse: (1) o şirket için "şirket finansallarından" sonucu varsa ürün onu "yedek" etiketiyle gösterecek ve yedek sayı seçilen yöntemin sayısı diye adlandırılmayacaktır; (2) o da yoksa model çıktısı olmadığı yazılır ve referans marj gösterilir (yukarıdaki, bugün ekranda olan davranış). Bugünkü ekranda "yedek" etiketi yoktur. [Kaynak: ekibin yöntem belgesi v1.3, yürürlük 2026 Ç4; ürünün Projeksiyon sayfaları, 17.11.2026]

**Dürüstlük kaydı.** Aralık ve yedek kural, ilk ileri kayıt ölçümünün sonuçları görüldükten sonra yazıldı; bu yüzden o ölçüm için geriye dönük bir kanıt değildir. İlk gerçek sınav 2026'nın dördüncü çeyreğidir ve orada kapsama yalnız betimleyici olacaktır: "n=…, k=…" yazılır, "tuttu / tutmadı" hükmü verilmez. [Kaynak: ekibin yöntem belgesi]

### Henüz hesapta olmayanlar

Projeksiyon'un **Makro** görünümü (kur ve enflasyonun etkisi) ve **Operasyonel** görünümü (hacim, kapasite ve hedge etkisi) henüz hesapta değildir; ekran bunu açıkça "henüz hesapta değil" diye yazar ve bu etkiler motorun hiçbir sayısına girmez. [Kaynak: ürünün Projeksiyon·Makro ve Operasyonel sayfaları, 17.11.2026]

### Sınırlar

- Sepet ağırlıklarının çoğu varsayımdır; izlenen sepet maliyetin tamamı değildir.
- Satış değişimi tutar tepkisidir: hacim ve ürün karışımı ayrı gösterilmez.
- Bazı şirketlerde kapsam, geçmiş ya da taban yetmez; motor orada "ölçülemedi" yazar.
- Enflasyon muhasebesi (TMS 29) ve işlevsel parası dolar ya da avro olan şirketlerin TL sütunu hesabı etkileyen ayrı özel durumlardır; yöntem belgesi bunları açıkça ayırır.
- Yöntem belgesi ve ön kayıtlar sonuç görülmeden donar; değişiklik yeni belge ve yeni sürümdür, eski sürüm değişmez.

## Yöntem

Dört büyüklük yan yana durur: **girdi endeksi** (şirketin girdi emtia sepetinin ağırlıklı fiyatı, 01.01.2015 = 100, stok devir süresi kadar geriden okunur), **çıktı endeksi** (çoğu şirkette TÜİK Yurt İçi Üretici Fiyat Endeksi'nin ilgili alt kalemi), **fiyat–maliyet farkı** (çıktı endeksinin girdi endeksine oranı) ve **gerçekleşen brüt marj** (şirketin KAP'ta yayımladığı üç aylık finansal rapordan). Aralarına "bu yüzden" konmaz; ikisi ayrı ayrı gözlenen serilerdir. Hesaplanan marj bilanço öncesi kayda geçirilir, gerçekleşen değer gelince yanına eklenir; ekranda bugün "Bant (alt – üst)" görünür; geçmiş hatalardan hesaplanan bir aralık ise 2026'nın dördüncü çeyreğinden itibaren planlıdır ve ekranda henüz yoktur ([Emtia Marj Motoru](#emtia-marj-motoru)). [Kaynak: ürünün hesap kuralı; tam metin aşağıda]

<details>
<summary><b>Ayrıntılar: Yöntem (tam metin)</b></summary>

Bu bölüm Vantage Castle'ın dört temel büyüklüğünü anlatır. Hepsi ölçüm ve hesaptır; hiçbiri bir hisse hakkında görüş değildir ve yatırım tavsiyesi değildir. Sayıların yanında kaynağı ya da ölçümün türü yazılıdır. Ölçüm kayıtları bu depoda yer almaz; yöntem bu bölümde kendi başına anlatılır.

### 1. Girdi endeksi

Şirketin girdi emtia sepetinin ağırlıklı ortalama fiyatıdır; 01.01.2015 = 100 tabanıyla kurulur. Ağırlıklar çoğu şirkette sıra varsayımıdır: birinci girdi %50, ikinci %30, üçüncü %20. Ölçülmüş oranı olan az sayıda şirkette varsayımın yerine ölçülen oran kullanılır. Fiyat serisi bulunamayan bileşen sepetten düşer, kalan ağırlıklar yeniden ölçeklenir ve düşen pay "girdi kapsamı" olarak satırda görünür. [Kaynak: ürünün hesap kuralı; ağırlıklar tasarım tercihidir]

Bir emtia bugün pahalansa da şirket bir süre eski stokla üretir. Girdi fiyatları bu yüzden şirketin stok devir süresi kadar geriye alınır; süre son dört ile sekiz geçerli çeyreğin ortalamasıdır ve 0–365 gün arasında tutulur. Çıktı fiyatı geriye alınmaz. [Kaynak: ürünün hesap kuralı]

### 2. Çıktı endeksi

Çoğu şirkette TÜİK Yurt İçi Üretici Fiyat Endeksi'nin ilgili alt kalemidir; aynı 01.01.2015 = 100 tabanıyla kurulur. [Kaynak: TÜİK Yurt İçi Üretici Fiyat Endeksi]

### 3. Fiyat–maliyet farkı (makas)

Çıktı endeksinin girdi endeksine oranıdır. Ölçülen şey fiyattır; kâr, satış hacmi ya da verimlilik değildir. Güncel değer, şirketin kendi son 5 yıllık geçmişindeki yüzdelik dilimiyle birlikte gösterilir; tek başına bir sayı olarak sunulmaz. Değer, sepetteki her bileşenin bilindiği en son ortak tarihe göre okunur. [Kaynak: ürünün hesap kuralı]

### 4. Gerçekleşen brüt marj

(Hasılat − satışların maliyeti) ÷ hasılat; şirketin KAP'ta yayımladığı finansal raporun üç aylık cari sütunundan alınır, kümülatif farktan türetilmez. Ürün gerçekleşen marjı fiyat–maliyet farkının yanında gösterir ve ikisi arasına "bu yüzden" koymaz: ikisi ayrı ayrı gözlenen serilerdir. [Kaynak: şirketlerin KAP'ta yayımladığı finansal raporlar]

### 5. Projeksiyon: hesap, hüküm değil

Projeksiyon sayfası emtia hareketinin bilanço marjına aritmetik etkisini "diğer her şey sabit kalırsa" varsayımıyla hesaplar; hacim, izlenmeyen maliyet kalemleri ve fiyat geçişkenliği sabit kabul edilir. Emtia girdi etkisi, girdi sepetinin belirli bir penceredeki hareketinden alınır ve sepet §1'deki gibi stok devir süresi kadar geriden okunur; ürünün ayarlarında pencere 30, 90 ve 180 gün olarak tanımlıdır, [marj akışı şemasındaki](diagrams/marj-akisi.png) örnek 90 günlük penceredir. [Kaynak: ürünün Projeksiyon sayfası, 17.11.2026] Şirketler fiyatlama, stok, hedge ve ürün karması yoluyla etkiyi karşılayabilir. Geçmiş ölçümlerde fiyat–maliyet farkının yönü ile gerçekleşen brüt marjın yönü arasında yazı turadan ayırt edilebilen bir uyum bulunamadı ([Dürüst bulgular](#dürüst-bulgular)). Bu yüzden ürün hisse fiyatı ve yatırım yönü bildirmez; girdi maliyetinden hesaplanan marjı, bandını ve gerçekleşen marjla farkını kayıt olarak gösterir. Bu bir hesaptır, hakem değildir ve yatırım tavsiyesi değildir; gerçekleşen değer sonradan yanına eklenir. Hesabın nasıl kurulduğu [Emtia Marj Motoru](#emtia-marj-motoru) bölümünde anlatılır.

### Sınırlar

- Sepet ağırlıklarının çoğu varsayımdır; ölçülmüş oran yalnız az sayıda şirkette vardır.
- İzlenen sepet maliyetin tamamı değildir; işçilik ve amortisman sepette yoktur.
- Aynı girdi sepetini ve aynı çıktı endeksini paylaşan şirketlerin fiyat–maliyet farkı sayısal olarak aynıdır; ürün bunu "özdeş seri" diye işaretler ve aralarında fark iddia etmez.
- İleri kayıtla ölçüm henüz çok kısa bir geçmişe dayanır; ortak bir çeyrek şoku bütün şirketleri aynı yönde etkilemiş olabilir.

</details>

## Dürüst bulgular

Vantage Castle'ın en önemli tasarım kararı, ne söylemediğidir. Emtia fiyatından marj ya da hisse fiyat serisi değişimi çıkarılıp çıkarılamayacağını deneyen altı ölçümün hiçbiri anlamlı bir ilişki bulmadı. Örneğin fiyat–maliyet farkının yönü ile gerçekleşen brüt marjın yönü aynı dönemde yazı turadan ayırt edilemedi. Ürün bu yüzden görüş bildirmez, ölçtüğünü yan yana sunar. İlk ileri kayıt ölçümü hakem değildir. [Kaynak: ürünün iç ölçümleri; tam metin aşağıda, sayılar bu depoda yer almaz]

<details>
<summary><b>Ayrıntılar: Dürüst bulgular (tam metin)</b></summary>

Vantage Castle'ın en önemli tasarım kararı, ne söylemediğidir. Aşağıdaki ölçümler emtia fiyatından marj ya da hisse fiyat serisi değişimi çıkarılıp çıkarılamayacağını denedi; hiçbiri anlamlı bir ilişki bulmadı. Ürün bu yüzden görüş bildirmez, ölçtüğünü yan yana sunar.

Hisse fiyatı kullanan ölçümler emtia, marj ve hisse fiyat serileri üzerinde yapılmış iç çalışmadır. "İlişki yok" burada "bu veriyle, bu yöntemle bulunamadı" demektir; ilişkinin olmadığının kanıtı değildir.

### Denenip bırakılan yollar (altı ölçüm)

Tablodaki "Veri" sütunu ölçümün hangi veri türüne dayandığını gösterir. Bunlar ürünün kendi iç ölçümleridir; ayrıntılı kayıtları ve sayıları bu depoda yer almaz.

| # | Ölçüm | Sonuç | Veri |
|---|---|---|---|
| 1 | Regresyon hattı: şirket bazında ve tek modelde, emtia değişiminden marj ve hisse fiyat serisi değişimi | Anlamlı güç yok; örnek-dışı dönemde açıklama gücü negatif, yani basit bir ortalamadan bile kötü | Emtia, marj ve hisse fiyat serileri |
| 2 | Fiyat–maliyet farkının yönü ile gerçekleşen brüt marjın yönü aynı dönemde uyuşuyor mu? | Uyum yazı turadan ayırt edilemedi; hiçbir gecikme ya da hizalama düzeltmesi eşiği geçmedi | Fiyat–maliyet farkı ve KAP marjı, geçmiş yıllar |
| 3 | Sektör-nötr ters sıralı iki grup farkı: fark ölçüsü en olumlu şirketlerden oluşan bir grup ile en olumsuz şirketlerden oluşan ters sıralı bir grubun fiyat serisi değişimi farkı | Fark gürültüden ayırt edilemedi | Fiyat–maliyet farkı ve hisse fiyat serisi |
| 4 | Fiyatlanma ölçümü: fark belirgin değiştiğinde hisse fiyat serisi sektör emsallerinden nasıl ayrıştı? | İlişki bulunamadı | Fiyat–maliyet farkı ve hisse fiyat serisi |
| 5 | Stok devir hızı: stok devir süresi emtia fiyatıyla birlikte değişiyor mu? | İlişki bulunamadı; sabit stok devir varsayımı bu yüzden korunur | Emtia fiyatı ve KAP finansal raporları |
| 6 | KAP olay çalışması: bildirimden sonra hisse fiyat serisi sektöründen normalden fazla ayrışıyor mu? | Yalnız ayrışmanın büyüklüğüne bakar, yönüne bakmaz | KAP bildirimleri ve hisse fiyat serisi |

Ayrıca iki yol bırakıldı: fiyat–maliyet farkının büyük değiştiği dönemleri sonraki marjla eşleştiren "epizot tablosu" kaldırıldı (kanıtlanmamış bir ilişkiyi kanıtlanmış gibi gösterirdi) ve finansal tabloları tüketici fiyatlarıyla ortak tabana çevirme denemesi başarısız oldu, tablolara uygulanmadı.

### Haber yönü etiketi ölçümü (ürün sayfalarında yer almaz)

Haberlere yön etiketi verilip etiketin ardından fiyat serisinin aynı yönde değişip değişmediğine bakıldı; plan etiketleme başlamadan yazılıp dondurulmuştu. Sonuç: etiket yönü ile sonraki fiyat serisi yönü kısa, orta ve uzun işlem günü ufuklarının üçünde de yazı turadan ayırt edilemedi; üç ölçüm de önceden yazılmış anlamlılık eşiğini geçmedi. Etiketleyiciler arası uyum orta düzeydeydi; bu yüzden sonuç "kesin ilişki yok" değil "zayıf yokluk bulgusu" olarak kaydedildi. Bu ölçüm ürüne girmez; etiketler hiçbir ekranda gösterilmez. [Ölçüm: ekibin iç ölçümü, 10.10.2026; haber etiketleri ve hisse fiyat serisi]

### İleri kayıt ölçümü (hakem değil)

Hesaplar bilanço açıklanmadan önce yapılır ve kayda geçirilir; gerçekleşen değer gelince yanına eklenir. İlk ileri kayıt ölçümü 2026'nın üçüncü çeyreği için yapıldı. Bu ölçüm hakem değildir: ondan yöntem seçimi ya da geçti/kaldı hükmü çıkarılmaz. Ölçümün sayıları bu depoda yer almaz; ürünün ekranlarında kayıt ile gerçekleşen yan yana görünür ([Emtia Marj Motoru](#emtia-marj-motoru)).

### Bu bulgular ürünü nasıl şekillendirdi

Ürün hisse fiyatı ve yatırım yönü bildirmez, işlem talimatı vermez, "makas daraldı, marj baskısı var" gibi bir durum ya da yön iddiası kurmaz; girdi endeksi, çıktı endeksi, fiyat–maliyet farkı ve gerçekleşen brüt marjı aralarında nedensellik ima etmeden yan yana koyar. Girdi maliyetinden hesaplanan marjı, bandını ve gerçekleşen marjla farkını kayıt olarak gösterir; bu bir hesaptır, hakem değildir ve yatırım tavsiyesi değildir. Bu bir üslup tercihi değil, yukarıdaki ölçümlerin sonucudur. Sistem ölçtüğünü yan yana sunar, yorumu okuyucuya bırakır.

</details>

## Mimari

![Mimari şema](diagrams/mimari.png)

Şemada planlı özellikler "PLANLI (2026 Ç4)" etiketiyle işaretlidir.

Altı basamak: kaynaklardan gelen seriler → kayıt ve kontrol katmanı (birim ve tarih kontrolü, kaynak kaydı) → ölçüm katmanı (girdi endeksi, çıktı endeksi, fiyat–maliyet farkı, gerçekleşen brüt marj) → Emtia Marj Motoru (iki yöntem ve bant; aralık ve yedek kural planlı, ekranda henüz yok) → sunum sayfaları (kaynak ve lisanslar Kaynak sayfasındadır) → yapay zekâ ajanlarından kurulu bir ekiple geliştirme.

<details>
<summary><b>Ayrıntılar: Mimari (tam metin)</b></summary>

1. **Veri kaynakları.** Kaynağı belirtilen seriler: emtia fiyatları, kurlar, faiz ve enflasyon serileri, şirket finansalları. Bu depodaki görsellerde yer alan verilerin kaynakları [Lisans ve atıflar](#lisans-ve-atıflar) bölümünde yazılıdır; ürünün Kaynak sayfası her serinin kurumunu, lisansını ve son gözlemini ayrıca gösterir.
2. **Kayıt ve kontrol katmanı.** Her satır birim ve tarih kontrolünden geçer ve hangi kaynaktan geldiği kaydedilir.
3. **Ölçüm katmanı.** Her şirket için girdi endeksi (girdi sepetindeki emtiaların ağırlıklı fiyatı), çıktı endeksi (satış fiyatına yakın seri) ve ikisinin oranı olan fiyat–maliyet farkı hesaplanır; gerçekleşen brüt marj yanında durur.
4. **Emtia Marj Motoru.** Ölçüm katmanındaki serileri ve şirketin finansallarını Projeksiyon hesabına çevirir: iki yöntem ve bant. Geçmiş hatalardan hesaplanan aralık ile yedek kural 2026'nın dördüncü çeyreğinden itibaren planlıdır ve ekranda henüz yoktur. Yöntemler bilanço açıklanmadan önce yazılıp kayda geçirilir; kayıtlı hesap sonradan değişmez, gerçekleşen değer yanına eklenir ([Emtia Marj Motoru](#emtia-marj-motoru)).
5. **Sunum.** Panom, Değişimler, Bülten, Şirketler, Projeksiyon, Sektörler, Emtia, Emtia Ağı, Harita, Tedarik Zinciri, KAP, Kaynak, Veri kalitesi, Terimler, Ayarlar ve Tarama sayfaları yalnız ölçüm katmanından ve motorun kaydından okur; kaynak ve lisanslar Veri › Kaynak sayfasında yazılıdır. Yayın kipinde hisse fiyatı, KAP bildirimleri ve bilanço tabloları gösterilmez; maske kipinde ayrıca haber başlıkları, elektrik (EPİAŞ) ve geçiş noktası (PortWatch) değerleri ile hesap bilgileri de gösterilmez. Demo kipinde KAP, Sektörler'in marj sayfası ve Projeksiyon·Gerçekleşen menüde listelenmez. Bu depodaki sayfa görüntüleri maske kipinden alınmıştır. [Kaynak: ürünün menü tanımı, 17.11.2026]
6. **Geliştirme.** Ürün, yapay zekâ ajanlarından kurulu bir ekiple geliştirilir: her iş planla başlar, üretim ayrı, denetim ayrı oturumda yapılır, dışarı giden her adım insandadır. Ayrıntı: [Ekip](#ekip)

</details>

## Ekip

Vantage Castle, yapay zekâ ajanlarından kurulu bir ekiple geliştirildi: her ajan ayrı bir oturumda, tek bir rolle çalışır. Her iş bir planla başlar, üreten kendi işini onaylamaz (ayrı bir denetçi uygulanmış sonuca bakar), dışarı giden her şey insandadır ve son söz insandadır. [Kaynak: çalışma düzeninin kısa özeti; tam metin aşağıda]

<details>
<summary><b>Ayrıntılar: Ekip (tam metin)</b></summary>

Vantage Castle, HBK Software'in ürünüdür. HBK Software, yapay zekâ ajanlarından kurulu bir ekiptir: her ajan ayrı bir oturumda, tek bir rolle çalışır. Şirketin sahibi bir insandır ve son söz onundadır. Bu bölüm ekibin nasıl çalıştığını, neyi yapıp neyi yapamadığını anlatır.

### Roller

Ekipte dokuz rol vardır:

| Rol | Yaptığı iş |
|---|---|
| Özel kalem | İstekleri dağıtır, bitenleri toplar, insana kısa sonuç kâğıdı bırakır |
| Ön yüz | Arayüzü yazar |
| Arka uç | Sunucu, hesap ve test kodunu yazar |
| Tasarımcı | Ekran yönünü ve maketleri çizer |
| Veritabanı uzmanı | Veriyi salt okunur sorgular, sayım ve doğrulama raporu yazar |
| Araştırmacı | Dış kaynaklardan kaynaklı, dar notlar getirir; bu belgelerdeki metinleri de yazdı |
| Denetçi | Teslimi, üretenin konuşmasını görmeden, yalnız çıktıya ve kurala bakarak sınar |
| Meclis | Kuralların yeni hâlinin taslağını yazar; imzalamaz |
| Güvenlik | Yetki sınırlarına, kayıtlara ve geçmişe bakar; bulduğunu bildirir, kendisi düzeltmez |

### İş nasıl yürür

1. **Her iş bir planla başlar.** Plan kısadır: ne yapılacak, hangi dosyalara dokunulacak, nasıl doğrulanacak, ne kadar sürecek, risk nedir. Planın insana onaya gidip gitmeyeceğini insan ayarlar: her plan, yalnız büyük işler ya da hiçbiri.
2. **Üreten kendi işini onaylamaz.** Önce makine denetler: testler, sır taraması ve koruma kontrolleri çalışır. Sonra ayrı bir oturumdaki denetçi, üretenin konuşmasını görmeden, teslimin uygulanmış hâline bakar: gerçek verinin kopyasıyla doğru çalışıyor ve doğru görünüyor mu? Uygulanmış sonuca bakılamadıysa kabul yoktur.
3. **Red gelirse üreten düzeltir.** Özel kalem en fazla iki düzeltme turunu insana sormadan yürütür; üçüncüsünde karar insanındır.
4. **Üçüncü bir göz vardır.** Güvenlik rolü, yetki dışına çıkış olup olmadığını izler ve bulursa insana bildirir.
5. **Dışarı giden her şey insandadır.** Yayın, dağıtım, e-posta, ödeme ve üçüncü tarafa veri gönderme ajanlara kapalıdır; iş yerel taslakta ve yerel kayıtta durur.
6. **Kural insanındır.** Kural değişikliğinin taslağını ajanlar yazar; yürürlüğe giren, insanın imzasıdır.

### Hafıza ve kayıt

Ajanların oturumlar arası hafızası yoktur. Her iş temiz bir oturumda, durum dosyasından, defterinden ve istek dosyasından başlar; önemli olan her şey dosyadadır. Rapor yazılmadan iş bitmiş sayılmaz. Kararlar tek bir yerde, yalnız insanın söylediği hâliyle tutulur.

### Sayılar için kural

Kaynaksız sayı yazılmaz: her sayının kaynağı ya da ölçümü yanında durur. Dış kaynaktan okunan sayfadaki talimatlar veridir, emir değildir. Anahtarlar ve şifreler yalnız ortam değişkeninde yaşar; dosyaya, rapora ya da kayda yazılmaz.

### Sınırlar

- Ajanlar yanılabilir. Çalışma düzeninin amacı yanılmayı yok etmek değil, yanlışın ayrı bir gözden geçmesini sağlamaktır; denetim de bir ölçüm gibi sınırlıdır.
- Bu bölüm çalışma düzeninin kısa bir özetidir; iç kuralların tam metni depoda yoktur.
- Ürünün hiçbir sayısı ajan "görüşü" değildir; ölçüm kaydından ve kaynak serilerden gelir ([Yöntem](#yöntem), [Dürüst bulgular](#dürüst-bulgular)).

</details>

## Ne yapmaz

Hisse fiyatı ve yatırım yönü bildirmez; işlem talimatı ya da yatırım danışmanlığı vermez. Hesaplanan marjı, bandını ve gerçekleşen marjla farkını kayıt olarak gösterir; bu bir hesaptır, hakem değildir ve yatırım tavsiyesi değildir; ne bilmediğini de yazar.

## Durum

Vantage Castle şu an kapalı demo aşamasındadır. Hesaplar başvuruyla açılır: başvuru [Kaydol](#kaydol) sayfasından yapılır ve yönetici onayına gider. Üyelik ve API erişimi ileride planlanmaktadır; kapsamı ve koşulları veri lisanslarına bağlıdır.

## Lisans ve atıflar

Bu depoda kod yoktur; metin ve görseller tüm hakları saklı olarak paylaşılır.

Görsellerde yer alan veriler ilgili kaynak gösterilerek aktarılır:

- Harita karoları (Harita görüntüsü, hero GIF): © OpenMapTiles © OpenStreetMap katkıcıları
- Haber kümeleri (Harita): Kaynak: The GDELT Project (gdeltproject.org)
- Emtia fiyatları (Panom, Şirketler, Emtia, Değişimler, Bülten, Emtia Ağı, Eşleşme matrisi, hero GIF):
  - Jet yakıtı, LPG, bütan, petrokok, fuel oil, hurda çelik, arpa/malt, tuz, mürekkep, karbon siyahı, selüloz/atık kağıt: Kaynak: FRED, Federal Reserve Bank of St. Louis (EIA ve BLS serileri)
  - İthal kömür (Newcastle), uranyum, çinko, kurşun, nikel, kalay, kereste, pirinç, kahve, yün, doğal kauçuk: Kaynak: FRED, Federal Reserve Bank of St. Louis (IMF serileri); bu serilerde FRED'in "Copyrighted: Citation Required" notu vardır
  - Palm yağı, DAP, fosfat kayası, potas, üre: Kaynak: The World Bank, Commodity Price Data (The Pink Sheet)
- Çiğ süt tavsiye fiyatı (Emtia, hero GIF): Kaynak: Ulusal Süt Konseyi
- Kur verisi (TL kaynaklı serilerin dolar karşılığı, Değişimler): Kaynak: TCMB Elektronik Veri Dağıtım Sistemi (EVDS)
- Çıktı fiyat endeksleri (Şirketler, Projeksiyon): Kaynak: TÜİK Yurt İçi Üretici Fiyat Endeksi, TCMB EVDS üzerinden
- Tedarik Zinciri (görüntüler): geçiş noktalarının günlük geçiş sayıları: Kaynak: IMF PortWatch; menşe ülke payları: Kaynak: CEPII BACI; yerli üretim payı: Kaynak: USGS Mineral Commodity Summaries 2026 ve Enerji ve Tabii Kaynak Bakanlığı yayınları; geçiş noktası konumları: Kaynak: EIA kaynaklı temsili merkez noktaları
- Ürünün Harita sayfasındaki kriz dosyası panelinde yer alan uydu görüntüsü (bu depodaki karelerde panel açık değildir): MODIS Land Rapid Response Team, NASA GSFC (02.12.2020). Ürün içindeki görüntüde yazan atıf: "Kamu malı (ABD federal hükümeti çalışması – NASA)". [Kaynak: NASA, görsel ve medya kullanım ilkeleri, <https://www.nasa.gov/nasa-brand-center/images-and-media/>; erişim 16.11.2026: NASA içeriği ABD'de genellikle telif hakkına tabi değildir, kaynak olarak NASA belirtilir]
- Yazı tipi: Martian Mono, SIL Open Font License 1.1
