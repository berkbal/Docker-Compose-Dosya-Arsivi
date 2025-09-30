# PowerDNS Docker Compose Kurulumu

Bu repo, PowerDNS ve PowerDNS-Admin'i Docker Compose ile hızlıca ayağa kaldırmak için gerekli dosyaları içerir.

## Nasıl Kullanılır?

1.  `.env.example` dosyasını kopyalayarak `.env` adında yeni bir dosya oluşturun.
2.  `.env` dosyasındaki değişkenleri kendinize göre düzenleyin. 
3.  Aşağıdaki komut ile container'ları ayağa kaldırın:

    ```bash
    docker-compose up -d
    ```

## PowerDNS-Admin Kurulumu

PowerDNS-Admin arayüzüne ilk kez girdiğinizde, sizden bir PowerDNS sunucusu eklemenizi isteyecektir. Ayarları yaparken API Endpoint olarak `http://powerdns:8081` adresini ve API Key olarak `.env` dosyanızdaki `PDNS_api_key` değerini kullanabilirsiniz. Container'lar aynı ağda olduğu için IP adresi yerine container adını (`powerdns`) kullanabilirsiniz.

## Servisler

-   `powerdns`: PowerDNS sunucusu.
-   `db`: PostgreSQL veritabanı.
-   `powerdns-admin`: PowerDNS için web arayüzü.


