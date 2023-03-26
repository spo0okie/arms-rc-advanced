# arms-rc-advanced
Продвинутая схема подключения удаленного управления компьютерами из веб-интерфейса [БД Инвентаризации](https://wiki.reviakin.net/%D0%B8%D0%BD%D0%B2%D0%B5%D0%BD%D1%82%D0%B0%D1%80%D0%B8%D0%B7%D0%B0%D1%86%D0%B8%D1%8F:%D1%83%D0%B4%D0%B0%D0%BB%D0%B5%D0%BD%D0%BD%D0%BE%D0%B5_%D1%83%D0%BF%D1%80%D0%B0%D0%B2%D0%BB%D0%B5%D0%BD%D0%B8%D0%B5_%D0%BE%D1%81)
В отличии от [arms-rc-simaple](https://github.com/spo0okie/arms-rc-simple) само ПО управления работает от другого пользователя нежели браузер, вызывающий управление

Регистрируем файлик *register.reg*
Размещаем файлк *remotecontrol.cmd* по пути `C:\Program Files\remotecontrol\remotecontrol.cmd`
В самом *remotecontrol.cmd* вызывается ПО удаленного управления *Lite Manager*. Можно поменять на свое
