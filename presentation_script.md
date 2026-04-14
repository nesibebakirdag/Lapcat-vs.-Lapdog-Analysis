# Waggle Projesi: Lapcat vs. Lapdog Yönetici Paneli Sunumu

Sayın Yönetim Kurulu / Değerli Jüri Üyeleri, merhabalar.
Bugün sizlere Veri Analitiği (Data Analytics) ekibimiz tarafından hazırlanan **Lapcat vs. Lapdog Performans Analizi ve Yönetici Paneli'ni (Executive Dashboard)** sunacağız.

Sunumumuzu 4 ana başlıkta toparlayacağız: Projenin vizyonu, kullandığımız mimari, elde ettiğimiz analitik içgörüler ve nihai stratejik kararımız.

---

## BÖLÜM 1: Yönetici Özeti ve Proje Amacı (Home Sayfası)
**Konuşmacı 1:**
"Waggle şirketi olarak akıllı köpek tasmamız 'Lapdog' ile uzun süredir pazarda güçlü bir konumdayız ve müşteri sadakatimiz oldukça yüksek. Bu majör başarının ardından stratejik bir soru gündeme geldi: *'Mevcut teknolojimizi ve marka gücümüzü kullanarak kediler için tasarladığımız Lapcat ürünü, şirketimiz için kârlı bir inovasyon olabilir mi, yoksa markamıza zarar verebilecek riskli bir deneme mi?'*

Bu soruyu veriye dayalı (data-driven) yöntemlerle yanıtlayabilmek için sahaya 1.000 adet Lapcat prototipi sürdük ve aylarca telemetri/müşteri senkronizasyon verilerini topladık. Bugün sizlerle, kurduğumuz dinamik altyapının bize sunduğu finansal ve operasyonel içgörüleri paylaşacağız."

---

## BÖLÜM 2: Veri Mimarisi ve Metodoloji (Arka Plan Anlatımı)
**Konuşmacı 2:**
"Analizlere ve görselleştirmelere geçmeden önce kurduğumuz analitik altyapıdan (Data Model) kısaca bahsetmek istiyorum. 
Saha testlerinden ve veritabanından elde edilen ham datalar Power Query kullanılarak ETL sürecinden (Ayıklama, Çevirme, Yükleme) geçirilmiş ve temizlenmiştir.

Power BI'da kurduğumuz ilişkisel veri modelinde 'Yıldız Şema (Star Schema)' prensiplerine sadık kaldık. Operasyonel kayıtları içeren *Tracker Data* ve *Rating Data* gibi (Fact) tablolarımız merkeze alınırken; filtre mekanizmasını yöneten *Pet, Family* ve *Date* (Dimension) tabloları etrafında konumlandırılmıştır. Modeldeki filtreleme yönleri (cross-filter direction) çift yönlü (Both) ayarlanmış ve karmaşık iş metrikleri için DAX (Data Analysis Expressions) diliyle özel ölçekler (Measures) oluşturulmuştur."

---

## BÖLÜM 3: Karşılaştırmalı Performans Analizi (Cats vs. Dogs Sayfası Açılır)
**Konuşmacı 3:** *(Ekranda grafikler gösterilerek)*
"En kritik analizimiz olan Lapcat ve Lapdog ürünlerinin karşılaştırmasına baktığımızda tablonun son derece çarpıcı olduğunu görüyoruz.

1. **Davranışsal Çıktılar (Adım Sayıları KPI):** Lapdog ürünümüzde köpeklerin günlük ortalama adım sayısı 12.000 (12.2K) seviyelerinde güçlü seyrederken, Lapcat prototipini kullanan kedilerde bu sayı sadece 2.800 bandında kalmıştır. Bu durum, mevcut ürün özelliklerinin kedilerin doğasına (yürüyüş rutini) uymadığını açıkça göstermektedir.
2. **Müşteri Memnuniyeti (Rating & Recommendation):** En majör hezimet memnuniyet sekmesindedir. Yıllardır piyasada olan Lapdog tasmalarımız 5 üzerinden ortalama **4.7** gibi harika bir skora sahipken, Lapcat deneyen kullanıcıların ortalama memnuniyeti **1.8**'de kalmıştır. Markayı Tavsiye Oranlarında (NPS) ise köpek sahiplerinin %89'una karşılık, kedi sahiplerinin sadece %11'i ürünü bir başkasına önermektedir.
3. **Trend Dağılımı (Line Chart):** Sayfanın altındaki zaman serisine dikkat ederseniz; köpek ürünlerinin 2018'den bu yana gösterdiği stabil ve yükselen performansa karşın, kedi prototipinin sahaya sürüldüğü 2020 yılındaki veri noktasının (1.8 bandında) dibe vurduğunu net olarak izleyebiliriz."

