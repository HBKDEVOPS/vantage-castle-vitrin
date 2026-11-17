# Dürüst bulgular

[English](findings.md)

Vantage Castle'ın en önemli tasarım kararı, ne söylemediğidir. Aşağıdaki ölçümler emtia fiyatından marj ya da hisse fiyat serisi değişimi çıkarılıp çıkarılamayacağını denedi; hiçbiri anlamlı bir ilişki bulmadı. Ürün bu yüzden görüş bildirmez, ölçtüğünü yan yana sunar.

Hisse fiyatı kullanan ölçümler emtia, marj ve hisse fiyat serileri üzerinde yapılmış iç çalışmadır. "İlişki yok" burada "bu veriyle, bu yöntemle bulunamadı" demektir; ilişkinin olmadığının kanıtı değildir.

## Denenip bırakılan yollar (altı ölçüm)

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

## Haber yönü etiketi ölçümü (ürün sayfalarında yer almaz)

Haberlere yön etiketi verilip etiketin ardından fiyat serisinin aynı yönde değişip değişmediğine bakıldı; plan etiketleme başlamadan yazılıp dondurulmuştu. Sonuç: etiket yönü ile sonraki fiyat serisi yönü kısa, orta ve uzun işlem günü ufuklarının üçünde de yazı turadan ayırt edilemedi; üç ölçüm de önceden yazılmış anlamlılık eşiğini geçmedi. Etiketleyiciler arası uyum orta düzeydeydi; bu yüzden sonuç "kesin ilişki yok" değil "zayıf yokluk bulgusu" olarak kaydedildi. Bu ölçüm ürüne girmez; etiketler hiçbir ekranda gösterilmez. [Ölçüm: ekibin iç ölçümü, 10.10.2026; haber etiketleri ve hisse fiyat serisi]

## İleri kayıt ölçümü (hakem değil)

Hesaplar bilanço açıklanmadan önce yapılır ve kayda geçirilir; gerçekleşen değer gelince yanına eklenir. İlk ileri kayıt ölçümü 2026'nın üçüncü çeyreği için yapıldı. Bu ölçüm hakem değildir: ondan yöntem seçimi ya da geçti/kaldı hükmü çıkarılmaz. Ölçümün sayıları bu depoda yer almaz; ürünün ekranlarında kayıt ile gerçekleşen yan yana görünür ([Emtia Marj Motoru](yontem.md#emtia-marj-motoru)).

## Bu bulgular ürünü nasıl şekillendirdi

Ürün hisse fiyatı ve yatırım yönü bildirmez, işlem talimatı vermez, "makas daraldı, marj baskısı var" gibi bir durum ya da yön iddiası kurmaz; girdi endeksi, çıktı endeksi, fiyat–maliyet farkı ve gerçekleşen brüt marjı aralarında nedensellik ima etmeden yan yana koyar. Girdi maliyetinden hesaplanan marjı, bandını ve gerçekleşen marjla farkını kayıt olarak gösterir; bu bir hesaptır, hakem değildir ve yatırım tavsiyesi değildir. Bu bir üslup tercihi değil, yukarıdaki ölçümlerin sonucudur. Sistem ölçtüğünü yan yana sunar, yorumu okuyucuya bırakır.
