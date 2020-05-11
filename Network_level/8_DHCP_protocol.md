[Лекция "Протокол DHCP"](https://youtu.be/uZJ8WVdw-Ck)
1. Клиент и сервер обмениваются сообщениями DHCP в режиме запрос-ответ
2. Получение IP-адреса - DORA
3. Список сообщений в DHCP:
    1. DISCOVER - поиск DHCP сервера
    2. OFFER - предложение IP-адреса DHCP сервером
    3. REQUEST - запрос IP-адреса клиентом
    4. ACK - подтверждение получения IP-адреса клиенту
    5. NACK - запрет использования запрещенного DHCP-клиентом IP-адреса
    6. RELEASE - освобождение IP-адреса
    7. INFORM - запрос и передача дополнительной конфигурационной информации
4. Пул адресов - список IP-адресов, который назначает DHCP сервер. Следит за уникальностью распределения IP-адресов
5. Время аренды в DHCP:
    * Продление после половины срока аренды
    * Сокращенная процедура получения IP-адреса
6. DHCP сервер должен находиться в одной подсети с компьютером. Либо маршрутизатор должен поддерживать механизм - DHCP Relay.