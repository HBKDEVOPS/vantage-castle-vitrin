# Dürüst bulgular

[English](findings.md)

Vantage Castle'ın en önemli tasarım kararı, ne söylemediğidir. Aşağıdaki ölçümler emtia fiyatından marj ya da hisse fiyat serisi değişimi çıkarılıp çıkarılamayacağını denedi; hiçbiri anlamlı bir ilişki bulmadı. Ürün bu yüzden görüş bildirmez, ölçtüğünü yan yana sunar.

Hisse fiyatı kullanan ölçümler kayıtlı seriler üzerinde yapılmış iç çalışmadır. "İlişki yok" burada "bu veriyle, bu yöntemle bulunamadı" demektir; ilişkinin olmadığının kanıtı değildir.

## Denenip bırakılan yollar (altı ölçüm)

Tablodaki "Veri" sütunu ölçümün hangi türde kayıtlı seriye dayandığını gösterir. Bunlar ürünün kendi iç ölçümleridir; ayrıntılı kayıtları bu depoda yer almaz.

| # | Ölçüm | Sonuç | Veri |
|---|---|---|---|
| 1 | Regresyon hattı: şirket bazında ve tek modelde, emtia değişiminden marj ve hisse fiyat serisi değişimi | Anlamlı güç yok; örnek-dışı (2023 sonrası) açıklama gücü negatif, yani basit bir ortalamadan bile kötü | Emtia, marj ve hisse fiyat serileri |
| 2 | Fiyat–maliyet farkının yönü ile gerçekleşen brüt marjın yönü aynı dönemde uyuşuyor mu? | **%49,0** (n=1492, 2015–2022); yazı turadan ayırt edilemedi; hiçbir gecikme ya da hizalama düzeltmesi %55 eşiğini geçmedi | Fiyat–maliyet farkı ve KAP marjı, 2015–2022 |
| 3 | Sektör-nötr ters sıralı iki grup farkı: fark ölçüsü en olumlu şirketlerden oluşan bir grup ile en olumsuz şirketlerden oluşan ters sıralı bir grubun fiyat serisi değişimi farkı | Fark t = **0,613**, p = **0,543**; gürültüden ayırt edilemedi | Fiyat–maliyet farkı ve hisse fiyat serisi |
| 4 | Fiyatlanma ölçümü: fark belirgin değiştiğinde hisse fiyat serisi sektör emsallerinden nasıl ayrıştı? | İlişki bulunamadı | Fiyat–maliyet farkı ve hisse fiyat serisi |
| 5 | Stok devir hızı: stok devir süresi emtia fiyatıyla birlikte değişiyor mu? | İlişki bulunamadı; sabit stok devir varsayımı bu yüzden korunur | Emtia fiyatı ve KAP finansal raporları |
| 6 | KAP olay çalışması: bildirimden sonra hisse fiyat serisi sektöründen normalden fazla ayrışıyor mu? | Yalnız ayrışmanın büyüklüğüne bakar, yönüne bakmaz | KAP bildirimleri ve hisse fiyat serisi |

Ayrıca iki yol bırakıldı: fiyat–maliyet farkının büyük değiştiği dönemleri sonraki marjla eşleştiren "epizot tablosu" kaldırıldı (kanıtlanmamış bir ilişkiyi kanıtlanmış gibi gösterirdi) ve finansal tabloları tüketici fiyatlarıyla ortak tabana çevirme denemesi başarısız oldu, tablolara uygulanmadı.

## Haber yönü etiketi ölçümü (ürün sayfalarında yer almaz)

Haberlere yön etiketi verilip etiketin ardından fiyat serisinin aynı yönde değişip değişmediğine bakıldı; plan etiketleme başlamadan yazılıp dondurulmuştu. Sonuç: etiket yönü ile sonraki fiyat serisi yönü 1, 5 ve 20 işlem gününde %51,2, %50,3 ve %51,5 örtüştü (yazı tura %50); anlamlılık eşiği p < 0,0045 iken bulunan p = 0,449, 0,873 ve 0,366 (n = 1.029, 1.034 ve 1.038 bağımsız küme). Üçü de anlamlı değildir. [Ölçüm: 10.10.2026; haber etiketleri ve hisse fiyat serisi]

