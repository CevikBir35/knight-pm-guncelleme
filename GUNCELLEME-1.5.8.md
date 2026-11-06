# 1.5.8 — Canlı Durum günlüğünde kaydırma

Canlı Durum kutusunun fare tekerleği ana pencereyi de kaydırıyordu. Yeni kayıt ekleyen kod da her mesajda görünümü zorla en sona götürüyordu. Bu iki davranış düzeltildi.

- Günlüğe ayrı bir dikey kaydırma çubuğu eklendi.
- Fare günlük kutusunun üzerindeyken tekerlek yalnızca kayıtları kaydırır. Üst/alt sınıra ulaşınca ana pencereye geçmez.
- Küçük tekerlek hareketleri biriktirilir; hassas fare/trackpad hareketleri kaybolmaz.
- Eski mesajlar okunurken yeni kayıtlar ekranın yerini değiştirmez. Son kayda dönünce yeni mesajları izleme devam eder.
- “İlk kayıt” ve “Son kayıt” düğmeleri eklendi. Günlük odaktayken Ctrl+Home / Ctrl+End de kullanılabilir.
- Bir arayüz yenilemesinde en fazla 200 mesaj eklenir; yoğun günlük akışı kaydırma olaylarını bekletmez.
- Ana pencerenin tekerlek dinleyicisi ayrı ayar pencerelerine karışmaz.

Doğrulama: 10 gerçek Tk arayüz testi, 11 hassas K-PM testi ve 6 PM çalışma döngüsü testi geçti (27 test). 10.000 ek kayıt sonrasında ilk mesajın erişilebilir kalması, yeni mesaj geldiğinde eski görünümün korunması, son kaydı izleme, kaydırma çubuğu bağlantısı, tekerleğin iki yönde çalışması, hassas tekerlek hareketleri, sınırda ana pencerenin oynamaması ve yoğun kuyruk kontrol edildi.

Paketlenmiş EXE eski 1.4.21 çalışma dosyalarıyla arayüz, günlük bileşeni, K/NP/standart PM, OCR ve Windows token koruması öz testini geçti. Değiştirilmemiş eski güncelleyicide EXE değiştirme hazırlığı ve SHA-256 doğrulaması kontrol edildi.

Kurulum: PM programında **Güncellemeleri denetle → 1.5.8**. Bu sürüm PM programının Canlı Durum ekranını günceller. Site dosyası değiştirilmedi. Testlerde oyun veya Telegram'a bağlanılmadı.
