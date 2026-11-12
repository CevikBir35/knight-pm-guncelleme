# 1.5.16 — Fabric Coat alış bildirimi ve Pazar onayı

- Fabric Coat(+8) işlem satırı bazen Fabric Goat(+8) veya Fabnc Coat(+8) okunuyordu. Bu üç okuma aynı eşya olarak düzeltilir. Eski gönderim geçmişindeki bu yazımlar da tek işleme eşlenir; aynı alım için tekrar bildirim gönderilmez.
- Onay kuyruğuna kayıt başarısız olursa işlem tüketilmez; sonraki taramada yeniden denenir. Bildirim ile onay kaydı birbirinden kopmaz.
- Takip ekranında Pazar onayının açık veya kapalı olduğu açıkça gösterilir. Kapalıyken işlemlerin siteye gitmediği belirtilir.
- Bu bilgisayardaki Pazar bağlantısı kapalıydı; bu nedenle normal alış Telegram bildirimi gelmesine rağmen Onay Merkezi ve Telegram onay kartı oluşmadı. MsMestan / PC-1 bağlantısı açıldı ve 16:00 Fabric Coat(+8) alımı yerel onay kuyruğuna bir kez eklendi. Program yeniden başladığında kart siteye ve Telegram'a gönderilir.

## Kontrol

16:00 saatli Sylvanasz kaynaklı Fabric Coat(+8), 10.000.000 Coin örneğinin üç OCR yazımıyla yalnızca tek bildirim ve tek onay kuyruğu kaydı oluşturduğu doğrulandı. Onaylandığında stokta bir adet Fabric Coat(+8) ve kasadan 10.000.000 Coin düşümü oluştuğu test edildi. Eski gönderim geçmişiyle uyumluluk ve mevcut PM, item, Pazar köprüsü testleri geçti.
