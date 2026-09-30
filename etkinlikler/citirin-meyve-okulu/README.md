# Çıtır'ın Meyve Okulu

5. sınıf için makine öğrenmesinin temel fikrini gösteren 3B bir atölye. Öğrenci, meyve bahçesinin yanındaki atölyede robot Çıtır'a banttan gelen meyveleri sepetlere ayırmayı öğretiyor. Öğretilen her örnek arkadaki "Çıtır'ın Beyni" panosunda bir nokta oluyor.

Tek dosya: `index.html`. İnternet bağlantısı gerekir; Three.js `cdn.jsdelivr.net`, yazı tipleri `fonts.googleapis.com` adresinden yüklenir. Okul ağı bu adresleri engellerse sayfa bunu Türkçe bir mesajla söyler.

## Adımlar

1. **Tanış:** Çıtır hiçbir şey bilmiyor ve getirilen meyveyi tahmin edemiyor. Resmi görmediğini, yalnızca iki **özellik** ölçtüğünü anlatıyor: uzunluk ve renk.
2. **Öğret:** Öğrenci banttaki meyveyi doğru sepete koyuyor (paneldeki düğmelerle ya da 3B sepete dokunarak). Her meyve bir **örnek**, sepet de onun **etiketi**. Meyve sepete uçuyor, bir ışık da panoya giderek orada nokta oluyor ve renkli bölgeler Çıtır'ın tahminlerini gösteriyor.
3. **Sına:** Çıtır daha önce görmediği meyveleri tahmin ediyor. Nedenini de söylüyor: "Buna en çok benzeyen 3 örneğe baktım." Bu 3 örnek panoda çizgiyle gösteriliyor. Yanılırsa öğrenci doğrusunu öğretebiliyor.
4. **Deney yap:** Üç deney var:
   - Az örnek mi, çok örnek mi? Başarı yüzdesi karşılaştırılıyor.
   - Hiç yeşil elma görmezse? Veri çeşitliliği ve önyargı konusu.
   - Yanlış öğretirsek ne olur? Hatalı etiketlerin etkisi.
5. **Ne öğrendik?** Beş maddelik özet ve günlük hayattan örnekler: istenmeyen e-posta, fotoğraf albümü, öneriler.

Beyin panosunda herhangi bir yere dokunmak "hayalî bir meyve" sorar. Öğretmen bununla sınıfa "Sence Çıtır burada ne der?" diye sorabilir.

## Öğretmen için

- Çıtır'ın bütün konuşmaları dosyanın başındaki `METIN` nesnesinde. Tırnak içlerini değiştirmen yeterli.
- Öğret adımındaki "Öğretmen: 12 örneği otomatik ekle" bağlantısı derste zaman kazandırır.
- Arka planda "en yakın komşu" (k-NN, k = 3) yöntemi çalışıyor. Çıtır'ın açıklaması bu yöntemi 5. sınıf diliyle anlatıyor.
- Sağ üstte Bölgeler (panodaki renkli tahmin bölgeleri), Görünümü sıfırla ve Kalite düğmeleri var. Telefonda ve zayıf donanımda Hafif mod kendiliğinden açılır. Sahneyi sürükleyerek çevirebilirsin.
- Açık ve koyu tema, telefon ve akıllı tahta düzeni destekleniyor.
