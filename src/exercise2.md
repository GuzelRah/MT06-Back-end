# CRUD
REST API основывается на протоколе передачи гипертекста HTTP (Hypertext Transfer Protocol). Это стандартный протокол в интернете, созданный для передачи гипертекста. 
Каждый объект на сервере в HTTP имеет свой уникальный URL-адрес в строгом последовательном формате. 

В REST API есть 4 метода HTTP, которые используют для действий с объектами на серверах:

- GET (получение информации о данных или списка объектов)  
- DELETE (удаление данных)  
- POST (добавление или замена данных)  
- PUT (регулярное обновление данных)  

Такие запросы еще называют идентификаторами CRUD:  
__С__ reate (создать),   
__R__ ead (прочесть),  
__U__ pdate (обновить),   
__D__ elete (удалить).   

Это стандартный набор действий для работы с данными. 

### Create
Создание новых данных — ключевая функция всего CRUD. Остальные операции не имеют смысла без создания новой записи в базе данных.

При создании новой записи важно валидировать данные, как и в любой форме. Подробнее про валидацию вы узнали из урока «Формы».

Валидация помогает не допустить ошибочные данные в базу и таким образом предотвратить возможные ошибки при чтении. Правильная валидация данных так же обеспечивает защиту от вредоносных значений, которые могут быть добавлены в базу данных.

### Read
Чтение данных — операция, которая доступна всем пользователям. Зачастую, чтение — единственная операция, которая доступна пользователю без прав администратора. Например, вы и другие студенты Хекслета можете читать этот урок, но отредактировать урок или создать новый не получится.

В операции чтения важно контролировать доступ к информации. Пользователь не должен видеть информацию, к которой у него нет доступа. Например, как владелец банковского счета вы можете увидеть только свой баланс, доступа к чужим счетам у вас нет.

### Update
Операция обновления похожа на создание — с ее помощью мы вносим изменения в базу данных. В случае с обновлением важно корректно сохранять ранее внесенные данные. Например, если вы меняете свой логин на сайте, то при этом не должна затрагиваться информация о пароле и электронной почте.

### Delete
Удаление — последняя операция для CRUD. Она удаляет записи из базы данных, будь то информация о картине или метка на карте.

Обычно удаление выполняется после проверки прав доступа к данным. Например, если пользователь не имеет право удалять записи, запрос не сработает. Если право есть, система начинает удалять данные.

С точки зрения реализации удаление делится на два типа:

- Физическое — запись стирается из базы данных без возможности восстановления

- Логическое — к записи закрывается доступ на чтение, то есть она скрывается. Доступ всегда можно восстановить при необходимости. Логическое удаление больше похоже на обновление, потому что физически запись в базе данных остается.