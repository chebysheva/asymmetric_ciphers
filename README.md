Модифицируйте код клиента и сервера так, чтобы приватный и публичный ключ хранились в текстовых файлах на диске и, таким образом, переиспользовались между запусками.
Проведите рефакторинг кода клиента и сервера так, чтобы все, относящееся к генерации ключей, установлению режима шифрования, шифрованию исходящих и дешифрованию входящих сообщений было отделено от основного алгоритма обмена сообщениями.
Ключи клиента и сервера:
![image](https://user-images.githubusercontent.com/90459151/147104859-80d1446f-c70c-4de5-9507-ad0cc3b68348.png)
![image](https://user-images.githubusercontent.com/90459151/147104964-47f3f322-cc03-4d4d-8250-a1e30e31bc58.png)

Реализуйте на сервере проверку входящих сертификатов. На сервере должен храниться список разрешенных ключей. Когда клиент посылает на сервер свой публичный ключ, сервер ищет его среди разрешенных и, если такого не находит, разрывает соединение. Проверьте правильность работы не нескольких разных клиентах:
Разрешенные ключи хранятся в отдельном файле.

Модифицируйте код клиента и сервера таким образом, чтобы установление режима шифрования происходило при подключении на один порт, а основное общение - на другом порту. Номер порта можно передавать как первое зашифрованное сообщение.
![image](https://user-images.githubusercontent.com/90459151/147106910-49596b0c-ae4c-44c7-9126-a5766ef4ead1.png)


Модифицируйте код FTP-сервера таким образом, чтобы он поддерживал шифрование. Методы, поддерживающие шифрование:
![image](https://user-images.githubusercontent.com/90459151/147107322-b34538e2-53cc-4e3e-b05c-6a739a2821e8.png)
