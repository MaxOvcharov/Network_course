[Лекция "Технология Ethernet"](https://youtu.be/s-uDMX4X2jQ)
1. Технологии Ethernet:
    1. Использование на уровнях OSI:
        1. Физический
        2. Канальный
    2. Классический Ethernet:
        * Разделяемая среда
        * Ethernet - Gigabit
    3. Коммутируемый Ethernet:
        * Точка-точка
        * Появился в Fast Ethernet
        * Единственный вариант в 10G и выше Ethernet
    4. На Физическом уровне Ethernet:
        * Коаксиальный кабель
        * Витая пара
        * Оптоволокно
    5. На Канальном уровне Ethernet:
        * Методы доступа и протоколы, одинаковы для любой среды передачи данных
        * В Классическом Ethernet смешаны подуровни LLC и MAC
    6. Формат кадра Ethernet 2:
        1. Заголовок:
            * Адрес получателя - 6 байт
            * Адрес отправителя - 6 байт
            * Тип - 2 байта (IPv4, IPv6, ARP)
        2. Данные:
            * Максимальное ограничение - 1500 байт (JumboFrame - 9000 байт)
            * Минимальная длина - 46 байт
        3. Концевик - контрольная сумма