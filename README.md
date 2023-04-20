# arms-rc-advanced
Продвинутая схема подключения удаленного управления компьютерами из веб-интерфейса [БД Инвентаризации](https://wiki.reviakin.net/%D0%B8%D0%BD%D0%B2%D0%B5%D0%BD%D1%82%D0%B0%D1%80%D0%B8%D0%B7%D0%B0%D1%86%D0%B8%D1%8F:%D1%83%D0%B4%D0%B0%D0%BB%D0%B5%D0%BD%D0%BD%D0%BE%D0%B5_%D1%83%D0%BF%D1%80%D0%B0%D0%B2%D0%BB%D0%B5%D0%BD%D0%B8%D0%B5_%D0%BE%D1%81)  
В отличии от [arms-rc-simple](https://github.com/spo0okie/arms-rc-simple) ПО управления запускается от другого пользователя нежели браузер (браузер не имеет полномочий на удаленное управление)

Для установки нужно заполнить файлик *params.vbs*  


```vbs
workDir = "C:\Program Files\inventoryRC"          'папка где будут располагаться скрипты
dim pidFile : pidFile = workDir & "\watcher.pid"  'pid файл (он же heartbeat)

const fileTimeout=40           'такймаут запроса на соединение
const hbTimeout=10             'таймаут heartBeat файла
const watcher="watcher.wsf"    'скрипт watcher работающий от имени админа с правами на удаленное управление
const launcher="launcher.wsf"  'скрипт launcher вызываемый из браузера

```