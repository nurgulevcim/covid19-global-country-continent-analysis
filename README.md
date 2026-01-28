# Global COVID-19 Pandemisinin Ülke ve Kıta Bazlı Analizi

Bu çalışma, COVID-19 pandemisinin küresel ölçekteki etkilerini **ülke ve kıta bazında** incelemektedir.  
Amaç, yalnızca küresel toplamlara bakmak yerine; vaka, ölüm, iyileşme ve test göstergeleri üzerinden pandeminin **heterojen yapısını** ortaya koymaktır.

---

## 1. Giriş (Introduction)

COVID-19 pandemisi, ülkeler ve kıtalar arasında hem yayılım hem de sonuçlar açısından belirgin farklılıklar göstermiştir.  
Bu çalışma, pandeminin etkilerini hem **küresel toplamlar** hem de **ülke ve kıta bazlı göstergeler** üzerinden analiz etmeyi amaçlamaktadır.

Analizde kullanılan temel göstergeler:
- Toplam vaka sayıları  
- Toplam ölüm sayıları  
- İyileşen vaka sayıları  
- Yapılan test sayıları  

Bu göstergeler aracılığıyla pandeminin küresel ölçekte **eşit olmayan etkileri** incelenmiştir.

---

## 2. Veri ve Yöntem (Data & Methodology)

Analizde günlük COVID-19 verileri kullanılmıştır. Veri temizleme ve ön işleme sürecinde aşağıdaki adımlar izlenmiştir:

- Eksik **Deaths** ve **Recovered** değerleri 0 ile doldurulmuştur.
- **Tests** değişkenindeki eksik gözlemler medyan değer ile tamamlanmıştır.
- **“All”** ve kıta toplamı niteliğindeki gözlemler, ülke bazlı analizlerden çıkarılmıştır.
- Ölüm oranı, iyileşme oranı ve nüfus başına vaka göstergeleri türetilmiştir.

### Türetilen Göstergeler
  
- **Ölüm Oranı (Fatality Rate)**  
  `Fatality Rate = Deaths / Confirmed`

- **İyileşme Oranı (Recovery Rate)**  
  `Recovery Rate = Recovered / Confirmed`

- **Milyon Kişi Başına Vaka Sayısı (Cases per Million)**  
  `Cases per Million = (Confirmed / Population) × 1,000,000`

Analiz süreci; betimsel istatistikler, sıralama analizleri, kıtasal karşılaştırmalar ve korelasyon analizlerinden oluşmaktadır.

---

## 3. Betimsel Bulgular (Descriptive Findings)

### 3.1 Küresel (Global) Göstergeler

- **Toplam vaka:** 2.11 milyar  
- **Toplam ölüm:** 21.0 milyon  
- **Toplam iyileşen:** 1.91 milyar  
- **Toplam test:** 7.08 milyar  

Buna göre:
- **Global ölüm oranı:** %0.99  
- **Global iyileşme oranı:** %90.42  

Bu oranlar, dünya genelinde tespit edilen vakaların büyük çoğunluğunun iyileşme ile sonuçlandığını göstermektedir.

---

### 3.2 Ülke Bazlı Oranlar (Mean & Median)

| Gösterge | Ortalama | Medyan |
|--------|----------|--------|
| Ölüm Oranı | %1.38 | %0.88 |
| İyileşme Oranı | %73.6 | %97.3 |

Ortalama ve medyan arasındaki fark, ülkeler arasında **belirgin heterojenliğe** işaret etmektedir.  
Bazı ülkelerdeki yüksek ölüm oranları, ortalama değerleri yukarı çekmektedir.

---

## 4. Sıralama Analizleri (Top-10 Countries)

### 4.1 En Çok Vaka Görülen Ülkeler
ABD, Hindistan ve büyük Avrupa ülkeleri toplam vaka sayılarında öne çıkmaktadır.

### 4.2 En Çok Ölüm Yaşanan Ülkeler
ABD, Brezilya ve Hindistan listenin üst sıralarında yer alırken, Latin Amerika ülkelerinin ölüm sıralamasında daha üstte yer aldığı görülmektedir.

### 4.3 En Çok Test Yapan Ülkeler
Test kapasitesi açısından ABD, Hindistan ve Avrupa ülkeleri öne çıkmaktadır.

### 4.4 Nüfusa Oranla Etkilenen Ülkeler
Küçük nüfuslu ülkeler (ör. San Marino, Brunei) vaka/milyon göstergesinde üst sıralarda yer almakta; bu durum kişi başına düşen göstergelerin nüfus büyüklüğüne duyarlılığını göstermektedir.

---

## 5. Kıtasal Karşılaştırmalar (Continental Comparison)

### 5.1 Kıta Bazlı Ölüm Oranları

| Kıta | Ölüm Oranı |
|------|------------|
| Africa | %2.01 |
| South America | %1.95 |
| North America | %1.29 |
| Europe | %0.83 |
| Asia | %0.70 |
| Oceania | %0.22 |

Afrika ve Güney Amerika, mutlak vaka sayıları görece düşük olmasına rağmen en yüksek ölüm oranlarına sahiptir.  
Okyanusya ise en düşük ölüm oranı ile ayrışmaktadır.

📌 Bu bulgular, sağlık sistemine erişim, test kapasitesi ve erken müdahale politikalarının önemini vurgulamaktadır.

---

## 6. Korelasyon Analizi (Correlation Analysis)

### 6.1 Test Sayısı – Vaka Sayısı
- **Korelasyon katsayısı:** r = 0.84  

Test kapasitesi arttıkça tespit edilen vaka sayısının da arttığı görülmektedir.

### 6.2 Nüfus – Vaka Sayısı
- **Korelasyon katsayısı:** r = 0.37  

Nüfus büyüklüğü vaka sayısını kısmen açıklasa da tek başına belirleyici değildir.

---

## 7. Sonuç ve Değerlendirme (Conclusion)

Bu çalışma, COVID-19 pandemisinin küresel etkilerinin ülkeler ve kıtalar arasında **ciddi biçimde farklılaştığını** ortaya koymaktadır.  
Küresel oranlar genel durumu özetlerken, ülke bazlı analizler sağlık altyapısı, test stratejileri ve demografik yapının önemini vurgulamaktadır.

Elde edilen bulgular, pandemiye yönelik politika tasarımlarında **tek tip çözümler yerine bölgesel ve ülke-özel yaklaşımların** gerekliliğini göstermektedir.

---

## 📂 Proje İçeriği

- Jupyter Notebook (`covid19_analysis.ipynb`)
- Üretilen grafikler (`plots/`)
- Kullanılan veri seti (`covid_19.csv/`)
