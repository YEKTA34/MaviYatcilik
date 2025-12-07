# ⚓ Mavi Yatçılık Kurumsal Web Sitesi Proje Özeti (README)

Bu dosya, üniversite projesi olarak geliştirilen Mavi Yatçılık web sitesinin teknik detaylarını ve uygulanan zorunlu proje isterlerini özetler.

## 1. Giriş ve Temel Hedefler

Bu çalışma, lüks yat kiralama sektörüne yönelik modern, responsive (duyarlı) tasarım teknikleri kullanılarak geliştirilmiştir. Proje, açık kaynaklı **"WaterBoat"** şablonunu temel almış ve sektörel ihtiyaçlara göre kapsamlı bir şekilde özelleştirilmiştir.

### 🎯 Temel Hedefler

* **Lüks yat kiralama** hizmetlerini dijital ortamda profesyonel bir kurumsal kimlikle sunmak.
* **Masaüstü, tablet ve mobil** cihazlarda kusursuz çalışan **(Responsive)** bir yapı oluşturmak.
* Sıfırdan kodlama yerine endüstri standardı olan **Framework (Bootstrap)** yapısını analiz edip özelleştirerek geliştirme hızını artırmak.
* **Chart.js** entegrasyonu ile istatistiksel verileri (Filo dağılımı, memnuniyet) görselleştirmek.

---

## 2. Materyal ve Yöntem

### 🛠 Kullanılan Teknolojiler

Projenin geliştirilmesinde **W3C standartlarına uygun** teknolojiler kullanılmıştır:

* **HTML5 & CSS3:** İskelet yapı ve stil düzenlemeleri.
* **Bootstrap 5:** "Mobile-First" yaklaşımını benimseyen ana Framework. Grid sistemi, içeriklerin farklı cihazlarda yeniden hizalanmasını sağlamıştır.
* **JavaScript (Chart.js):** Dinamik davranışlar, Modal pencerelerin tetiklenmesi ve istatistiksel verilerin görselleştirilmesi.

### 🌐 Şablon Seçimi ve Yapılandırma

**WaterBoat** şablonunun seçilmesindeki temel kriterler şunlardır:

* **Responsive Uyumluluk:** Farklı ekran çözünürlüklerinde bozulmadan çalışabilmesi.
* **Özelleştirilebilir Yapı:** CSS sınıflarının modüler olması sayesinde stil düzenlemelerinin kolay yapılabilmesi.

---

## 3. Uygulama Detayları ve Özellikler

### 3.1. Yönetici (Admin) Paneli Simülasyonu

Projenin teknik isterleri doğrultusunda, **sunucu taraflı kodlama (Backend) yapılmaksızın**, sadece ön yüz (Frontend) teknolojileri kullanılarak bir **"Yönetici Paneli"** arayüzü (`admin-panel.html`) tasarlanmıştır:

* **CMS İskeleti:** Yat Ekleme/Düzenleme form alanları ve dosya yükleme (PDF/Word) simülasyonu yapan butonlar yer almaktadır.
* **Erişim:** Admin Paneli girişi, sitenin navigasyonundan ayrılmış ve **Header Top** bölümüne konumlandırılmıştır.

### 3.2. Duyurular ve Kampanya Yönetimi

* **Modal Pencere Kullanımı:** Kullanıcı etkileşimini artırmak amacıyla, duyuru detayları için sayfa yenilemesi gerektirmeyen **Bootstrap Modal** yapısı kullanılmıştır.
* **Arşiv Sistemi:** Tüm duyuruların **en yeniden en eskiye doğru sıralandığı** ayrı bir listeye erişim sağlayan **"Tüm Duyurulara Git"** düğmesi entegre edilmiştir.

### 3.3. İstatistiksel Grafikler

Kurumsal güveni artırmak amacıyla **Chart.js** kütüphanesi kullanılarak istatistiksel veriler görselleştirilmiştir:

* **Veriler:** Filo Dağılımı (Doughnut), Müşteri Memnuniyeti (Bar) ve Rota Talebi (Line) gibi zorunlu veriler sergilenmiştir.
* **Optimizasyon:** Bar Grafiği, verilerin doğru oranlanması için Y ekseni `min: 0` olarak ayarlanarak performansı optimize edilmiştir.

---

## 4. Karşılaşılan Zorluklar ve Çözümleri

Proje geliştirme sürecinde karşılaşılan temel teknik zorluklar ve bu zorluklara getirilen çözümler:

| Zorluk Alanı | Çözüm |
| :--- | :--- |
| **Dil ve Tipografi Uyumsuzlukları** | İngilizce şablonun Türkçeleştirilmesi sonucu oluşan taşmalar, **CSS dosyasındaki font-size** değerleri optimize edilerek ve menü boşlukları yeniden düzenlenerek giderilmiştir. |
| **Modal Açılışında Sayfa Kayması** | Duyuruya tıklanınca sayfanın otomatik olarak üste kayması problemi, linklerdeki `href="#"` etiketi yerine **`href="javascript:void(0)"`** kodu kullanılarak çözülmüştür. |
| **Buton Hizalama (Duyurular)** | "Tüm Duyurulara Git" butonunun CSS çakışmaları nedeniyle sola kayması. | Butonun kapsayıcı yapısı sadeleştirilerek ve **`text-center`** sınıfı ile zorla ortalama sağlanmıştır. |
| **Bar Grafiği Görünürlüğü** | Bar Grafiği'nde bazı verilerin görünmemesi. | Chart.js kodunda Y ekseni **`min: 0`** olarak ayarlanmış ve grafiğin **sıfırdan başlaması** zorlanarak verilerin doğru görüntülenmesi sağlanmıştır. |

---

## 5. Canlı Sunucu ve Kaynakça

### 🚀 Canlı Sunucu Entegrasyonu

Geliştirilen proje, versiyon kontrol sistemi olan **Git** kullanılarak GitHub platformuna yüklenmiştir. **"GitHub Pages"** hizmeti aktif edilerek web sitesi canlı sunucu üzerinde yayınlanmış ve genel erişime açılmıştır.

### 📚 Kaynakça

Bu projede kullanılan temel kaynaklar ve dokümantasyonlar:

* [1] ThemeWagon. **"WaterBoat – Free HTML/CSS Template."**
    *Erişim adresi: https://themewagon.com/themes/free-bootstrap-4-html5-responsive-transportation-website-template-waterboat/*
* [2] Bootstrap Team. **"Bootstrap 5 Documentation."**
    *Erişim adresi: https://getbootstrap.com/docs/5.0/getting-started/introduction/*
* [3] Chart.js. **"Chart.js Documentation."**
    *Erişim adresi: https://www.chartjs.org/docs/latest/*
* [4] Kurumsal Veri Modeli (Örnek Alınan Yapı): Kocaeli Üniversitesi. **"Sayılarla KOÜ."**
