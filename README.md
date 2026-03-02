ShopLite Ürün Listeleme Projesi

1. Kullanılan Layout Yöntemleri:
- Header, Filtre Satırı ve Footer alanlarında elemanları yan yana dizmek ve esnek bir yapı kurmak için Flexbox (display: flex) kullanılmıştır.
- Ürün kartlarının ızgara yapısında düzenli bir şekilde listelenmesi için CSS Grid (display: grid) kullanılmıştır.

2. Breakpoint'ler (Kırılım Noktaları):
- Masaüstü (>= 1024px): 4 sütunlu grid yapısı.
- Tablet (600px - 1023px): 2 sütunlu grid yapısı.
- Mobil (< 600px): 1 sütunlu grid yapısı ve dikey yerleşimli header/filtre alanı.

3. Öğrendiklerim ve Zorlandıklarım:
- CSS değişkenleri kullanarak renk ve tasarım tutarlılığını sağlamanın projenin yönetilebilirliğini ne kadar artırdığını deneyimledim.
- Grid yapısında 'repeat' ve 'fr' birimlerini kullanarak responsive sütunlar oluşturmayı pekiştirdim.
- Başlangıçta sticky header'ın z-index değerini ayarlarken çakışmalar yaşadım ancak katman hiyerarşisini düzenleyerek çözdüm.
- Erişilebilirlik için :focus-visible ve kontrast oranlarına dikkat etmenin önemini kavradım.