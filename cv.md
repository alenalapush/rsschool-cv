# ***Алена Ивановская*** 


![Моё фото](https://raw.githubusercontent.com/alenalapush/rsschool-cv/gh-pages/photo.jpg)

## *Контакты*
   - Беларусь - Витебск
   - +375(29) 216-69-32 
   - Telegram: [@pro100key](https://t.me/@pro100key)
   - Discord: alenalapush_49680
   
  


## *О себе*

Нацелена на активный профессиональный старт и развитие в IT-сфере. Главными своими сильными сторонами считаю: высокую скорость обучения, инициативность, готовность быстро вникать в сложные рабочие процессы и  стремление к большему.


## *Навыки*
    **Практические навыки:**
     Построение диаграмм UML 2.0
     Знание SQL

    **Теоритические знания:**
     процесс разработки ПО, принципы ООП, БД, СУБД, методологий управления проектами

    **Программы:**
      DBeaver
      Visual Studio Code


## *Примеры кода*

SQL: [практика по SQL](https://github.com/alenalapush/SQL)

```sql
select PERCENTILE_CONT(0.95) within group(order by score) as p95
from users
where date_joined>'2022,01,01'
and score>100
```

UML: [практика по UML](https://github.com/alenalapush/UML)

```UML
@startuml
' Настройка стиля
skinparam componentStyle uml2
left to right direction

package "Client Layer" {
    [Mobile App] as App <<Component>>
}

package "API Management" {
    [API Gateway] as Gateway <<Component>>
}

package "Core Business Logic" {
    [Order Service] as Orders <<Component>>
    [Payment Service] as Payments <<Component>>
    [Notification Service] as Notifications <<Component>>
}

package "Data & Analytics" {
    [Analytics Service] as Analytics <<Component>>
    queue "Message Broker (Kafka/RabbitMQ)" as Queue
    database "Main DB" as DB
}

node "External Systems" {
    [Google Maps API] as Maps <<Service>>
    [Stripe Payment] as Stripe <<Service>>
    [Push Notification Service] as PushSrv <<Service>>
}

' --- Интерфейсы ---
interface "Mobile API" as MAPI
interface "Payment API" as PAPI

' --- Связи ---

' Клиент заходит через шлюз
App --( MAPI
MAPI - Gateway

' Шлюз распределяет задачи
Gateway --> Orders
Gateway --> Payments

' Сервис заказов взаимодействует с окружением
Orders ..> DB : CRUD Operations
Orders ..> Maps : Route & ETA
Orders ..> Notifications : Trigger: "Status Changed"

' Асинхронная передача данных в аналитику (через очередь)
Orders ..> Queue : Publish: "Trip Finished"
Queue ..> Analytics : Consume events

' Платежи
Payments --( PAPI
PAPI - Stripe

' Уведомления
Notifications ..> PushSrv : Send Push
PushSrv ..> App : Deliver to device

@enduml
```

Javascript: [практика по Javascript](https://www.codewars.com/kata/50654ddff44f800200000004/train/javascript)

```javascript
function multiply(a, b) {
  return a * b;
}
```


## *Мой проект*
 **Репозиторий:** [rsschool-cv](https://github.com/alenalapush/rsschool-cv)


## *Опыт работы*

[![GitHub](https://img.shields.io/badge/GitHub-alenalapush-181717?logo=github)](https://github.com/alenalapush)


## Образование

* **Высшее техническое (Инженер-программист)**   
  *2026 — 2027 (ожидаемый год окончания)*
 

* **Высшее экономическое (Бухгалтер)**  
  *2011 — 2012*

* **Высшее биологическое (Эколог)**  
  *2005 — 2010*

## Опыт работы

* **Бухгалтер** 
  *2012г — 2025г*
  * Профессиональный опыт в экономическом секторе. 
  * Автоматизировала бухгалтерский учет, участвовала в обновлении и тестировании корпоративного ПО 

* **Инженер-технолог**
  *2010г — 2012г*
  * Разработка технической документации и контроль соблюдения тех.процесса  производства печатных плат.


## *Английский язык*

     Pre-Intermediate   

 





