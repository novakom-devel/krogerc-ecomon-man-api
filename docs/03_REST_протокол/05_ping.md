# Ідентифіктор /ping 
Тест працездатності сервісу. Повертає відповідь та дату.

## Вхідні параметри
Поле | Обов'язкове | Тип даних | Описую
:----|:-----------:|:-----------|:------
**token** | √ | string | Секретний токен від [collector](/99_Глосарій#collector)

## Вихідні дані
Результат повинен бути рядком. Що містить текст `"PONG at <date_iso8601>"`. Дата та час у форматі [ISO8601](/99_Глосарій#iso8601).

## Приклад

### Дані, що відправляють 
```JSON
  { "token": "xxxxxxxxxxxxxxxxxxxx"}
```

### Дані, що отримують
```JSON
  {
    "success" : true,
    "code" : 200,
    "status" : "success",
    "result": "PONG at 2018-01-19T11:30:17+02:00"
  }
```

### Варіація запиту через консоль
запит:
```BASH
curl -H "Content-Type: application/json" -X POST --data '{"token": "xxxxxxxxxxxxxxxxxxxx"}' "http://example.com/ping"
```
відповідь:
```JSON
{
  "success" : true,
  "code" : 200,
  "status" : "success",
  "result": "PONG at 2018-01-19T11:30:17+02:00"
}
```
