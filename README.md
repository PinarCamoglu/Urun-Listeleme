# ShopLite | Modern Ürün Listeleme Arayüzü

Bu proje, modern CSS teknikleri (Flexbox, Grid, CSS Değişkenleri) ve responsive tasarım prensipleri kullanılarak geliştirilmiş bir e-ticaret arayüzü çalışmasıdır.  
Proje kapsamında tamamen saf HTML ve CSS kullanılmış, herhangi bir kütüphaneye (Bootstrap, Tailwind vb.) yer verilmemiştir.

---

## Proje Özellikleri

- **Semantik Yapı:**  
  `header`, `main`, `section`, `article` ve `footer` gibi anlamlı HTML5 etiketleri kullanılmıştır.

- **Modern UI:**  
  CSS Değişkenleri ile yönetilebilir tema rengi ve yumuşak gölge efektleri uygulanmıştır.

- **Kategorizasyon:**  
  Ürünler üzerinde "Yeni", "Popüler" ve "İndirimli" etiketleri (badge) bulunmaktadır.

- **Etkileşim:**  
  Hover efektleri, buton aktif durumları ve erişilebilirlik odaklı `focus-visible` özellikleri eklenmiştir.

---

## Teknik Detaylar

### 1. Yerleşim (Layout) Stratejileri

Projede iki ana layout yöntemi hibrit olarak kullanılmıştır:

- **Flexbox:**  
  Üst bar (Header), filtre satırı (Filter Bar) ve alt bilgi (Footer) alanlarında elemanların tek boyutlu hizalanması ve esnek boşluk yönetimi için kullanılmıştır.

- **CSS Grid:**  
  Ürün listeleme alanında, kartların iki boyutlu bir düzlemde (satır ve sütun) simetrik dizilmesi için kullanılmıştır.

---

### 2. Responsive Tasarım (Kırılım Noktaları)

Sayfa, üç farklı ekran boyutu için optimize edilmiştir:

- **Masaüstü (>= 1024px):**  
  Ürün grid yapısı 4 sütun olarak görüntülenir.

- **Tablet (600px - 1023px):**  
  Ürün grid yapısı 2 sütuna düşer.

- **Mobil (< 600px):**  
  Ürün grid yapısı 1 sütun olur; header menüsü ve filtre alanı dikey yerleşime geçer.

---

### 3. Kullanılan CSS Değişkenleri

Tasarım tutarlılığını sağlamak için `:root` altında tanımlanan temel değişkenler:

```css
--primary: Ana marka rengi (#2563eb)
--bg: Sayfa arka plan rengi
--text: Ana metin rengi
--muted: Yardımcı metin rengi
--radius: Kenar yumuşatma (12px)
--shadow: Kart ve bileşen gölgeleri
```

### 4. Öğrendiklerim ve Zorlandıklarım

#### Öğrendiklerim
- CSS değişkenleri kullanmanın, büyük projelerde renk revizyonu yaparken ciddi zaman kazandırdığını fark ettim.
- Grid sisteminde `repeat(4, 1fr)` kullanımıyla esnek ve hatasız sütun genişlikleri oluşturmayı pekiştirdim.
- Farklı boyuttaki görsellerin kart içinde düzgün görünmesi için `object-fit: cover` özelliğinin önemini öğrendim.

#### Zorlandıklarım
- Sticky header yapısında `backdrop-filter` (bulanıklık efekti) eklerken `z-index` çakışmaları yaşadım.
- Katman hiyerarşisini doğru kurgulayarak bu sorunu çözdüm.

**Hazırlayan:** [Pınar Çamoğlu](https://github.com/PinarCamoglu)  
*Ondokuz Mayıs Üniversitesi - Bilgisayar Mühendisliği*