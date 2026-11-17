# Yöntem

[English](method.md)

Bu sayfa Vantage Castle'ın dört temel büyüklüğünü ve ölçüm kayıtlarını anlatır. Hepsi ölçüm ve hesaptır; hiçbiri bir hisse hakkında görüş ya da öneri değildir. Sayıların yanında kaynağı ya da ölçümün türü yazılıdır. Ölçüm kayıtları bu depoda yer almaz; yöntem bu sayfada kendi başına anlatılır.

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

Projeksiyon sayfası emtia hareketinin bilanço marjına aritmetik etkisini "diğer her şey sabit kalırsa" varsayımıyla hesaplar; hacim, izlenmeyen maliyet kalemleri ve fiyat geçişkenliği sabit kabul edilir. Emtia girdi etkisi, girdi sepetinin belirli bir penceredeki hareketinden alınır ve sepet §1'deki gibi stok devir süresi kadar geriden okunur; ürünün ayarlarında pencere 30, 90 ve 180 gün olarak tanımlıdır, [marj akışı şemasındaki](../sema/marj-akisi.png) örnek 90 günlük penceredir. [Kaynak: ürünün hesap kuralı] Şirketler fiyatlama, stok, hedge ve ürün karması yoluyla etkiyi karşılayabilir. Ölçülen veride fiyat–maliyet farkının yönü ile gerçekleşen brüt marjın yönü aynı dönemde %49,0 uyuşmuştur (n=1492, 2015–2022); bu oran yazı turadan ayırt edilemez ([bulgular](bulgular.md)). Bu yüzden ürün hisse fiyatı ve yatırım yönü bildirmez; girdi maliyetinden hesaplanan marjı, aralığı ve gerçekleşen marjla farkını kayıt olarak gösterir. Bu bir hesaptır, hakem ya da öneri değildir; gerçekleşen değer sonradan yanına eklenir. [Kaynak: bu sayfadaki §4 ve §6; yön uyumu ölçümü [bulgular](bulgular.md) sayfasında]

## 6. Ölçüm kaydı: FM-1 ve Alfa

Hesabın geçmişte ne kadar tuttuğu "ileri kayıtla" ölçülür: hesap bilanço açıklanmadan önce yapılır ve kayda geçirilir; gerçekleşen değer gelince yanına eklenir. [Kaynak: ürünün ölçüm usulü] Bu depo ölçüm kayıtlarını içermez; okuyucunun bu depodan doğrulayabileceği, bu sayfadaki hesap kuralları ve şirketlerin KAP'ta açıkladığı gerçekleşen değerlerdir.

- **FM-1**, şirketin kendi finansallarından brüt marj değişimi için kurulan bir senaryo hesabıdır (adı yöntemin kısa adıdır): bir ana sayı ve iki senaryo kolu (alt kol, üst kol). Aynı yöntemin ikinci yüzü, gerçekleşen marj değişiminin hangi kalemlerden (emtia, satış fiyatı, hacim, kur, enflasyon muhasebesi, stok, diğer giderler) oluştuğunu yan yana gösteren bir ayrıştırmadır; "sapma şundan geldi" hükmü vermez. [Kaynak: ürünün hesap kuralı]
- **Alfa**, sektör başına iki yöntemden (FM-1 ve ürünün önceki hesap motoru, "eski motor") hangisinin ana sayısının gösterileceğini önceden yazılmış bir kuralla seçen seçim kuralının kısa adıdır; kural geçmiş yön uyumuna bakar ve sonuç görüldükten sonra değiştirilmez. [Kaynak: ürünün hesap kuralı]
- 2026'nın üçüncü çeyreği (Ç3) bu kayıtların ilk ölçümüdür ve hakem değildir: Ç3'ten yöntem seçimi, geçti/kaldı hükmü ya da yön çıkarılmaz. Sonuçlar [bulgular](bulgular.md) sayfasında.

## 7. Aralık ve yedek kural (2026 Ç4'ten itibaren)

**Aralık.** Ürünün gösterdiği ana sayının iki yanına tek bir yarı genişlik q eklenir: [ana sayı − q, ana sayı + q]. q, o yöntemin kendi geçmiş mutlak hatalarından hesaplanır (bölünmüş konformal yöntem; kapsama %80); şirkete ya da sektöre özgü elle genişlik yoktur, aralık kırpılmaz, yöntemler arasında hata havuzlanmaz. Geçmişi 30 şirketten az olan yöntemde aralık "örnek n=…: kaba" etiketiyle gelir. Kapsama güvencesi hataların aynı dağılımdan geldiği varsayımına dayanır; bu varsayım Ç3'ten Ç4'e ölçülmemiştir. [Kaynak: ürünün hesap kuralı; formül: Angelopoulos ve Bates, arXiv 2107.07511]

Ç3 hatalarıyla (örnek-içi, kanıt sayılmaz) hesaplanan %80 yarı genişlik: FM-1 için ±7,994 puan (n=50), eski motor için ±21,846 puan (n=10, kaba). [Ölçüm: 2026 Ç3'te açıklanan gerçekleşen marjlar üzerinde 15.11.2026'da yapılan hesap]

**Yedek kural.** Alfa'nın seçtiği yöntem bir şirket-çeyrek için sonuç üretmediyse: (1) o şirketin FM-1 kaydı varsa ürün bunu "Alfa çıktısı yok; yedek: FM-1" etiketiyle gösterir ve yedek sayı hiçbir yerde Alfa'nın sayısı diye adlandırılmaz; (2) FM-1 kaydı da yoksa ürün model çıktısı olmadığını yazar ve referans olarak şirketin KAP'ta en son açıklanmış üç aylık gerçekleşen brüt marjını gösterir; bu referans hiçbir yöntemin sayısı sayılmaz, aralığa ve hiçbir ölçüme girmez. [Kaynak: ürünün hesap kuralı]

**Dürüstlük kaydı.** Aralık ve yedek kural, Ç3 sonuçları görüldükten sonra yazıldı; bu yüzden Ç3 için geriye dönük bir kanıt değildir. İlk gerçek sınav 2026 Ç4'tür ve orada kapsama yalnız betimleyicidir: "n=…, k=…" yazılır, "tuttu / tutmadı" hükmü verilmez. [Kaynak: ürünün hesap kuralı]

## Sınırlar

- Sepet ağırlıklarının çoğu varsayımdır; ölçülmüş oran yalnız az sayıda şirkette vardır.
- İzlenen sepet maliyetin tamamı değildir; işçilik ve amortisman sepette yoktur.
- Aynı girdi sepetini ve aynı çıktı endeksini paylaşan şirketlerin fiyat–maliyet farkı sayısal olarak aynıdır; ürün bunu "özdeş seri" diye işaretler ve aralarında fark iddia etmez.
- Ç3 tek çeyrek ve 40–50 şirkettir; ortak bir çeyrek şoku hepsini aynı yönde etkilemiş olabilir.
