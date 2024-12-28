### Linux: Основы работы с аппаратной частью (LPI 101.1)
Основные навыки:

- Управление комплектующими ПК.
- Работа с оборудованием и его настройка через Linux.

Что изучаем:

- Получение информации об оборудовании:
- Узнаем, как просматривать данные о процессоре, памяти, шинах и подключенных устройствах.

 
Управление устройствами:

- Работа с модулями ядра и драйверами.


Понятия и инструменты:

- sysfs: хранит данные об устройствах.
- udev: современный менеджер устройств.
- dbus: шина для обмена данными между процессами.

Основные утилиты:

-  /sys/, /proc/, /dev/ — специальные каталоги с информацией об устройстве и системе.
-  modprobe, lsmod — управление модулями ядра.
-  lspci, lsusb — данные об устройствах PCI и USB.
-  udevadm — утилита для работы с udev (например, просмотр событий устройств).

Основные принципы работы:

- /dev: доступ к устройствам через специальные файлы, которые "ссылаются" на драйверы.
- /sys: структура данных о подключенном оборудовании (например, блочные устройства или шины).
- /proc: информация о процессах и состоянии системы (например, данные о процессоре или подключенных файловых системах).

Особенности udev:

- Работает на уровне пользователя (гибкость).
- Управляется событиями.
- Держит только активные устройства в системе.
- Удобные конфигурационные файлы (не XML).

Примеры команд:

- lsmod: посмотреть загруженные модули.
- lspci: вывести информацию об устройствах PCI.
- lsusb: узнать о подключенных USB-устройствах.
- modprobe: загрузить или выгрузить модули ядра.
- udevadm info: получить данные об устройстве.