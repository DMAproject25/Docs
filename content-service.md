# Техническое Задание
## 1)Сущности:
* profile - id, name - имя пользователя, surname - Фамилия, description - описание, sex - пол, age - возраст
* tag - id, name - имя тэга
* response - id, sender_id - id отправителя, recipient_id - id получателя, verdict - ожидает PENDING, принят APPROVED или отклонен REJECTED 

## 2)Api

Сервис должен предоставить RestFull Api для работы с этими сущностями.

Пользовательские методы:

* POST api/profile - создать профиль
* GET api/profile - получить профиль
* PUT api/profile - обновить профиль
* DELETE api/profile - удалить профиль
* POST api/response - отправить отклик
* GET api/response?profile_id= - получить все отклики на профиль
* PUT api/response/verdict - принять/отклонить отклик

Админские методы:

* POST api/admin/tags - создать интерес
* PUT api/admin/tags - обновить интерес
* DELETE api/admin/tags - удалить интерес 
