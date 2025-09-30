# PowerDNS Docker Compose Kurulumu

Bu repo, PowerDNS ve PowerDNS-Admin'i Docker Compose ile hızlıca ayağa kaldırmak için gerekli dosyaları içerir.

## Nasıl Kullanılır?

1.  `.env.example` dosyasını kopyalayarak `.env` adında yeni bir dosya oluşturun.
2.  `.env` dosyasındaki değişkenleri kendinize göre düzenleyin. 
3.  Aşağıdaki komut ile container'ları ayağa kaldırın:

    ```bash
    docker-compose up -d
    ```





## Servisler

-   `powerdns`: PowerDNS sunucusu.
-   `db`: PostgreSQL veritabanı.
-   `powerdns-admin`: PowerDNS için web arayüzü.


