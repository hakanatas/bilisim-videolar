# Çıtır'ın Meyve Okulu

5. sınıf için makine öğrenmesinin temel fikrini gösteren bir araç. Öğrenci, robot Çıtır'a meyve ayırmayı örneklerle öğretiyor ve Çıtır'ın "beyninin" her örnekte nasıl değiştiğini haritada görüyor.

Tek dosya: `index.html`. Tarayıcıda açılır. Yazı tipleri dışında internet gerekmez; kütüphane de kullanmaz.

## Adımlar

1. **Tanış:** Çıtır hiçbir şey bilmiyor ve getirilen meyveyi tahmin edemiyor. Resmi görmediğini, yalnızca iki **özellik** ölçtüğünü anlatıyor: uzunluk ve renk.
2. **Öğret:** Öğrenci banttaki meyveyi doğru sepete koyuyor. Her meyve bir **örnek**, sepet de onun **etiketi**. Örnekler haritada nokta oluyor ve renkli bölgeler Çıtır'ın tahminlerini gösteriyor.
3. **Sına:** Çıtır daha önce görmediği meyveleri tahmin ediyor. Nedenini de söylüyor: "Buna en çok benzeyen 3 örneğe baktım." Bu 3 örnek haritada çizgiyle gösteriliyor. Yanılırsa öğrenci doğrusunu öğretebiliyor.
4. **Deney yap:** Üç deney var:
   - Az örnek mi, çok örnek mi? Başarı yüzdesi karşılaştırılıyor.
   - Hiç yeşil elma görmezse? Veri çeşitliliği ve önyargı konusu.
   - Yanlış öğretirsek ne olur? Hatalı etiketlerin etkisi.
5. **Ne öğrendik?** Beş maddelik özet ve günlük hayattan örnekler: istenmeyen e-posta, fotoğraf albümü, öneriler.

Haritada herhangi bir yere dokunmak "hayalî bir meyve" sorar. Öğretmen bununla sınıfa "Sence Çıtır burada ne der?" diye sorabilir.

## Öğretmen için

- Çıtır'ın bütün konuşmaları dosyanın başındaki `METIN` nesnesinde. Tırnak içlerini değiştirmen yeterli.
- Öğret adımındaki "Öğretmen: 12 örneği otomatik ekle" bağlantısı derste zaman kazandırır.
- Arka planda "en yakın komşu" (k-NN, k = 3) yöntemi çalışıyor. Çıtır'ın açıklaması bu yöntemi 5. sınıf diliyle anlatıyor.
- Açık ve koyu tema, telefon ve akıllı tahta düzeni destekleniyor.
