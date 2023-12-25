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


#### <a>Настройка R01_SBP:</a>


#### <a>Настройка R01_SVL:</a>


#### <a>Настройка R01_HKI:</a>


#### <a>Настройка R01_LND:</a>

#### <a>Настройка R01_LBN:</a>