İki sınır açıkça yazılır: bu veriyle yaklaşık %55,8'in üstündeki bir etki dışlanabildi, daha küçük bir etki ayırt edilemez; etiketleyiciler arası uyum orta düzeydeydi (κ 0,570–0,657), bu yüzden sonuç "kesin ilişki yok" değil "zayıf yokluk bulgusu" olarak kaydedildi. Bir geleceğe bakma ihlali bulunmadı (0). Bu ölçüm ürüne girmez; etiketler hiçbir ekranda gösterilmez.

## İleri kayıtta ilk ölçüm: 2026 Ç3 (hakem değil)

Hesaplar bilanço açıklanmadan önce yapılır ve kayda geçirilir; gerçekleşen KAP değeri gelince yanına eklenir. 2026'nın üçüncü çeyreğinde 50 şirket için bakıldı. Ç3 hakem değildir: bu tablolardan yöntem seçimi ya da geçti/kaldı hükmü çıkarılmaz.

Tabloda iki kısa ad geçer; ikisi de [yöntem](yontem.md) sayfasında tanımlıdır. Alfa, sektör başına iki yöntemden hangisinin ana sayısının gösterileceğini önceden yazılmış bir kuralla seçen seçim kuralıdır. FM-1, şirketin kendi finansallarından brüt marj değişimi için kurulan, bir ana sayısı ve alt ile üst iki senaryo kolu olan hesaptır.

| Ölçüm | Sonuç | Veri |
|---|---|---|
| Alfa'nın seçtiği yöntemin ana sayısının gerçekleşen marja ortalama mutlak hatası (ana sayısı olan 40 şirket) | **5,855 puan**; "marj bir önceki çeyrekteki gibi kalır" varsayımında 7,140 puan; medyanlar 3,836 ↔ 3,830; 20 şirkette Alfa, 20 şirkette basit varsayım daha yakın | 2026 Ç3: ürünün kayıtlı hesapları ↔ KAP'ta açıklanan gerçekleşen marjlar; 15.11.2026 |
| Aynı ölçüm FM-1 sektörlerinde (35 şirket) | 5,295 ↔ 7,057 puan (Alfa daha yakın 19, basit daha yakın 16) | Aynı veri |
| Aynı ölçüm eski motor sektörlerinde (yalnız 5 şirketin sayısı var) | 9,776 ↔ 7,724 puan (Alfa daha yakın 1, basit daha yakın 4) | Aynı veri |
| Gerçekleşenin FM-1'in alt ve üst senaryo kolları arasına düşmesi | 19 / 49 (0,388); kolları sıralı olan 11 / 29, kolları ters sıralı olan 8 / 20 (ters sıralı kollarda aralık en küçük ile en büyük değer arasında alındı) | Aynı veri |

Okuma notları: (1) Ortalamayı birkaç uç değer yukarı çeker; medyanlar neredeyse aynıdır. (2) Alfa'nın seçim kuralı yön uyumuna bakar, ortalama mutlak hataya değil; hata burada betimleyici ek bir ölçüdür. (3) Eski motorun sayısı olmayan 10 şirkette Alfa'nın çıktısı yoktur; kapsama 40/50'dir. (4) Eski motor kolunda basit varsayım 4/5 şirkette daha yakındır; bu küçük örnek hakkında bir şey söylemez. (5) Ç2 yerine KAP'ın üç aylık Ç2 sütunu kullanıldığında basit varsayımın hatası 7,159 olur (duyarlılık satırı). (6) Tek çeyrek, ortak şok aynı yönde olabilir.

## Bu bulgular ürünü nasıl şekillendirdi

Ürün hisse fiyatı ve yatırım yönü bildirmez, işlem önerisi vermez, "makas daraldı, marj baskısı var" gibi bir durum ya da yön iddiası kurmaz; girdi endeksi, çıktı endeksi, fiyat–maliyet farkı ve gerçekleşen brüt marjı aralarında nedensellik ima etmeden yan yana koyar. Girdi maliyetinden hesaplanan marjı, aralığı ve gerçekleşen marjla farkını kayıt olarak gösterir; bu bir hesaptır, hakem ya da öneri değildir. Bu bir üslup tercihi değil, yukarıdaki ölçümlerin sonucudur. Sistem ölçtüğünü yan yana sunar, yorumu okuyucuya bırakır.
