# Проєктування системи

@startuml
Client <--> [Get] : JSON
[Get] <--> Server : HTTP

Client <--> [Post] : JSON
[Post] <--> Server : HTTP

Client <--> [Put] : JSON
[Put] <--> Server : HTTP

Client <--> [Delete] : JSON
[Delete] <--> Server : HTTP
@enduml

### Пояснення:

Клієнт надсилає (Get, Post, Put, Delete) запит у форматі JSON, який сервер обробляє вже у форматі HTTP.

-  Get - (запит на отримання інформації)
-  Post - (запит на додання інформації)
-  Put - (запит на оновлення інформації)
-  Delete - (запит на видалення інформації)

</center>
