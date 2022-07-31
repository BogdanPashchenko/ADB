# Работа с AndroidStudio и с инструментом программирования, используемый для отладки устройств на базе Android - ADB

### Отобразить подключённый девайс в консоли:
#### *./adb devisec *

### Вывести адрес приложения todolist в системе Android:
#### *./adb shell pm list packages | findstr todolist *

### Установить .apk файл приложениия todolist на телефон с компьютера через ADB:
#### *./adb install D:\todo.apk *

### Сделать скриншот запущенного приложения todolist и сразу скопировать на компьютер в одной команде:
#### *./adb shell screencap /sdcard/screen.png | ./adb pull /sdcard/screen.png D:\AndroidSDK *

### Вывести в консоль логи приложения todolist:
#### *./adb install D:\todo.apk*

### Сделать скриншот запущенного приложения todolist и сразу скопировать на компьютер в одной команде:
#### *./adb shell  – Происходит переход в Shell, затем logcat | grep com.android.todolist*

###  Скопировать логи приложения todolist на компьютер:
#### *./adb install D:\todo.apk*

### Сделать скриншот запущенного приложения todolist и сразу скопировать на компьютер в одной команде:
#### *./adb shell – Происходит переход в Shell, затем logcat | grep todolist > /sdcard/todolist.txt – Создается txt с логами на самом телефоне, далее выход из shell, ./adb pull /sdcard/todolist.txt todolist_1.txt – Переносится файл на ПК*

###  Удалить приложение todolist с телефона через ADB:
#### *./adb uninstall com.android.todolist*
