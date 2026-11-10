# 1.5.10 — Gerçek video ile K PM algılama düzeltmesi

Gönderilen yakın çekimdeki K çubuğu eski şablonlarla 270 karenin hiçbirinde bulunamıyordu. Oyuncu adı içermeyen sabit sol/sağ çerçeve örnekleri eklendi. Genel videoda çerçeve bulunmasına rağmen isimdeki ince piksellerin parlamayla değişmesi aynı oyuncuyu iki ayrı takibe bölüyor, bu yüzden yanıp sönme doğrulanmıyordu.

K çubuğunda mevcut isim maskesine ek olarak arka planı çıkarılmış gri tonlu isim çizgileri karşılaştırılır. Bu ek eşleşme yalnızca aynı yerde, 1,8 saniyeden uzun süre kaybolmadan takip edilen çubuklarda kullanılır. Ekran kaydındaki düzensiz zaman aralıkları da dikkate alındı.

Doğrulama:
- Yakın çekimde 270 karenin 252'sinde çerçeve tanındı; tek takip kaydı ve yaklaşık 2,28 saniyede tek bildirim oluştu.
- Genel video kendi zaman damgalarıyla, her beşinci kare örneklenerek baştan sona oynatıldı: 384/384 örnekte çerçeve bulundu, tek takip kaydı ve yaklaşık 3,22 saniyede tek bildirim oluştu. Bildirim onayından sonra tekrar gönderim oluşmadı.
- Önceki 16 görüntü/satış testi ve 11 hassas K PM testi geçti. Daha önce gönderilen küçük K görselleri canlı yerel doğrulama yolunda da tek bildirim üretti.

Videolar çevrimdışı oynatıldı; gerçek oyun oturumuna veya Telegram'a test mesajı gönderilmedi. Dragon'un ikinci yanıp sönme hâli bu videolarda olmadığından Dragon sorununun çözüldüğü iddia edilmez.

Kurulum: Programda Güncellemeleri denetle → 1.5.10.
