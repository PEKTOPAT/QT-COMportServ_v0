# SEMZ-QT-COMportGenerate
Протокол обмена между arduino и приложением на ПК по COM порту для формирования биимпульсного сигнала
1.Для сброса arduino необходимо выдать 1 байт информации с информацией 0xАА
2. Для начала формирования сигнала необходимо заполнить буфер соответствующего канала.на 10 байт(для скорости 9,6 кбит/с — 20 байт), установить необходимую скорость и выставить бит разрешения(Таблица 2)
3 При уменьшении информации для формирования меньше пороговых (таблица 3) устройство выдаёт соответствующую информацию в COM-порт. (Таблица 3).
4. При опустошении буфера, канал прекращает формирование информации. В COM-порт выдаётся соответствующее сообщение. (Таблица 3)
