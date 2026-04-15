# Анализ API

## Endpoint
GET /geo-suggest/v2/suggest

## Назначение
API предназначен для получения подсказок (suggestions) при вводе поискового запроса пользователем.

## Query параметры

| Параметр   | Тип     | Описание |
|-----------|--------|---------|
| query     | string | Поисковая строка |
| regionId  | number | ID региона |
| offerType | string | Тип недвижимости (flat) |
| dealType  | string | Тип сделки (rent) |
| source    | string | Источник запроса (serp) |

## Пример запроса

GET /geo-suggest/v2/suggest?query=сaнкт-петербург&regionId=2&offerType=flat&dealType=rent&source=serp

## Структура ответа

```json
{
  "data": {
    "suggestions": {
      "cities": {
        "items": [
          {
            "id": 2,
            "type": "city",
            "regionId": 2,
            "name": "Сaнкт-Петербург",
            "fullName": "Сaнкт-Петербург"
          }
        ]
      }
    }
  }
}