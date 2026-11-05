# Mütalaa: Hukuk, Mevzuat, İçtihat ve Vergi

Mütalaa, Türk hukuku için mevzuat ve içtihat araştırmasını Claude'a getirir.
Kanun, madde metni ve gerekçe resmi kaynaktan aranıp okunur. Yargıtay, Danıştay,
bölge adliye, ilk derece hukuk mahkemesi ve Anayasa Mahkemesi (AYM) için emsal
karar araması yapılabilir. Vergi sorularında GİB özelge araması da var. Claude
cevabında kaynağın bağlantısını verebilir.

Bu eklenti, Mütalaa bağlantısının yanına dört Türkçe skill ekler. Skill'ler
soruyu mevzuat, karar ya da özelge aramasına yönlendirir. Sonuca varmadan önce
ilgili metni okutur, kaynak hatalarını ve kota sınırlarını açıklar. Borçlar
hukuku, ticaret hukuku, iş hukuku, aile hukuku, miras hukuku, ceza hukuku,
idare hukuku, vergi hukuku ve anayasa hukuku gibi alanlarda kullanılabilir.

## Kurulum

Claude'da Customize sayfasındaki eklentiler bölümünden Mütalaa'yı ekleyin.
Bağlanırken Mütalaa giriş sayfası açılır. Hesabınız yoksa orada açabilirsiniz.

Claude Code'da:

```text
/plugin marketplace add hburaktasyurek/mutalaa-plugin
/plugin install mutalaa@mutalaa
```

Ardından `/mcp` içinde Mütalaa bağlantısını seçip Mütalaa hesabınızla giriş
yapın ve yeni bir oturumda sorunuzu sorun. Videolu kurulum rehberi
https://mutalaa.tr/start adresinde.

## Neler gönderilir

Araç çağrıları arama terimlerini, filtreleri ve herkese açık belge
kimliklerini, giriş yapılmış hesapla https://mutalaa.tr/mcp adresindeki
Mütalaa sunucusuna gönderir. Sunucu metinleri kamu kurumlarının herkese açık
kaynaklarından getirir. Mütalaa arama metnini saklamaz. Konu, alt konu ve amaç
alanları yalnız kullanım istatistiği için kaydedilir. Ayrıntılar gizlilik
politikasında (https://mutalaa.tr/legal).

Sorularınıza müvekkil adı ve dosya ayrıntısı yazmayın. Skill'ler modele araç
girdilerini anonimleştirmesini söyler, ama sunucu kişisel veriyi ayrıca
temizlemez. Paket kimlik bilgisi, yerel sunucu, kurulum betiği ya da kanca
içermez.

## Kapsam

Mütalaa hukuki bilgi ve kaynak araştırması sunar, avukatlık hizmeti vermez.
Ceza istinafı ve bölge idare mahkemesi araması, UYAP'taki kişisel dosyalar ve
yalnız yabancı hukuka dair araştırma bu sürümün dışında.

## Yayıncı ve destek

- Yayıncı Hasan Burak Taşyürek
- Destek admin@mutalaa.tr
- Web sitesi https://mutalaa.tr
- Gizlilik politikası ve kullanım koşulları https://mutalaa.tr/legal

## English

Mütalaa brings Turkish law, legislation and case law research into Claude.
Search and read laws, article texts and legislative rationales, court decisions
from Yargıtay, Danıştay, regional appellate and first-instance civil courts and
the Constitutional Court (AYM), and GİB private tax rulings, with source links.
This plugin adds four Turkish workflow skills to the Mütalaa connector at
https://mutalaa.tr/mcp, which users sign in to with OAuth.

Tool calls send search terms, filters and public document identifiers to the
Mütalaa server with the signed-in account. The server retrieves texts from the
public sources of Turkish public institutions. Search text is not stored.
Topic, subtopic and purpose fields are recorded only for usage statistics. The
package contains no credentials, local server, install scripts or hooks.

## Lisans

`LICENSE` içindeki MIT izni, skill ve referans Markdown dosyalarını ve eklenti
ile MCP manifest JSON dosyalarını kapsar. Mütalaa adı, logosu ve `assets/`
klasörü bu iznin dışındadır, marka hakkı verilmez. Sunucu kodu bu pakette yok.
