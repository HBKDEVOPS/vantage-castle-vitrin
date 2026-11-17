# Yöntem

[English](method.md)

Bu sayfa Vantage Castle'ın dört temel büyüklüğünü ve hesabı yapan Emtia Marj Motoru'nu anlatır. Hepsi ölçüm ve hesaptır; hiçbiri bir hisse hakkında görüş değildir ve yatırım tavsiyesi değildir. Sayıların yanında kaynağı ya da ölçümün türü yazılıdır. Ölçüm kayıtları bu depoda yer almaz; yöntem bu sayfada kendi başına anlatılır.

## 1. Girdi endeksi

Şirketin girdi emtia sepetinin ağırlıklı ortalama fiyatıdır; 01.01.2015 = 100 tabanıyla kurulur. Ağırlıklar çoğu şirkette sıra varsayımıdır: birinci girdi %50, ikinci %30, üçüncü %20. Ölçülmüş oranı olan az sayıda şirkette varsayımın yerine ölçülen oran kullanılır. Fiyat serisi bulunamayan bileşen sepetten düşer, kalan ağırlıklar yeniden ölçeklenir ve düşen pay "girdi kapsamı" olarak satırda görünür. [Kaynak: ürünün hesap kuralı; ağırlıklar tasarım tercihidir]

Bir emtia bugün pahalansa da şirket bir süre eski stokla üretir. Girdi fiyatları bu yüzden şirketin stok devir süresi kadar geriye alınır; süre son dört ile sekiz geçerli çeyreğin ortalamasıdır ve 0–365 gün arasında tutulur. Çıktı fiyatı geriye alınmaz. [Kaynak: ürünün hesap kuralı]

## 2. Çıktı endeksi

Çoğu şirkette TÜİK Yurt İçi Üretici Fiyat Endeksi'nin ilgili alt kalemidir; aynı 01.01.2015 = 100 tabanıyla kurulur. [Kaynak: TÜİK Yurt İçi Üretici Fiyat Endeksi]

## 3. Fiyat–maliyet farkı (makas)

Çıktı endeksinin girdi endeksine oranıdır. Ölçülen şey fiyattır; kâr, satış hacmi ya da verimlilik değildir. Güncel değer, şirketin kendi son 5 yıllık geçmişindeki yüzdelik dilimiyle birlikte gösterilir; tek başına bir sayı olarak sunulmaz. Değer, sepetteki her bileşenin bilindiği en son ortak tarihe göre okunur. [Kaynak: ürünün hesap kuralı]

## 4. Gerçekleşen brüt marj

(Hasılat − satışların maliyeti) ÷ hasılat; şirketin KAP'ta yayımladığı finansal raporun üç aylık cari sütunundan alınır, kümülatif farktan türetilmez. Ürün gerçekleşen marjı fiyat–maliyet farkının yanında gösterir ve ikisi arasına "bu yüzden" koymaz: ikisi ayrı ayrı gözlenen serilerdir. [Kaynak: şirketlerin KAP'ta yayımladığı finansal raporlar]

## 5. Projeksiyon: hesap, hüküm değil

Projeksiyon sayfası emtia hareketinin bilanço marjına aritmetik etkisini "diğer her şey sabit kalırsa" varsayımıyla hesaplar; hacim, izlenmeyen maliyet kalemleri ve fiyat geçişkenliği sabit kabul edilir. Emtia girdi etkisi, girdi sepetinin belirli bir penceredeki hareketinden alınır ve sepet §1'deki gibi stok devir süresi kadar geriden okunur; ürünün ayarlarında pencere 30, 90 ve 180 gün olarak tanımlıdır, [marj akışı şemasındaki](../diagrams/marj-akisi.png) örnek 90 günlük penceredir. [Kaynak: ürünün Projeksiyon sayfası, 17.11.2026] Şirketler fiyatlama, stok, hedge ve ürün karması yoluyla etkiyi karşılayabilir. Geçmiş ölçümlerde fiyat–maliyet farkının yönü ile gerçekleşen brüt marjın yönü arasında yazı turadan ayırt edilebilen bir uyum bulunamadı ([Dürüst bulgular](bulgular.md)). Bu yüzden ürün hisse fiyatı ve yatırım yönü bildirmez; girdi maliyetinden hesaplanan marjı, bandını ve gerçekleşen marjla farkını kayıt olarak gösterir. Bu bir hesaptır, hakem değildir ve yatırım tavsiyesi değildir; gerçekleşen değer sonradan yanına eklenir. Hesabın nasıl kurulduğu [Emtia Marj Motoru](yontem.md#emtia-marj-motoru) bölümünde anlatılır.

## Sınırlar

- Sepet ağırlıklarının çoğu varsayımdır; ölçülmüş oran yalnız az sayıda şirkette vardır.
- İzlenen sepet maliyetin tamamı değildir; işçilik ve amortisman sepette yoktur.
- Aynı girdi sepetini ve aynı çıktı endeksini paylaşan şirketlerin fiyat–maliyet farkı sayısal olarak aynıdır; ürün bunu "özdeş seri" diye işaretler ve aralarında fark iddia etmez.
- İleri kayıtla ölçüm henüz çok kısa bir geçmişe dayanır; ortak bir çeyrek şoku bütün şirketleri aynı yönde etkilemiş olabilir.
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
