# Bug Report

## BUG-01 — 500 при передаче спецсимволов в query
- [ ] При передаче спецсимволов в параметре query API возвращает ошибку 500 Internal Server Error.
- [ ] *Endpoint:* GET https://api.cian.ru/geo-suggest/v2/suggest
- [ ] *Пaрaметры:* 
- [ ] offerType=flat
- [ ] query=[]{}!!!
- [ ] regionId=2
- [ ] dealType=rent
- [ ] source=serp
- [ ] *Steps:*
- [ ] Отправить GET-запрос с указанными параметрами
- [ ] Использовать спецсимволы в query
- [ ] *Ожидaемый результaт:*
- [ ] 400 Bad Request или 200 OK с пустым результатом
- [ ] *Фактический результат*
- [ ] 500 Internal Server Error
- [ ] *Severity*
- [ ] High
- [ ] *Priority*
- [ ] High

