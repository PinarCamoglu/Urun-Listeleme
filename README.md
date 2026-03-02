ShopLite | Modern Urun Listeleme Arayuzu
Bu proje, modern CSS teknikleri (Flexbox, Grid, Degiskenler) ve responsive tasarim prensipleri kullanilarak gelistirilmis kapsamli bir urun listeleme arayuzudur. Proje kapsaminda tamamen saf HTML5 ve CSS3 kullanilmis, herhangi bir kutuphane veya framework (Bootstrap, Tailwind vb.) tercih edilmemistir.

Proje Ozellikleri
Proje, odev gereksinimlerinde belirtilen tum layout yapilarini ve etkilesim durumlarini icermektedir:

Semantik Yapi: header, main, section, article ve footer gibi anlamli HTML5 etiketleri ile hiyerarsik bir yapi kurulmustur.

Kategorizasyon: Urunler uzerinde Yeni, Populer ve Indirimli etiketleri (badge) bulunmaktadir.

Gelismis Gorunum: CSS Degiskenleri ile yonetilebilir tema renkleri, yumusak golge efektleri ve modern tipografi uygulanmistir.

Erisilebilirlik: Renk kontrasti okunabilirlik standartlarina uygun tutulmus ve erisilebilirlik odakli focus-visible ozellikleri eklenmistir.

Etkilesim: Kartlar uzerinde hover (golge/transform), butonlar uzerinde hover/active ve input alanlarinda belirgin focus durumlari tasarlanmistir.

Teknik Detaylar ve Yerlesim (Layout)
Projede iki ana yerlesim yontemi hibrit olarak kullanilmistir:

Flexbox: Ust bar (Header), Filtre Satiri (Filter Bar) ve Alt Bilgi (Footer) alanlarinda elemanlarin tek boyutlu hizalanmasi ve esnek bosluk yonetimi icin kullanildi.

CSS Grid: Urun listeleme alaninda, kartlarin iki boyutlu bir duzlemde simetrik dizilmesi icin tercih edildi.

Sticky Header: Sayfa kaydirildiginda ust barin sabit kalmasi icin position: sticky ozelligi uygulandi.

Responsive Tasarim (3 Kirilim)
Sayfa, media query kullanilarak uc farkli ekran boyutu icin optimize edilmistir:

Masustu (>= 1024px): Urun gridi 4 sutun olarak goruntulenir.

Tablet (600px - 1023px): Urun gridi 2 sutun yapisina duser.

Mobil (< 600px): Urun gridi 1 sutun olur; header menusu ve filtre alani dikey yerlesime gecer.

Ogrendiklerim ve Zorlandiklarim
CSS degiskenleri kullanmanin, projede renk revizyonu yaparken ne kadar buyuk bir zaman kazandirdigini fark ettim.

Sticky header yapisinda backdrop-filter (bulaniklik efekti) eklerken z-index cakismalari yasadim; katman hiyerarsisini dogru kurgulayarak bu sorunu cozdum.

Grid sisteminde repeat(4, 1fr) kullanimiyla esnek ve hatasiz sutun genislikleri olusturmayi pekistirdim.

Gorsellerin farkli boyutlarda olmasina ragmen kart icinde duzgun durmasi icin object-fit: cover ozelliginin onemini deneyimledim.

Hazirlayan: Pinar Camoglu

Ondokuz Mayis Universitesi - Bilgisayar Muhendisligi