---

## BÖLÜM 4: Demografik ve Operasyonel Dağılımlar (General Pet Data Sayfası)
**Konuşmacı 4:**
"Müşteri segmentasyonumuzu daha derinden anlamak adına Genel Hayvan Verilerini haritalandırdık.
Ekranda gördüğünüz Coğrafi Analiz (Map Visual), kullanıcılarımızın ve tasmalarımızın ABD genelindeki coğrafi yoğunluğunu göstermektedir. 
Panole eklediğimiz dinamik Slicer (Dilimleyici) sayesinde yöneticilerimiz tek tıkla herhangi bir yılı seçip; o yıla ait en popüler 5 hayvan ırkını, yaş ve cinsiyet dağılımlarını anlık olarak listeleyebilmektedir. Bu veriler hedef kitle optimizasyonu için eşsiz bir değer taşımaktadır."

---

## BÖLÜM 5: Finansal İçgörüler ve Müşteri Profili (Family Data & Drillthrough)
**Konuşmacı 1 veya 2:**
"Son sayfamızda portföyümüzün finansal sağlığına odaklanıyoruz.
Oluşturduğumuz Dağılım Grafiğinde (Scatter Chart) her bir hanemizin yıllık geliri ile evcil hayvana yaptıkları harcamalar arasındaki korelasyon (ilişki) haritalanmıştır. Yüksek gelir segmentinde markamıza olan lojalitenin gücü net bir şekilde görülebiliyor. Yüksek gelirli müşterilerin harcamaları ve sadakati paralel artıyor.

*(ŞOV KISMI BURADA UYGULAMALI YAPILIR)*
Bu noktada geliştirdiğimiz panelin dinamik gücünü gösteren **Drillthrough (Detaya Git)** mimarisinden bahsetmek istiyoruz. 
Diyelim ki tabloda gördüğümüz ve harcaması spesifik olarak yüksek olan 'Smith Ailesi' (veya herhangi bir aile) ile ilgili derinlemesine bilgiye ihtiyacımız var. İsmine **sağ tıklayarak Detaya Git dediğimizde**...
*(Otomatik olarak o gizli Detail sayfasına geçiş yapılır)*
...Power BI bizi doğrudan ailenin bireysel mikro-profil CRM sayfasına yönlendirmektedir. Kaç hayvan besledikleri, sistemimize girdikleri doğrudan müşteri yorumları ve memnuniyet anketleri saniyeler içinde önümüze dökülmektedir." *(Tekrar CTRL+Geri Oku yaparak ana sayfaya dönülür).*

---

## BÖLÜM 6: Stratejik Yönetim Kararı ve Kapanış
**Konuşmacı 3 veya 4:**
"Özetle, veri analitiği birimimiz Lapcat projesi özelinde aşağıdaki stratejik sonuca varmıştır:

Lapdog, şirketimizin 'Nakit İneği (Cash Cow)' kalemi olarak son derece sağlıklı büyümektedir ve pazarlama bütçesi asıl oraya aktarılmalıdır. Ancak **Lapcat projesi bu haliyle piyasaya kesinlikle sürülmemelidir.** 

Kedi sahiplerinin akıllı tasmadan beklentileri (adım saymak yerine ev içi konum, kalp ritmi veya uyku süresi sensörleri) köpek sahiplerinden tamamen farklıdır. Muhtemel bir pazarlama fiyaskosu ve marka devalüasyonundan (güven kaybı) kaçınmak adına; Lapcat lansmanının mevcut haliyle iptal edilmesini, Ar-Ge birimimizin ürünü 'kedi doğasına' uygun donanımlarla sıfırdan tasarlamasını tavsiye ediyoruz.

Bizleri dinlediğiniz için teşekkür ederiz. Panelle veya aldığımız aksiyonlarla ilgili sorularınız varsa yanıtlamaktan memnuniyet duyarız."
