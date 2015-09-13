WebSocket Server Test
=====================

Тестовый сервер для обслуживания клиентов WebSocket.

Для запуска необходим модуль [Net::WebSocket::Server][] . Установить его
можно из CPAN следующим образом:

1.  Запустить CPAN shell от нимени суперпользователя:

        # cpan

    или

        # perl -MCPAN -e shell

2.  Установить модуль с помощью команды `install`:

        cpan[...]> install Net::WebSocket::Server

Для проверки нужно:

1.  Запустить сервер: `$ ./server`
2.  Пойти на [страницу теста][wsorg_echo] с этого же компа,
    ввести в поле Location адрес `ws://127.0.0.1:8080` и нажать Connect.
3.  Для нагладности можно открыть несколько клентских соединений, повторив
    предыдущий пункт из разных вкладок/браузеров.
4.  Отправлять сообщения на сервер со страницы, используя поле Message
    и кнопку Send.


[Net::WebSocket::Server]: http://search.cpan.org/~topaz/Net-WebSocket-Server-0.001003/lib/Net/WebSocket/Server.pm
[wsorg_echo]: http://www.websocket.org/echo.html
