# ayna

Profil fotoğrafını değiştirmeden önce **WhatsApp, Instagram, X ve TikTok**'ta gerçek boyutunda nasıl duracağını gör. Dilediğin gibi ölçekle, kırpılmış halini orijinal kalitede indir.

**Canlı:** https://erentaskale.github.io/ayna/

## Ne yapıyor?

- **Gerçek boyutlu önizleme:** Fotoğrafın dört uygulamanın güncel arayüzlerinde, telefonda kapladığı alan kadar gösterilir (1 CSS pikseli = 1 piksel, iPhone genişliği 390 px).
- **Her boyutta kontrol:** Sohbet listesindeki 28 px'lik daireden 150 px'lik web profiline kadar, fotoğrafın göründüğü tüm boyutlar yan yana.
- **Kırp ve indir:** Sürükle, yakınlaştır; ekranda gördüğün kırpma, orijinal fotoğrafın kendi pikselleriyle indirilir. Büyütme, küçültme yok. PNG kayıpsız, JPG %98 kalitede.
- **X kapağı:** 3:1 kapak fotoğrafı, profil fotoğrafının üstüne bindiği haliyle.
- **Açık / koyu tema**, **sürükle-bırak** ve **Ctrl+V ile yapıştırma**.

## Gizlilik

Fotoğrafın hiçbir sunucuya gönderilmez. Bütün işlem tarayıcında yapılır.

## Kullanım

Kurulum yok. `index.html` dosyasını tarayıcıda açman yeterli.

## Teknik

Tek dosya: HTML, CSS ve saf JavaScript. Framework ya da derleme adımı yok.

- Önizlemelerdeki ölçüler sayfadan canlı ölçülüp her ekranın altına yazılır.
- Kırpma, ekrandaki CSS (`object-fit: cover` + `object-position` + `scale`) ile aynı hesapla `<canvas>` üzerinde çizilir; indirilen dosya önizlemenin birebir aynısıdır.
- Ölçüler uygulamaların Ekim 2026 arayüzlerine göredir; uygulamalar güncellendikçe birkaç piksel oynayabilir.
