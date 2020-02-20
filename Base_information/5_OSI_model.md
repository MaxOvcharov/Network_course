[Лекция "Модель OSI" Модель взаимодействия открытых систем (Open Systems Interconnection - OSI)](https://youtu.be/Tt8BTkxz_Vc)
1. Уровни модели OSI:
    1. Физический:
        * Задача - представить биты информации в виде сигналов, передаваемых по сети
    2. Канальный:
        * Передача сообщений по каналу - определение начала/конца сообщения в потоке бит
        * Обнаружение и коррекция ошибок
    3. Сетевой:
        * Создание составной сети, согласование различий в сетях
        * Адресация(сетевые или глобальные адреса)
        * Определение маршрута пересылки в составной сети(маршрутизация)
    4. Транспортный:
        * Обеспечивает передачу данных между процессами на хостах
        * Может предоставлять надежность выше, чем у сети
        * Сквозной уровень: сообщения доставляются от источника адресату, предыдущие уровни используют принцип звеньев сети
    5. Сеансовый:
        * Управление диалогом(процесс передачи сообщений)
        * Управление маркерами(предотвращение одновременного выполнения кричиской операции)
        * Синхронизация(метки в сообщениях для возобновления передачи информации)
    6. Представления:
        * Обеспечивает согласование синтаксиса и семантики передаваемых сообщений
        * Шифрование и дешифрование
    7. Прикладной:
        * Набор приложений полезных пользователю
2. Сетевое оборудование:
    * Сетевой уровень      ->    маршрутизатор
    * Канальный уровень    ->    коммутатор, точка доступа
    * Физический уровень   ->    концентратор