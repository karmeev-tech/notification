### Оповещения

> *Что мы ожидаем от вызывающей стороны*

* Указание на важность сообщения
* Указание на тип запуска (файл/программа)

> *Что мы предоставляем вызывающей стороне*
> * Сообщение о том, что пришло оповещение
>> *Что мы готовы предоставить вызывающей стороне*
>> * Статус анализа
>> * Наименование процесса (наим. оповещения)
>> * Тип запуска (файл/программа)
>> * Информация оповещения (описание)
>> * Статус оповещения
>> * Время оповещения

### Notification

> *Request*

```json
{
    "NameOfProcess": "name",
    "TypeOfStartUp": "file",
    "MessageImportance" : "low"
}
```

> *Response*

```json
{
    "StatusCode": "",
    "Message": "",
    "Errors": [],
    "Time":"2021-07-26T01:37:41.7482907+03:00",
    "Information" :
    {
        "NameOfProcess": "test",
        "TypeOfStartUp": "file",
        "AnalyzeStatus" : "application in process",
        "Importance": "low",
        "NotificationInfo" : "information about process",
    }
}
```