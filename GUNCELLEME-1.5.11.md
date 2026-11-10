# 1.5.11 — DC doğrulama dayanıklılığı

- Kısa süreli OCR kaybı ilk DC okumasını silmez. En fazla 20 saniye içinde aynı yerde ikinci gerçek okuma gerekir; tek okuma bildirim üretmez.
- Genel OCR taraması zaman aşımına uğrarsa daha dar uyarı alanı yine taranır.
- DC takibi kapalı, ilk okuma, doğrulama ve zaten bildirilmiş uyarı durumları Canlı Durum ve dc_tani.log içinde açıkça gösterilir.
- 1.5.10 K PM düzeltmesi korunur.

## Kontroller
Gönderilen gerçek DC ekranı yüzde 75, 100 ve 125 ölçekte okundu. Altı test; kesintili okuma, zaman aşımı yedeği, tekrar bildirim koruması, yeniden bağlanma sonrası yeni DC ve gönderim hatası sonrası kuyruk yeniden denemesini kapsıyor. Telegram gönderimleri testte taklit edildi, canlı oyun doğrulaması yapılmadı.

Gönderilen ekran eski kodda da okunuyordu. Olay anının günlüğü olmadan yaşanan kaçırmanın kesin nedeni belirlenemedi; bu sürüm doğrulanan dayanıklılık açıklarını kapatır ve sonraki olayın hangi aşamada kaldığını görünür kılar.

Programdan Güncellemeleri denetle ile yükleyin; sürüm 1.5.11 olmalıdır.
