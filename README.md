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


# 🚀 Huawei DevOps Bootcamp Project

This project is a set of microservice-based applications developed as part of the Huawei DevOps Bootcamp. Dockerfiles have been created for different services, each designed to run in its own container. The main goal is to learn and apply modern DevOps and container technologies.

---

## 📦 Contents

- **paymentservice** 💳: A microservice managing payment operations. Built on Node.js and communicates via gRPC.
- **cartservice** 🛒: A service managing user shopping carts.
- **currencyservice** 💱: A service handling currency exchange rates and conversions.
- **productcatalogservice** 📋: A service managing product catalogs.

Each service has its own Dockerfile and can be built and deployed independently.

---

## ✨ Project Features

- **Microservice architecture** 🏗️: Each service focuses on its specific responsibility.
- **Docker containers** 🐳: Separate Docker images created for each service, runnable as containers.
- **gRPC communication** ⚡: Fast and type-safe communication between services.
- **Alpine Linux based images**

## Setup and Running

### Requirements

- Docker installed
- Node.js (for development)
- Git

### Clone the project

```bash
git clone https://github.com/zeynepatceken/Huawei-Devops-Bootcamp-Project.git
cd Huawei-Devops-Bootcamp-Project/src/paymentservice
