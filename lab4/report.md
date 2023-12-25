University: [ITMO University](https://itmo.ru/ru/)  
Faculty: [FICT](https://fict.itmo.ru)  
Course: [Introduction in routing](https://github.com/itmo-ict-faculty/introduction-in-routing)  
Year: 2023/2024  
Group: K33202 
Author: Dashkovskaya Dana  
Lab: Lab4  
Date of create: 16.12.2023  
Date of finished: 24.12.2023 
## Лабораторная работ №4 "Эмуляция распределенной корпоративной сети связи, настройка iBGP, организация L3VPN, VPLS" 
## <a>Ход работы</a>
* С помощью данной команды создаем папку: 
--- touch marsh3.clab.yaml---
* В файл записываем построение сети 
* С помощью данной команды собираем Containerlab:
--- sudo clab deploy marsh4.clab.yaml---
![image](https://github.com/DanaDaschoca/2023_2024-introduction_in_routing-k33202-Dashkovskaya/assets/90696514/0cb68e08-07be-4dab-9bb5-ded73d6edd8d)
* С помощью данной команды строим нашу сеть:
--- sudo clab graph ---
  ![image](https://github.com/DanaDaschoca/2023_2024-introduction_in_routing-k33202-Dashkovskaya/assets/90696514/1692b340-c288-4ba8-aeb4-2c5ec911ed11)
![image](https://github.com/DanaDaschoca/2023_2024-introduction_in_routing-k33202-Dashkovskaya/assets/90696514/0012111e-2e6d-433a-a7a6-bdf37b86260a)
С помощью данной команды входим в настроуку интерфейса: 
--- sudo ssh admin@clab-lab4-...---
  ### <a>Текст конфигураций для каждого сетевого устройства</a>
#### <a>Настройка R01_NY:</a> 
![image](https://github.com/DanaDaschoca/2023_2024-introduction_in_routing-k33202-Dashkovskaya/assets/90696514/0029a1d7-0039-4164-ac3e-b0486adc74db)

#### <a>Настройка R01_SBP:</a>
![image](https://github.com/DanaDaschoca/2023_2024-introduction_in_routing-k33202-Dashkovskaya/assets/90696514/573538d2-f590-431f-b073-96d7a348f04e)

#### <a>Настройка R01_SVL:</a>
![image](https://github.com/DanaDaschoca/2023_2024-introduction_in_routing-k33202-Dashkovskaya/assets/90696514/c0818883-526d-4f95-b234-6fb6c86e080c)

#### <a>Настройка R01_HKI:</a>
![image](https://github.com/DanaDaschoca/2023_2024-introduction_in_routing-k33202-Dashkovskaya/assets/90696514/235673f2-90d6-4821-8a81-1b226216e7f6)
#### <a>Настройка R01_LND:</a>
![image](https://github.com/DanaDaschoca/2023_2024-introduction_in_routing-k33202-Dashkovskaya/assets/90696514/175c78f4-9595-4742-818f-c8b15fd181c1)

#### <a>Настройка R01_LBN:</a>
![image](https://github.com/DanaDaschoca/2023_2024-introduction_in_routing-k33202-Dashkovskaya/assets/90696514/ad9f3c74-9339-4598-9dc2-7178b5f2ce0e)
### <a>Результаты пингов. Проверка связности VRF:</a> 
![image](https://github.com/DanaDaschoca/2023_2024-introduction_in_routing-k33202-Dashkovskaya/assets/90696514/d71977dd-cdfd-42fe-a290-a67e447f6c99)
![image](https://github.com/DanaDaschoca/2023_2024-introduction_in_routing-k33202-Dashkovskaya/assets/90696514/5815794f-ab16-4029-9469-ed2bbe213356)
![image](https://github.com/DanaDaschoca/2023_2024-introduction_in_routing-k33202-Dashkovskaya/assets/90696514/9a62a2c5-366c-4716-9e2d-b4df7e8c234d)
#### <a>Настройка PC1:</a> 
![image](https://github.com/DanaDaschoca/2023_2024-introduction_in_routing-k33202-Dashkovskaya/assets/90696514/15ddf711-929d-4c85-acae-5e82ae091626)
#### <a>Настройка PC2:</a>  
![image](https://github.com/DanaDaschoca/2023_2024-introduction_in_routing-k33202-Dashkovskaya/assets/90696514/06c2aa60-edc1-4d74-83d2-a7d3dc2b8494)

#### <a>Настройка PC3:</a> 
![image](https://github.com/DanaDaschoca/2023_2024-introduction_in_routing-k33202-Dashkovskaya/assets/90696514/ae42b069-ec21-4088-bd78-88ce5a3179df)

#### <a>Настройка R01_SVL:</a>  
![image](https://github.com/DanaDaschoca/2023_2024-introduction_in_routing-k33202-Dashkovskaya/assets/90696514/0c453b63-76ca-4de4-a9a3-ffe8977cfdf6)

#### <a>Настройка R01_NY:</a> 
![image](https://github.com/DanaDaschoca/2023_2024-introduction_in_routing-k33202-Dashkovskaya/assets/90696514/891cf671-65a0-408d-a4ae-47993487eea3)

#### <a>Настройка R01_SPB:</a>  
![image](https://github.com/DanaDaschoca/2023_2024-introduction_in_routing-k33202-Dashkovskaya/assets/90696514/067b178e-09ec-4a2e-bedc-60e3bab85315)

### <a>Результаты пингов.</a>  
![image](https://github.com/DanaDaschoca/2023_2024-introduction_in_routing-k33202-Dashkovskaya/assets/90696514/9a734ad5-a0c6-406a-9909-cfdec323519f)
![image](https://github.com/DanaDaschoca/2023_2024-introduction_in_routing-k33202-Dashkovskaya/assets/90696514/3d9c02e7-fe8c-4f30-86e7-f3e5e2fcaa1f)
![image](https://github.com/DanaDaschoca/2023_2024-introduction_in_routing-k33202-Dashkovskaya/assets/90696514/0d41dbcf-ac96-4c81-8012-7dd7710120a0)
