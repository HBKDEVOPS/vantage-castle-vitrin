# Mimari

![Mimari şema](../sema/mimari.png)

1. **Veri kaynakları.** Kaynağı belirtilen seriler: emtia fiyatları, kurlar, faiz ve enflasyon serileri, şirket finansalları.
2. **Veri hattı.** Günlük ve aylık zamanlı işler kaynakları okur; her satır birim ve tarih kontrolünden geçer ve hangi kaynaktan geldiği kaydedilir.
3. **Ölçüm katmanı.** Her şirket için girdi endeksi (girdi sepetindeki emtiaların ağırlıklı fiyatı), çıktı endeksi (satış fiyatına yakın seri) ve ikisinin oranı olan fiyat–maliyet farkı hesaplanır; gerçekleşen brüt marj yanında durur.
4. **Sunum.** Panom, Harita, Şirketler, Emtialar, Değişimler, Bülten, Projeksiyon, Sektörler, Emtia Ağı, Tedarik Zinciri, KAP, Veri kalitesi ve Tarama sayfaları yalnız ölçüm katmanından okur; her sayının yanında kaynağı yazar.
5. **Demo ve maske kipi.** Yayın kipinde hisse fiyatı, KAP bildirimleri ve bilanço tabloları gösterilmez; maske kipinde ayrıca haber başlıkları, elektrik (EPİAŞ) ve geçiş noktası (PortWatch) değerleri ile hesap bilgileri de gösterilmez. Bu depodaki sayfa görüntüleri maske kipinden alınmıştır.
6. **Geliştirme.** Ürün, yapay zekâ ajanlarından kurulu bir ekiple geliştirilir: her iş planla başlar, üretim ayrı, denetim ayrı oturumda yapılır, dışarı giden her adım insandadır. Ayrıntı: [ekip.md](ekip.md)
