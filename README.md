# 02.simple

Простейший HTTP-сервер на С, базируется на статье: 

[A Very Simple HTTP Server writen in C](https://blog.abhijeetr.com/2010/04/very-simple-http-server-writen-in-c.html)

## Возможности

- Выполняет базовую обработку GET-запроса (протокол доступа, HTTP-команда, запрашиваемый ресурс)
- Выдает запрашиваемые HTTP-клиентом файлы
- Позволяет параметризовать порт и корневой каталог
- Обработка каждого запроса в отдельном процессе

## Сборка/запуск

- Сборка

~~~
make HTTPSimple
~~~

- Запуск

~~~
./HTTPSimple -p 8080 -r webroot
~~~

- Проверка работоспособности

~~~
curl -v --cert client_cert.pem --key client_key.pem --cacert keys/ca/ca_cert.pem https://localhost:10000/
~~~

