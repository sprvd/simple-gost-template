# `simple-gost-template`

Шаблон оформления учебных работ по ГОСТ для [Typst](https://typst.app).

## Использование

```typst
#import "@preview/simple-gost-template:0.1.0": gost-work

#show: gost-work.with(
  organization: [Название организации],
  department: [Название кафедры],
  work-name: [Вид работы],
  subject: [Название дисциплины],
  student-text: [Работу выполнил \ студент группы],
  student-group: [ГРУ-ПА],
  student-name: [Фамилия И.О.],
  teacher-text: [Работу проверил],
  teacher-name: [Фамилия И.О.],
  city: [Город],
)

= Введение

= Основная часть
```

## Параметры

| Параметр | Тип | По умолчанию | Описание |
|---|---|---|---|
| `organization` | content | — | Название организации |
| `department` | content | — | Название кафедры |
| `work-name` | content | — | Вид работы |
| `subject` | content | — | Название дисциплины |
| `student-text` | content | — | Текст перед именем студента |
| `student-group` | content | — | Номер группы |
| `student-name` | content | — | Фамилия И.О. студента |
| `teacher-text` | content | — | Текст перед именем преподавателя |
| `teacher-name` | content | — | Фамилия И.О. преподавателя |
| `city` | content | `[Город]` | Город |
| `year` | int or none | `none` | Год (если не задан — текущий) |
| `bibliography-file` | string | `""` | Путь до файла библиографии |

## Альтернативы

Если нужен более полный шаблон с поддержкой всех требований ГОСТ 7.32, обратите внимание на [modern-g7-32](https://github.com/typst-gost/modern-g7-32).
