University: [ITMO University](https://itmo.ru/ru/)  
Faculty: [FICT](https://fict.itmo.ru)  
Course: [Introduction in routing](https://github.com/itmo-ict-faculty/introduction-in-routing)  
Year: 2023/2024  
Group: K33202  
Author: Dashkovskaya Dana 
Lab: Lab2 
Date of create: 1.11.2023  
Date of finished: 27.11.2023  

## Лабораторная работ №2 "Эмуляция распределенной корпоративной сети связи, настройка статической маршрутизации между филиалами"    
## <a> Ход работы</a>  
#### <a> Построение сети связи</a>  
[Uploading marsh2.yaml…]()
name: lab2

mgmt:
  network: statics
  ipv4-subnet: 172.30.20.0/24

topology:
  nodes:
    R01.MSK:
      kind: vr-ros
      image: vrnetlab/vr-routeros:6.47.9
      mgmt-ipv4: 172.30.20.13

    R01.BRL:
      kind: vr-ros
      image: vrnetlab/vr-routeros:6.47.9
      mgmt-ipv4: 172.30.20.14

    R01.FRT:
      kind: vr-ros
      image: vrnetlab/vr-routeros:6.47.9
      mgmt-ipv4: 172.30.20.15

    PC1:
      kind: vr-ros
      image: vrnetlab/vr-routeros:6.47.9
      mgmt-ipv4: 172.30.20.16

    PC2:
      kind: vr-ros
      image: vrnetlab/vr-routeros:6.47.9
      mgmt-ipv4: 172.30.20.17

    PC3:
      kind: vr-ros
      image: vrnetlab/vr-routeros:6.47.9
      mgmt-ipv4: 172.30.20.18

#### <a> Сборка и построение происходит также как и в прошлой работе</a> 
![граф](https://github.com/DanaDaschoca/2023_2024-introduction_in_routing-k33202-Dashkovskaya/assets/90696514/210f5906-3fef-4a56-89cc-43bab7996410)
#### <a> Далее мы используем команду sudo ssh admin@clab-lab2-Ro1.MSK с помощью этой команды мы настраиваем конфигурацию </a>
#### <a> Чтобы посмотреть конфигурацию используем команду export </a>
#### <a> Настройка R01.MSK</a> 
![R01 MSK](https://github.com/DanaDaschoca/2023_2024-introduction_in_routing-k33202-Dashkovskaya/assets/90696514/6b22a089-b4a4-4b19-a0d7-08a2352519a6)
#### <a> Настройка R01.FRT</a> 
![R01 FRT](https://github.com/DanaDaschoca/2023_2024-introduction_in_routing-k33202-Dashkovskaya/assets/90696514/3893e0c2-0699-446e-97b8-4a7fc400bfc5)
#### <a> Настройка R01.BRL</a> 
![R01 BRL](https://github.com/DanaDaschoca/2023_2024-introduction_in_routing-k33202-Dashkovskaya/assets/90696514/83fb1a97-1db7-4f4f-baf8-cfea26630585)
#### <a> Настройка PC1</a> 
![PC1](https://github.com/DanaDaschoca/2023_2024-introduction_in_routing-k33202-Dashkovskaya/assets/90696514/3e38d539-650f-4f59-b313-32f1f63c27fb)
#### <a> Настройка PC2</a> 
![PC2](https://github.com/DanaDaschoca/2023_2024-introduction_in_routing-k33202-Dashkovskaya/assets/90696514/acd1d299-b8bd-45ef-b456-df0b4514e387)
#### <a> Настройка PC3</a>    
![PC3](https://github.com/DanaDaschoca/2023_2024-introduction_in_routing-k33202-Dashkovskaya/assets/90696514/3c1b4ce9-2ec9-469a-bbb2-48b47a397e25)

#### <a> Результаты пингов:</a> 
#### <a> Для этого заходим в каждый PC1 PC2 PC3  и вводим ping </a> 
![ping 1](https://github.com/DanaDaschoca/2023_2024-introduction_in_routing-k33202-Dashkovskaya/assets/90696514/db249821-bdf4-42a6-83f3-eba67eaf9901)
![ping 2](https://github.com/DanaDaschoca/2023_2024-introduction_in_routing-k33202-Dashkovskaya/assets/90696514/be98a355-06b4-4ca4-92df-361a24ba4f9f)
![ping 3](https://github.com/DanaDaschoca/2023_2024-introduction_in_routing-k33202-Dashkovskaya/assets/90696514/51181551-4f60-4e4c-9227-44c5727a4d82)

