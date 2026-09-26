# Açıklamalı Kaynak Listesi (Literatür Taraması)

Sunumunuzda yer alması gereken **en az 5 adet akademik veya teknik kaynağın** açıklamalı listesi aşağıdadır:

### 1. Fowler, M. (2004). "Strangler Fig Application"
*   **Kaynak Türü:** Teknik / Mimari Makale (Martin Fowler Blog)
*   **Proje Açısından Önemi (İlişki Notu):** Bu makale, projemizin temel modernizasyon felsefesini oluşturmaktadır. Makale, eski (legacy) sistemlerin tamamen yıkılıp yeniden yapılması yerine, yeni sistemin eski sistemin etrafında kademeli olarak örülmesi (boğma inciri taktiği) yöntemini anlatır. Biz de eShop projesinde bileşenleri bu yaklaşımla teker teker modernize edeceğiz.

### 2. Richardson, C. (2018). "Microservices Patterns: With Examples in Java"
*   **Kaynak Türü:** Akademik / Teknik Kitap (Manning Publications)
*   **Proje Açısından Önemi (İlişki Notu):** Kitap her ne kadar Java diliyle yazılmış olsa da, monolitik bir uygulamanın mikroservislere parçalanırken veritabanlarının nasıl ayrılacağı (Decompose by Subdomain) desenlerini detaylandırır. Projemizde geleneksel .NET mimarisini ayırırken buradaki "Database per service" kalıbını referans alacağız.

### 3. Microsoft Architecture (2023). "Modernize existing .NET applications with Cloud and Windows Containers"
*   **Kaynak Türü:** Resmi Teknoloji Dokümantasyonu (Microsoft Learn)
*   **Proje Açısından Önemi (İlişki Notu):** Projemizin ana ekseni olan eShopModernizing için Microsoft'un yayınladığı temel teknik rehberdir. Geleneksel WCF ve WebForms yapılarının doğrudan Windows Container'ları içine nasıl alınacağını ve bulut tabanlı bir DevOps döngüsünün nasıl kurulacağını gösterdiği için başvuru kaynağımızdır.

### 4. Pahl, C. (2015). "Containerization and the PaaS Cloud"
*   **Kaynak Türü:** Akademik Makale (IEEE Cloud Computing)
*   **Proje Açısından Önemi (İlişki Notu):** Projemizin "Neden Container kullanmalıyız?" sorusuna bilimsel altyapı sağlar. Makale, donanım sanallaştırması (Sanal Makineler - VM) ile işletim sistemi sanallaştırması (Konteynerler - Docker) arasındaki performans ve kaynak tüketimi farklarını bilimsel verilerle ortaya koyar.

### 5. Jamshidi, P., et al. (2013). "Microservices: The Journey So Far and Challenges Ahead"
*   **Kaynak Türü:** Akademik Makale (IEEE Software)
*   **Proje Açısından Önemi (İlişki Notu):** Sunumdaki "Problem Tanımı" kısmını desteklemek için seçilmiştir. Makale, monolitik yazılımların kurumsal ölçekte yarattığı "bakım kabusu" (maintenance nightmare) durumunu incelemekte ve modernizasyon sırasında karşılaşılan veri tutarlılığı risklerini (Risk Yönetimi planımız için) detaylandırmaktadır.
