# GİB özelge araştırması

Vergi konusundaki idari görüş veya belirli bir özelge gerektiğinde bu akışı kullan.
Özelgeyi içtihat veya mahkeme kararı olarak sınıflandırma. Genel değerlendirmede
önce ilgili mevzuatı incele; yalnız özelge bulma talebini genişletme.

1. Vergi türünü, işlemi ve gerekiyorsa dönemi belirle. Sonucu değiştiren bilgi
   eksikse tek soru sor; cevaba bağlı uygulama değerlendirmesini beklet.
2. Ana skill'in anonimleştirme kuralını bütün araç girdilerine uygula;
   `gib_ozelge_ara` aracını kimliksiz, kısa bir `sorgu` ile çağır. Özel olayı
   ayırt eden ayrıntıları taşımak yerine hukuki işlem ve vergi kavramlarını kullan.
   Parametreleri mevcut araç şemasından doğrula; desteklenmeyen filtre uydurma.
3. Adayın kurum, başlık, tarih, numara ve kaynak bağlantısını incele. İlgili
   olanı `id` değeriyle `belge_getir` üzerinden oku. `next_page` varsa ilgili
   olay, gerekçe ve sonuç tamamlanana kadar gereken sayfalara devam et.
4. Özelgedeki olay ile kullanıcının olayı arasındaki farkları belirt. Görüşü
   otomatik olarak herkese uygulanacak hüküm diye sunma. Yargı kararı gerekiyorsa
   ana akıştan ayrıca uygun içtihat alt akışına geç.
5. Bulguyu özelge numarası, kaynak tarihi, kurum ve bağlantıyla aktar. Belgenin
   kalıcı arşivde bulunması görüşün güncel mevzuatla uyumlu olduğunu tek başına
   kanıtlamaz. Yeterli kanıt elde edilince dur.

Boş arama ile erişim/okunamama hatasını ayır. Yoğunluk/kota yanıtında verilen
bekleme bilgisini uygula; yeni bir gerekçe olmadan aynı çağrıyı tekrarlama.
