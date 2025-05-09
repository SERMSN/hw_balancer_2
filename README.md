# netology_hw_balancer_2
## Домашнее задание к занятию «Кластеризация и балансировка нагрузки» - Малявко Сергей

#### Задание 1
* Запустите два simple python сервера на своей виртуальной машине на разных портах
* Установите и настройте HAProxy, воспользуйтесь материалами к лекции по ссылке
* Настройте балансировку Round-robin на 4 уровне.
* На проверку направьте конфигурационный файл haproxy, скриншоты, где видно перенаправление запросов на разные серверы при обращении к HAProxy.

##### Скриншот результата блансировки Round-robin на 4 уровне:
![Скриншот результата блансировки Round-robin на 4 уровне рис. 1](https://github.com/SERMSN/hw_balancer_2/blob/main/images/HAProxy-1-1.png)
##### Конфигурационный файл haproxy:
[Конфигурационный файл haproxy](https://github.com/SERMSN/hw_balancer_2/blob/main/configs/haproxy1.cfg)


#### Задание 2
* Запустите три simple python сервера на своей виртуальной машине на разных портах
* Настройте балансировку Weighted Round Robin на 7 уровне, чтобы первый сервер имел вес 2, второй - 3, а третий - 4
* HAproxy должен балансировать только тот http-трафик, который адресован домену example.local
* На проверку направьте конфигурационный файл haproxy, скриншоты, где видно перенаправление запросов на разные серверы при обращении к HAProxy c использованием домена example.local и без него.

##### Скриншот настройки 3-х http серверов:
![Скриншот yнастройки 3-х серверов рис. 3](https://github.com/SERMSN/hw_balancer_2/blob/main/images/HAProxy-2-1.png)
##### Скриншот результата блансировки Weighted Round Robin на 7 уровне на example.local:
![Скриншот результата блансировки Weighted Round Robin на 7 уровне на example.local рис. 4](https://github.com/SERMSN/hw_balancer_2/blob/main/images/HAProxy-2-2.png)
##### Скриншот результата блансировки не приходящего на домен example.local т.е. отбрасывем запросы:
![Скриншот результата блансировки кроме example.local рис. 5](https://github.com/SERMSN/hw_balancer_2/blob/main/images/HAProxy-2-3.png)
##### Конфигурационный файл haproxy:
[Конфигурационный файл haproxy](https://github.com/SERMSN/hw_balancer_2/blob/main/configs/haproxy2.cfg)




