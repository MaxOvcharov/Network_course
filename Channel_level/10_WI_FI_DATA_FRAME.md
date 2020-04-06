[Лекция "Wi-Fi. Формат кадра"](https://youtu.be/nhhDsnQoWh0)
1. Формат кадра Wi-Fi уровня MAC:
    1. Управление кадром
    2. Длительность - указывается на какое время зарезервирован канал доступа Wi-Fi
    3. Адрес 1
    1. Адрес 2
    2. Адрес 3
    3. Управление очередностью
    4. Адрес 4
    5. Тело кадра - 2304 байт
    6. Контрольная сумма
2. Типы Адресов:
    1. DA - Destination address - адрес получателя
    2. SA - Source address - адрес отправителя
    3. RA - Receiver address - адрес принимающего устройства
    4. TA - Transmitter address - адрес отправляющего устройства
3. Пути передачи кадров:
    * Передача кадра в распределительную систему - a1(RA)->a2(TA/SA)->a3(DA)
    * Передача кадра от распределенной системы - a1(RA/DA)->a2(TA)->a3(SA)
    * Передача кадра в одноразовом режиме - a1(RA/DA)->a2(TA/SA)->a3(Идентификатор сети BSSID)
    * Беспроводной мост - a1(RA)->a2(TA)->a3(DA)->a4(SA)
4. Состав поля Управление кадром:
    1. Версия протокола - 0
    2. Тип:
        * Кадры данных - такие же как в Ethernet
        * Кадры контроля:
            1. Служебные кадры
            2. RTS, CTS, ACK
        * Кадры управления(Management frame):
            1. Реализация сервисов Wi-Fi
    3. Подтип
    4. To DS - к распределительной системе
    5. From DS - от распределительной системы
    6. MF - Управление очередностью:
        * Номер последовательности
        * Номер фрагмента
    7. RT - повторная отправка кадра
    8. Power Mgnt - экономия энергии клиента
    9. MD - есть ли еще данные
    10. Protected Frame - защита кадра
    11. Order - сохраняется ли порядок передачи данных, на практике всегда сохраняется