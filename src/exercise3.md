## 1. Код ответа: 201. Тело ответа:

[
    {
        "name": "Малышева Екатерина Матвеевна",
        "birthday": "1995-06-01",
        "post": "Бухгалтер"
    },
    {
        "name": "Капустин Роман Артёмович",
        "birthday": "1991-01-18",
        "post": "Финансовый аналитик"
    },
    {
        "name": "Касьянов Ярослав Ярославович",
        "birthday": "1989-07-29",
        "post": "Кредитный эксперт"
    },
    {
        "name": "Белова Елизавета Руслановна",
        "birthday": "1997-04-13",
        "post": "Аудитор"
    },
    {
        "name": "Романов Константин Александрович",
        "birthday": "2001-12-14",
        "post": "Кассир"
    },
    ...
]
#### Верный код ответа: 200 OK (успешный запрос)

## 2. Код ответа: 400. Тело ответа:
{
  "message": "Неверные данные для авторизации.
}  


 #### Верный код ответа: 401 (для доступа к запрашиваемому ресурсу требуется аутентификация)


## 3. Код ответа: 500. Тело ответа:
{
  "message": "Неверно составлен запрос."
}

##### Верный код ответа: 400 (сервер обнаружил в запросе клиента синтаксическую ошибку)
