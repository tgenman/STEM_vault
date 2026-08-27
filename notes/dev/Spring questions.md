---
aliases:
created: 2025-10-16 13:19
parent:
  - "[[root dev questions]]"
connected:
  - "[[Java questions]]"
  - "[[Kotlin questions]]"
tags:
---



TARGET DECK: stem::dev::spring

START
math_basic_single
FRONT: Какие существуют основные виды Scope в Spring?
BACK: 
1. **singleton** — один экземпляр бина на весь контекст Spring (по умолчанию).  
2. **prototype** — новый экземпляр бина при каждом запросе.  
3. **request** — один экземпляр на каждый HTTP-запрос (только в веб-контексте).  
4. **session** — один экземпляр на HTTP-сессию (только в веб-контексте).  
5. **application** — один экземпляр на весь `ServletContext`.  
6. **websocket** — один экземпляр на WebSocket-сессию.
ID: 1760612201095
END

START
math_basic_single
FRONT: В чём разница между scope `singleton` и `application` в Spring?
BACK: 
- **singleton** — создаётся один экземпляр бина **на весь Spring ApplicationContext**.  
  → Если несколько контекстов (например, root и web), то у каждого будет свой экземпляр.  
- **application** — создаётся один экземпляр **на весь ServletContext** (веб-приложение).  
  → Используется только в веб-контексте и общая для всех Spring ApplicationContext, связанных с этим ServletContext.
ID: 1760612201099
END

START
math_basic_single
FRONT: Примеры бизнес-использования scope `prototype` в Spring
BACK:
Примеры, когда `prototype` оправдан:
1. **Объекты с уникальным состоянием** — например, генерация отчёта или обработка конкретного запроса пользователя, где у каждого экземпляра свой набор данных.  
2. **DTO-конвертеры или билдеры**, которые накапливают состояние при построении ответа, но не должны шариться между потоками.  
3. **Модели расчётов** — например, расчёт стоимости кредита, где каждый объект содержит свои входные параметры.  
4. **Временные сервисы**, создаваемые под задачу (например, генератор токенов или PDF-документов), которые живут короткое время.  
5. **Интеграции с legacy-кодом**, где объект должен быть «чистым» при каждом использовании (например, Stateful клиент внешнего API).
ID: 1760612201106
END

START
math_basic_single
FRONT: Основное различие между @RestController и @Controller в Spring
BACK: @Controller возвращает view (HTML/шаблон) и требует @ResponseBody для JSON; @RestController = @Controller + @ResponseBody, всегда возвращает данные прямо в HTTP-ответ (обычно JSON).
ID: 1760610845094
END