![image](https://github.com/user-attachments/assets/c28faf2b-7127-4d2f-98d0-954c095ebe1f)
| Service                                            | Language      |
| ---------------------------------------------------| ------------- | 
| frontend                                           | Go            | 
| cartservice                                        | C#            | 
| productcatalogservice                              | Go            | 
| currencyservice                                    | Node.js       |   
| paymentservice                                     | Node.js       | 
| shippingservice                                    | Go            | 
| emailservice                                       | Python        | 
| checkoutservice                                    | Go            | 
| recommendationservice                              | Python        |
| loadgenerator                                      | Python/Locust | 


# Huawei DevOps Bootcamp Project

Bu proje, Huawei DevOps Bootcamp kapsamında geliştirilen mikroservis tabanlı bir uygulama setidir. Projede farklı servisler için Dockerfile’lar hazırlanmış, her servis kendi konteynerinde çalışmak üzere tasarlanmıştır. Amaç, modern DevOps ve konteyner teknolojilerini öğrenmek ve uygulamak üzerine yoğunlaşmaktır.

---

## İçerik

- **paymentservice**: Ödeme işlemlerini yöneten mikroservis. Node.js tabanlıdır ve gRPC protokolü üzerinden iletişim sağlar.
- **cartservice**: Kullanıcı sepeti işlemlerini yöneten servis.
- **currencyservice**: Döviz kurları ve para birimi dönüşümlerini yöneten servis.
- **productcatalogservice**: Ürün kataloglarını yöneten servis.
  ...
  
Her servisin kendi Dockerfile dosyası vardır ve bağımsız olarak build edilip deploy edilebilir.

---

## Proje Özellikleri

- **Mikroservis mimarisi**: Her servis kendi sorumluluğuna odaklanır.
- **Docker container**: Her servis için ayrı Docker image’ları oluşturulmuş ve container olarak çalıştırılabilir.
- **gRPC iletişimi**: Servisler arası hızlı ve tip güvenli iletişim.
- **Alpine Linux tabanlı imajlar**: Hafif ve güvenli base image kullanımı.
- **DevOps uygulamaları için uygun yapı**: CI/CD pipeline ve Kubernetes gibi platformlara entegrasyon için hazır.

---

## Kurulum ve Çalıştırma

### Gereksinimler

- Docker yüklü olmalı
- Node.js (geliştirme için)
- Git

### Projeyi klonlama

```bash
git clone https://github.com/zeynepatceken/Huawei-Devops-Bootcamp-Project.git
cd Huawei-Devops-Bootcamp-Project/src/paymentservice
