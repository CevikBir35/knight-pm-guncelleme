# 1.5.15 — Oyun kapanma uyarısı ve SteamKO metin makrosu

- Takip çalışırken Knight Online oyun penceresi 5 dakika boyunca görünmezse Telegram'a bilgisayar adı ve tespit saatiyle bir uyarı gönderilir. Bu durum oyun kapanınca veya küçültülünce oluşabilir.
- Uyarı, DC yazısını okuyan takipten bağımsız çalışır. Telegram bağlantısı geçici olarak başarısız olursa gönderim yeniden denenir.
- Oyun yeniden görünene kadar aynı kaybolma için tek uyarı verilir. Oyun geri gelince sayaç sıfırlanır.
- Seçenek DC bölümündeki **Oyun 5 dakika görünmezse bildir** kutusundan kapatılabilir; varsayılan olarak açıktır.
- SteamKO bu bilgisayarda yönetici yetkisiyle çalışıyor. Normal açılışta PM programı da Windows yönetici onayı isteyerek aynı yetkiyle yeniden başlar. İzin verilmezse nedenini gösterir.
- Metin makrosu oyun programdan yüksek Windows yetkisine sahipse gönderim sayacını artırmadan durur ve nedeni gösterir.
- Metin makrosu üstteki **Pazar Chat** sekmesine taşındı. Takip ekranındaki PM, item, DC ve güncelleme alanları sade kartlarla yeniden düzenlendi.
- Ulutatış için U harfi ve yükselen ok taşıyan yeni logo eklendi; başlıkta, pencere simgesinde ve EXE simgesinde kullanılır.

## Kontroller

Beş dakikalık eşik, geri dönünce sıfırlama, tek uyarı ve Telegram yeniden deneme testleri geçti. Windows yetki karşılaştırması ile otomatik yönetici açılışının test modunu etkilememesi de test edildi. PM/DC regresyon testleri ile eski güncelleyicinin 1.5.15 dosyasını kabul etmesi kontrol edildi.

Yönetici yetkisiyle açılan 1.5.15 programında Normal modda tek kısa metin gönderimi canlı SteamKO sohbetinde görüldü. Shout, dönüşümlü mod ve tekrarlı gönderim henüz canlı oyunda denenmedi. Takip ve Pazar Chat sekmeleri, tek ve iki sütun yerleşimi ile Canlı Durum kaydırması ayrıca kontrol edildi.
