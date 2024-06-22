# Тема 6

Реализация аутентификации пользователей на HTTP-сервере с использованием SSL-сертификатов. Пользователи хранятся в реляционной СУБД 

[A Very Simple HTTP Server writen in C](https://blog.abhijeetr.com/2010/04/very-simple-http-server-writen-in-c.html)

## Сборка/запуск

- Сборка

~~~
gcc HTTPSimple.c -o server -lssl -lcrypto -lsqlite3
~~~

- Запуск

~~~
./Server -p 10000 -r webroot
~~~

