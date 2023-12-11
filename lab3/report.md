University: [ITMO University](https://itmo.ru/ru/)  
Faculty: [FICT](https://fict.itmo.ru)  
Course: [Introduction in routing](https://github.com/itmo-ict-faculty/introduction-in-routing)  
Year: 2023/2024  
Group: K33202 
Author: Dashkovskaya Dana  
Lab: Lab3  
Date of create: 1.12.2023  
Date of finished: 11.12.2023  

## Лабораторная работ №3 "Эмуляция распределенной корпоративной сети связи, настройка OSPF и MPLS, организация первого EoMPLS" 
## <a>Ход работы</a>
#### <a>Минимальная теория</a>
* MPLS - это метод маркировки данных через приоритетность данных (скорость увеличивается) 
* OSPF - метод графа, нахождение кратчайшего пути.
* EoMPLS - EoMPLS представляет собой метод передачи Ethernet-фреймов через MPLS-сеть, позволяя нам объединить преимущества обоих протоколов.
#### <a>Первый этап</a>
* С помощью данной команды создаем папку: 
--- touch marsh2.clab.yaml---
* В файл записываем построение сети 
* С помощью данной команды собираем Containerlab:
--- sudo clab deploy marsh2.clab.yaml---
* С помощью данной команды строим нашу сеть:
--- sudo clab graph ---
![image](https://github.com/DanaDaschoca/2023_2024-introduction_in_routing-k33202-Dashkovskaya/assets/90696514/ffb6fde8-376d-406d-a20e-cad16e0bedb3)
#### <a>Второй этап-настройка устройств</a>
С помощью данной команды входим в настроуку интерфейса: 
--- sudo ssh admin@clab-lab3-...---
#### <a>R01.NY</a>
![image](https://github.com/DanaDaschoca/2023_2024-introduction_in_routing-k33202-Dashkovskaya/assets/90696514/47f3929b-3a94-44be-8b86-d74661899119)
#### <a>R01.LDN</a>
![image](https://github.com/DanaDaschoca/2023_2024-introduction_in_routing-k33202-Dashkovskaya/assets/90696514/25cc0487-aa5e-43d5-8b94-67cb87cdf343)
#### <a>R01.HKI</a>
![image](https://github.com/DanaDaschoca/2023_2024-introduction_in_routing-k33202-Dashkovskaya/assets/90696514/c8dee9db-1ce4-48dc-90f6-bfe173846b36)
#### <a>R01.SPB</a>
![image](https://github.com/DanaDaschoca/2023_2024-introduction_in_routing-k33202-Dashkovskaya/assets/90696514/2f28ddcb-b0f7-4763-9a6a-57ee9f7f0001)
#### <a>R01.MSK</a>
![image](https://github.com/DanaDaschoca/2023_2024-introduction_in_routing-k33202-Dashkovskaya/assets/90696514/76b3c84d-536a-40d6-8e27-e199f17f56df)
#### <a>R01.LBN</a>
![image](https://github.com/DanaDaschoca/2023_2024-introduction_in_routing-k33202-Dashkovskaya/assets/90696514/77c79fda-a46b-4e57-ada8-53e69bcf25a1)
#### <a>SGI-Prism</a>
![image](https://github.com/DanaDaschoca/2023_2024-introduction_in_routing-k33202-Dashkovskaya/assets/90696514/eb13837c-2705-4313-a033-79dc528e220a)
#### <a>PC1</a>
![image](https://github.com/DanaDaschoca/2023_2024-introduction_in_routing-k33202-Dashkovskaya/assets/90696514/5410ea24-9219-4b3d-8f75-58ef84b84721)
#### <a>Результат пинга</a>
![image](https://github.com/DanaDaschoca/2023_2024-introduction_in_routing-k33202-Dashkovskaya/assets/90696514/04dc892e-c888-4183-a092-29a6440786bb)
#### <a>Пример таблицы маршрутов MPLS</a>
![image](https://github.com/DanaDaschoca/2023_2024-introduction_in_routing-k33202-Dashkovskaya/assets/90696514/216dbff0-bf95-4983-be71-9a2183c4d7bd)
#### <a>Вывод</a>
В ходе выполнения данной лабораторной работы мы на практике познакомились с протоколами OSPF, MPLS, EoMPLS и механизмами их организации.
