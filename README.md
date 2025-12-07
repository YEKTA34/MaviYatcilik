# Mavi Yat Projesi
1. Giriş ve Proje Özeti
Bu çalışmada, modern web tasarım prensipleri ve responsive (duyarlı) tasarım teknikleri kullanılarak lüks yat kiralama sektöründe faaliyet gösteren "Mavi Yatçılık" firması için kurumsal bir web sitesi geliştirilmiştir. Proje kapsamında, açık kaynaklı "WaterBoat" şablonu temel alınmış ve sektörel isterlere göre kapsamlı bir şekilde özelleştirilmiştir. Çalışmanın temel amacı, kullanıcı dostu (UI) ve kullanıcı deneyimi (UX) odaklı bir arayüz sunmak, aynı zamanda sunucu taraflı kodlama gerektirmeyen, ancak görsel olarak fonksiyonel bir İçerik Yönetimi Sistemi (CMS) arayüzü tasarlamaktır.
Temel Hedefler
 Lüks yat kiralama hizmetlerini dijital ortamda profesyonel bir kurumsal kimlikle sunmak.
 Masaüstü, tablet ve mobil cihazlarda kusursuz çalışan (Responsive) bir yapı oluşturmak.
 Sıfırdan kodlama yerine endüstri standardı olan Framework yapısını analiz edip özelleştirerek geliştirme hızını artırmak.
 Chart.js entegrasyonu ile istatistiksel verileri (Filo dağılımı, memnuniyet) görselleştirmek.
2. Materyal ve Yöntem
Kullanılan Teknolojiler
Projenin geliştirilmesinde W3C standartlarına uygun aşağıdaki teknolojiler kullanılmıştır:
 HTML5 & CSS3: İskelet yapı ve stil düzenlemeleri için temel alınmıştır.
 Bootstrap 5: "Mobile-First" yaklaşımını benimseyen Framework olarak kullanılmıştır. Grid sistemi sayesinde içeriklerin farklı cihazlarda yeniden hizalanması sağlanmıştır.
 JavaScript (Chart.js): Dinamik davranışlar ve istatistiksel verilerin görselleştirilmesi için kullanılmıştır.
Şablon Seçimi ve Yapılandırma
WaterBoat şablonunun seçilmesindeki temel kriterler şunlardır:
 Responsive Uyumluluk: Farklı ekran çözünürlüklerinde (masaüstü, tablet, mobil) bozulmadan çalışabilmesi.
 Özelleştirilebilir Yapı: CSS sınıflarının modüler olması sayesinde renk paleti ve tipografinin kolayca değiştirilebilmesi.
 Zengin Bileşenler: İçerisinde hazır slider, hizmet kutuları ve iletişim formları barındırması.
3. Uygulama Detayları ve Özellikler
Arayüz Özelleştirme ve Ürün Tanıtımı
 Lokalizasyon: Orijinal şablon dili İngilizce olup, sektör gereksinimleri doğrultusunda tamamen Türkçe'ye çevrilmiştir.
 Menü Yapısı: Navigasyon, "Yat Modellerimiz" ve "Kurumsal" başlıkları altında hiyerarşik alt menülerle yeniden yapılandırılmıştır.
 Slayt Yapısı: Ana sayfada (index.html), üç ana ürünü (Motor Yat, Gulet, Katamaran) tanıtan otomatik geçişli slider kurgulanmıştır. Slaytlar, ilgili ürünün detay sayfasına yönlendirme yapar.
Yönetici (Admin) Paneli Simülasyonu
Projenin teknik isterleri doğrultusunda, sunucu taraflı kodlama (Backend) yapılmaksızın, sadece ön yüz (Frontend) teknolojileri kullanılarak bir "Yönetici Paneli" arayüzü tasarlanmıştır:
 İçerik Yönetimi: Panelde, Yat Ekleme/Düzenleme form alanları, ve dosya yükleme (upload) simülasyonu yapan butonlar (PDF/Word mantığı) yer almaktadır.
 Tasarım Bütünlüğü: Ana sitenin CSS kütüphanesi admin paneline de entegre edilmiştir.
Duyurular ve Kampanya Yönetimi
 Modal Pencere Kullanımı: Kullanıcı etkileşimini artırmak amacıyla, duyuru detayları için sayfa yenilemesi gerektirmeyen Bootstrap Modal (Açılır Pencere) yapısı kullanılmıştır.
 Arşiv Sistemi: Tüm duyuruların en yeniden en eskiye doğru sıralandığı ayrı bir listeye erişim sağlayan "Tüm Duyurulara Git" düğmesi entegre edilmiştir.
İstatistiksel Grafikler
Kurumsal güveni artırmak amacıyla, Chart.js kütüphanesi kullanılarak istatistiksel grafikler siteye eklenmiştir.
 Veriler: Filo Dağılımı (Doughnut), Müşteri Memnuniyeti (Bar) ve Rota Talebi (Line) gibi zorunlu veriler görselleştirilmiştir.
 Optimizasyon: Bar Grafiği, verilerin doğru oranlanması için Y ekseni min: 0 olarak ayarlanarak performansı optimize edilmiştir.
4. Karşılaşılan Zorluklar ve Çözümleri
Proje geliştirme sürecinde karşılaşılan temel teknik zorluklar ve bu zorluklara getirilen çözümler:
Zorluk Alanı
Çözüm
Dil ve Tipografi Uyumsuzlukları
İngilizce şablonun Türkçeleştirilmesi sonucu oluşan taşmalar, CSS dosyasındaki font-size değerleri optimize edilerek ve menü elemanlarının arasındaki boşluklar (spacing) yeniden düzenlenerek giderilmiştir.
Modal Açılışında Sayfa Kayması
Duyuruya tıklanınca sayfanın otomatik olarak üste kayması problemi, linklerdeki href="#" etiketi yerine href="javascript:void(0)" kodu kullanılarak çözülmüştür.
Buton Hizalama (Duyurular)
"Tüm Duyurulara Git" butonunun CSS çakışmaları nedeniyle sola kayması.
Bar Grafiği Görünürlüğü
Bar Grafiği'nde bazı verilerin görünmemesi.
5- Canlı Sunucu Entegrasyonu
Geliştirilen proje, versiyon kontrol sistemi olan Git kullanılarak GitHub platformuna yüklenmiştir. "GitHub Pages" hizmeti aktif edilerek web sitesi canlı sunucu üzerinde yayınlanmış ve genel erişime açılmıştır.
6-KAYNAKÇA (REFERANSLAR)
Aşağıdaki kaynaklar, web sitesi şablonunun temelini oluşturmak, geliştirme süreci boyunca teknik bilgileri doğrulamak ve zorunlu grafik isterini karşılamak amacıyla kullanılmıştır.
[1] Şablon Kaynağı:
ThemeWagon. "WaterBoat – Free HTML/CSS Template." Erişim adresi: https://themewagon.com/themes/free-bootstrap-4-html5-responsive-transportation-website-template-waterboat/
[2] Framework Belgeleri:
Bootstrap Team. "Bootstrap 5 Documentation." Erişim adresi: https://getbootstrap.com/docs/5.0/getting-started/introduction/
[3] Grafik Kütüphanesi:
Chart.js. "Chart.js Documentation." Erişim adresi: https://www.chartjs.org/docs/latest/
[4] Kurumsal Veri Modeli (Örnek Alınan Yapı):
Kocaeli Üniversitesi. "Sayılarla KOÜ." Erişim adresi: https://www.kocaeli.edu.tr/rakamlarlakou
