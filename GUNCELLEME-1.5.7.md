# 1.5.7 — K sembollü PM için hassas sarı ton takibi

K sembollü PM çubuğunda yanıp sönme ölçümü değiştirildi. Önceki ölçüm, isim bölgesinin altındaki yeşil kanal ortancasını kullanıyordu. Üstteki ince sarı şerit yanarken bu alan çok az değişebilir veya aynı kalabilir. Yeni ölçüm isim yazısının üstündeki şeridin kırmızı ve yeşil kanallarını birlikte izler. Genel parlaklık ve renk değişimlerini azaltmak için sabit kare simgenin içi referans alınır.

K desenine özel normalleştirilmiş eşik 0.060 oldu. Zayıf değişimlerde beş yön değişimi, güçlü değişimlerde üç yön değişimi doğrulanır. Sabit çubuk, tek renk değişimi veya hızlı gürültü bildirim üretmez. Tekrar bildirim için gereken sakinlik eşiği de yeni hassasiyete uyarlandı; düşük kontrastlı yanıp sönme yanlışlıkla “okundu” sayılmaz. K örnekleme geçmişi yavaş yanıp sönmelere yetecek şekilde 8,5 saniyedir. Diğer PM desenlerinin eşiği korunur.

Canlı Durum'a “K PM … örnek, ton farkı … eşik 0.060” satırı eklendi. Çerçeve tanındığı halde yanıp sönme doğrulanamıyorsa nedenini bu kayıtla ayırt edebiliriz. Açılışta “K çubuğunda hassas sarı ton takibi etkin” yazısı görünür.

## Kontroller

- 156 otomatik test geçti: yeni 11 hassas PM testi, önceki 16 görüntü/satış testi, 6 PM çalışma döngüsü testi, 5 eski PM testi, 99 genel işlem/DC testi ve 19 site/Telegram entegrasyon testi.
- Gönderilmiş yanık/sönük K görselleri, 21 ara ton, 9 görüntü ölçeği, dar seçilmiş çerçeve, hareket eden iki ayrı oyuncu ve canlı yerel doğrulama yolu kontrol edildi.
- Eski ölçümde değişim üretmeyen, kaynak görselin üst şeridine yalnızca 4/255 kırmızı/yeşil artışı uygulanmış testte yeni ölçüm 0,104 fark gördü ve bir kez bildirim oluşturdu.
- Sabit görüntü, rastgele piksel gürültüsü, tek değişim, yavaş aydınlanma, tüm çubukta parlaklık/renk değişimi, hızlı titreme, geçici kaybolma, tekrar engelleme ve okunduktan sonra yeniden bildirim testleri geçti.
- Eski PM çerçevelerinin beş oyunculu canlı tarama benzetimi ve yavaş tarama kontrolleri geçti.
- Paketlenmiş EXE eski 1.4.21 `_internal` dosyalarıyla arayüz, K/NP/standart PM, hassas yanıp sönme, OCR ve token koruması öz testini geçti.
- Değiştirilmemiş 1.4.21 güncelleyicisi yeni EXE'yi doğru SHA-256 ile kabul etti; hatalı SHA-256'yı reddetti.

Gerçek oyun oturumunda PM alınmadı ve test için Telegram'a mesaj gönderilmedi. Bildirilen olayı aynı bilgisayarda canlı gözlemlemediğimiz için kesin tek sebep iddiası yoktur; düşük kontrastlı sarı şeridin ölçümde kaybolması testte yeniden üretilip giderildi.

Kurulum: PM programındaki **Güncellemeleri denetle** ile **1.5.7** sürümüne geçin. PM alanı iki uç düğmesini ve üst sarı şeridi içermeli. Site dosyası, stok/kasa verileri ve Telegram bot ayarları değiştirilmedi.
