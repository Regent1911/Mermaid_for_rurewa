# Задания по Mermaid для студентов

## Приготовление чая — Mermaid from Regent1911

```mermaid
graph TD
    A[Начало] --> B[Кипячение воды]
    B --> C{Есть ли чай?}
    C -->|Да| D[Заварить чай]
    C -->|Нет| E[Купить чай] --> D
    D --> F[Пить чай]
    F --> G[Конец]
```

## Заказ такси — Mermaid from Regent1911

```mermaid
sequenceDiagram
    participant Клиент
    participant Приложение
    participant Сервер
    participant Водитель

    Клиент->>Приложение: Вызывает такси
    Приложение->>Сервер: Отправляет запрос
    Сервер->>Водитель: Ищет свободного водителя
    Водитель-->>Сервер: Принимает заказ
    Сервер->>Клиент: Уведомляет о принятии
    Клиент->>Водитель: Забирает клиента
```
<!--Задание 2.1: Диаграмма классов UML-->
## Библиотечная система — Mermaid from Regent1911

```mermaid
classDiagram
    class Book {
        -title: string
        -author: string
        -ISBN: string
        -isAvailable: boolean
    }

    class User {
        -name: string
        -userId: string
        -borrowedBooks: Book[]
    }

    class Library {
        -books: Book[]
        -users: User[]
    }

    User "*" --  Book :.borrowedBooks
    Library "1" o--  Book : содержит
    Library "1" o--  User : управляет
```

## Coming Soon<...>
<!--coming soon-->