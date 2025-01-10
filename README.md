# E-Commerce Microservices Project

Bu proje, modern yazılım geliştirme tekniklerini ve en iyi uygulamaları kullanarak bir **e-ticaret mikroservis mimarisi** oluşturmayı hedeflemektedir. 
Gerçek bir e-ticaret senaryosu üzerinden, farklı kullanıcı türleri (misafir, kayıtlı kullanıcı, admin) için detaylı yetkilendirme ve yönetim senaryoları uygulanmıştır.

## Proje Özeti

Proje, birden fazla mikroservis kullanılarak geliştirilmiştir ve aşağıdaki teknolojileri ve tasarım desenlerini içermektedir:

- **Redis**: Hızlı veri saklama ve önbellekleme.
- **Dapper**: Hafif ORM aracı ile veritabanı işlemleri.
- **Docker**: Konteyner tabanlı yapılandırma ve dağıtım.
- **MongoDB**, **PostgreSQL**, **MSSQL**, **SQLite**: Çoklu veritabanı desteği.
- **Google Drive Entegrasyonu**: Fotoğraf yükleme ve depolama.
- **Identity Server**: Kimlik doğrulama ve yetkilendirme.
- **Api Gateway (Ocelot)**: Mikroservisler arasında merkezi bir geçit.
- **Swagger**: API dokümantasyonu.
- **Onion Architecture**: Katmanlı mimari.
- **CQRS Design Pattern**: Komut ve sorgu ayrımı.
- **Mediator Design Pattern**: Bağımsız bileşenler arası iletişim.
- **Repository Design Pattern**: Veri erişimi için soyutlama.
- **JWT Authentication**: Kimlik doğrulama ve yetkilendirme.
- **SignalR**: Gerçek zamanlı bildirimler.
- **Rapid API**: Harici API entegrasyonu.
- **Postman** ve **Ajax** ile test ve istemci iletişimi.

## Özellikler

- **Yetkilendirme Senaryoları**: 
  - Misafir kullanıcılar için sınırlı erişim.
  - Kayıtlı kullanıcılar için genişletilmiş özellikler.
  - Admin kullanıcılar için yönetim paneli.
- **Mikroservis Mimari**: 
  - Her bir servis bağımsız çalışabilir.
  - Servisler birbirleriyle API Gateway üzerinden iletişim kurar.
- **Tam E-Ticaret Deneyimi**:
  - Ürün listeleme, sipariş oluşturma ve kullanıcı yönetimi.

## Kurulum

 1. **Depoyu Klonlayın**:
   ```bash
   git clone https://github.com/username/ecom-micro.git
   cd ecom-micro
   ```

2. **Docker ile Çalıştırın**:
   Proje konteynerlerde çalışacak şekilde yapılandırılmıştır. Docker'ın kurulu olduğundan emin olun ve aşağıdaki komutu çalıştırın:
   ```bash
   docker-compose up --build
   ```

3. **Servisleri Test Edin**:
   Postman veya Swagger kullanarak servisleri test edebilirsiniz. API Gateway üzerinden tüm mikroservislere erişim sağlayabilirsiniz.

## Proje Mimarisi

Proje aşağıdaki gibi tasarlanmıştır:

- **API Gateway**: Tüm mikroservislere merkezi giriş noktası.
- **Kimlik Doğrulama Servisi**: Kullanıcı oturumları ve yetkilendirme işlemleri.
- **Ürün Yönetimi Servisi**: Ürün listeleme ve detay bilgileri.
- **Sipariş Servisi**: Sipariş oluşturma ve yönetimi.
- **Kullanıcı Yönetimi Servisi**: Kullanıcı kayıt ve oturum işlemleri.

## Teknoloji Yığını

- **Backend**: ASP.NET Core
- **Frontend**: AJAX/HTML
- **Veritabanı**: PostgreSQL, MongoDB, MSSQL
- **Konteynerizasyon**: Docker
- **Gerçek Zamanlı Bildirimler**: SignalR



Bu README dosyası, projeyi detaylıca açıklarken, izlenilen eğitimi belli etmeden kendi geliştirdiğiniz bir proje izlenimi verecek şekilde düzenlenmiştir.
