[Лекция "Сетевой уровень"](https://youtu.be/K-yvp1ti-QU)
1. Согласование различай в сетях:
    * Тип сервиса:
        * Кадры из Wi-Fi принимаются с отправкой подтверждения
        * В Ethernet - без подтверждения
    * Адресация:
        * Глобальные адреса, не зависимые о конкретных технологий
        * Методы преобразования глобального адреса в локальный(ARP для TC/IP)
    * Широковещание:
        * Пакеты оправляются всем хостам сети по индивидуальным адресам
2. Масштабируемость на сетевом уровне:
    1. Агрегация адресов:
        * Работа не с отдельными адресами, а с блоками адресов
        * Блок адресов - сеть
    2. Запрет пересылки «мусорных» пакетов:
        1. Пакет отбрасывается, если нельзя определить, куда его нужно отправлять
    3. Возможность наличия нескольких путей в сети:
        1. Одна из основных причин создания сетей с пакетной коммутацией
        2. Допускается несколько активных путей
        3. Задача выбора лучшего пути - маршрутизация
3. Маршрутизация (routing) - поиск маршрута доставки пакета между сетями через транзитные узла - маршрутизаторы
    1. Учет изменений в топологии ети
    2. Учет загрузки каналов связи и маршрутизаторов
4. Продвижение (Forwarding) - передача пакета внутри маршрутизатора в соответствии с правилами маршрутизации
5. Протоколы сетевого уровня стека TC/IP: IP, ICMP, ARP, DHCP