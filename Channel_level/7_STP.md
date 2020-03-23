[Лекция "Протокол STP"](https://youtu.be/xtHlGmd94ec):

1. STP (Spanning Tree Protocol - Протокол связующего(основного) дерева):
    * Автоматическое отключение дублирующих соединений в Ethernet
    * Связующее дерево - подграф без циклов, содержащий все вершины исходного графа
2. Использование на уровнях OSI:
    * Канальный уровень (коммутаторы)
3. Преимущества:
    1. Надежность соединений между коммутаторами - Широковещательный шторм
    2. Защита от ошибок конфигурации
4. Этапы работы протокола:
    1. Выбор корневого коммутатора
    2. Определение кратчайшего пути до коммутатора
    3. Отключение всех остальных соединений
5. Сообщение протокола STP - BPDU - Bridge Protocol Data Units - отправляется каждые 2 сек, рассылается на групповой адрес STP
6. Расчет кратчайшего пути до корневого коммутатора:
    1. Количество промежуточных коммутаторов
    2. Скорость соединения
7. Состояние портов в STP:
    * Listening - порт обрабатывает BPDU, но не передает данные
    * Learning - порт не передает кадры, , но изучает MAC-адреса поступающие в кадрах и формирует таблицу коммутации
    * Forwarding - порт передает и принимает кадры данных и  BPDU
    * Blocking - порт заблокирован, чтобы избежать кольцевых соединений
    * Disabled - отключен администратором
8. Виды STP:
    * RSTP - Rapid Spanning Tree Protocol - быстрый переход между режимами Listening -> Forwarding
    * MSTP - Multiple Spanning Tree Protocol - для работы с VLAN