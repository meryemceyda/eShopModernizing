# TÜBİTAK 2209-B Araştırma Önerisi Formu (Taslak İçerik)

*(Bu taslağı hocanın verdiği asıl Word/PDF formuna kopyala-yapıştır yaparak aktarabilirsiniz.)*

### 1. Amaç ve Hedefler
**Amaç:** Bu projenin temel amacı, geleneksel monolitik mimariyle (legacy) yazılmış kurumsal uygulamaların, sürdürülebilirlik, ölçeklenebilirlik ve bakım kolaylığı sağlamak amacıyla modern bulut (cloud) ve konteyner (container) tabanlı mimarilere taşınması süreçlerini analiz etmek ve bu geçişi `eShopModernizing` referans uygulaması üzerinden uygulamalı olarak göstermektir.
**Hedefler:**
1. Monolitik bir .NET uygulamasının Docker kullanılarak konteynerize edilmesi.
2. Uygulama bileşenlerinin (Frontend, Backend, Veritabanı) birbirinden izole çalışabilir hale getirilmesi.
3. Bulut mimarisine geçişte karşılaşılan "vendor lock-in", veri bütünlüğü ve güvenlik zorluklarına çözüm önerileri sunulması.

### 2. Yenilikçi Yönü ve Teknolojik Değeri
Geleneksel yazılım modernizasyon projeleri genellikle sistemin tamamen durdurularak baştan yazılmasını (Big Bang Rewrite) hedefler ki bu büyük şirketler için maliyetli ve risklidir. Bu projenin yenilikçi yönü, "Strangler Fig" (Aşamalı Boğma) yaklaşımını kullanarak, legacy bir .NET sisteminin parçalar halinde modern .NET Core ve Docker ekosistemine entegre edilmesini modellemesidir. Mevcut kod tabanını çöpe atmadan teknolojik değer katmak, sektördeki en kritik ve sürdürülebilir mühendislik çözümüdür.

### 3. Yöntem
Araştırma kapsamında karma (hibrit) bir yöntem izlenecektir:
*   **Literatür ve Mimar Analizi:** Öncelikle Microsoft tarafından yayınlanan "eShopModernizing" orijinal kaynak kodları tersine mühendislik (reverse engineering) ve mimari inceleme yöntemleriyle analiz edilecektir.
*   **Konteynerleştirme Adımı:** Geleneksel WCF ve ASP.NET WebForms/MVC yapıları analiz edilerek, `Dockerfile` ve `docker-compose.yml` dosyaları yazılacaktır.
*   **Test ve Kıyaslama:** Sistemin legacy (eski) versiyonu ile konteynerize edilmiş modern versiyonu; başlatma süresi, kaynak tüketimi ve ölçeklenebilirlik açısından stres testlerine tabi tutularak karşılaştırılacaktır.

### 4. İş-Zaman Çizelgesi
*(Formdaki tabloya şu maddeleri haftalara bölerek yazabilirsiniz)*
*   **1.-2. Hafta:** Proje organizasyonu, literatür araştırması ve repository'nin çatallanması (fork).
*   **3.-4. Hafta:** Orijinal kod tabanının analizi ve bağımlılık haritasının çıkartılması.
*   **5.-6. Hafta:** Veritabanı ve servislerin birbirinden ayrıştırılarak Dockerize edilmesi.
*   **7.-8. Hafta:** Lokal testlerin yapılması, metriklerin toplanması ve final raporunun/sunumun yazılması.

### 5. Risk Yönetimi ve B Planları
*   **Risk 1:** Konteynerleştirme sırasında uyumsuz kütüphane sorunları (Dependency Hell) çıkması.
    *   **B Planı:** Sistemin tamamını modernize etmek yerine sadece Web API katmanını modernize edip, veritabanını legacy olarak bırakacak bir hibrit mimari yapılandırmak.
*   **Risk 2:** Ekip içi görevlerde gecikme veya bilgisayar performans yetersizliği.
    *   **B Planı:** Lokal Docker Desktop yerine bulut tabanlı ücretsiz eğitim sunucularını (AWS Educate, GitHub Codespaces) kullanmak.

### 6. Araştırma Olanakları
Çalışma, takım üyelerinin şahsi bilgisayarları, GitHub (Versiyon Kontrol Sistemi), GitHub Projects (Proje Yönetimi) ve açık kaynaklı Docker / .NET ekosistem araçları kullanılarak yürütülecektir. 

### 7. Sanayi Odaklı Çıktılar ve Yaygın Etki
Modernizasyon, günümüzde bankacılık, sigortacılık ve e-ticaret sanayisinin en büyük IT problemidir. Bu projenin çıktısı, şirketlere "eski sistemlerinizi durdurmadan nasıl yenilersiniz" sorusu için bir rehber (proof of concept) niteliği taşıyacaktır. Bu sayede yazılım sanayisinde bakım maliyetlerini düşürecek uygulanabilir bir metodoloji ortaya konulacaktır.
