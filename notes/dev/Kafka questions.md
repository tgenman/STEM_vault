---
aliases:
created: 2025-10-16 13:19
parent:
  - "[[root dev questions]]"
connected:
tags:
---
TARGET DECK: stem::dev::kafka
START
math_basic_single
FRONT: Что такое Topic в Kafka?
BACK: Topic — логическая очередь сообщений (поток событий), на которую продюсеры публикуют данные и с которой потребители их считывают. Разбивается на партиции для параллельной обработки.
ID: 1760615581928
END

START
math_basic_single
FRONT: Что такое Partition в Kafka?
BACK: Partition — физическая часть топика, в которой сообщения упорядочены по offset. Обеспечивает масштабируемость и параллелизм: разные партиции могут читаться разными потребителями.
ID: 1760615581933
END

START
math_basic_single
FRONT: Что такое Offset в Kafka?
BACK: Offset — порядковый номер сообщения внутри партиции, определяющий позицию чтения. Kafka сохраняет offset для каждой consumer group, чтобы знать, откуда продолжить чтение.
ID: 1760615581936
END

START
math_basic_single
FRONT: Что такое Producer в Kafka?
BACK: Producer — приложение, отправляющее сообщения в определённый топик (и партицию). Может выбирать партицию по ключу или случайно, если ключ не задан.
ID: 1760615581940
END

START
math_basic_single
FRONT: Что такое Consumer в Kafka?
BACK: Consumer — приложение, читающее сообщения из топика. Работает в составе consumer group и получает одну или несколько партиций для обработки.
ID: 1760615581944
END

START
math_basic_single
FRONT: Что такое Consumer Group в Kafka?
BACK: Consumer group — группа потребителей, совместно читающих топик. Каждая партиция может обрабатываться только одним consumer’ом внутри группы, что позволяет балансировать нагрузку.
ID: 1760615581948
END

START
math_basic_single
FRONT: Как связаны Topic, Partition, Producer и Consumer в Kafka?
BACK: Producer пишет сообщения в Topic (в конкретную Partition). Consumer group читает эти Partition; каждая Partition обрабатывается ровно одним Consumer внутри группы.
ID: 1760615581952
END

START
math_basic_single
FRONT: Что такое Replication в Kafka?
BACK: Replication — механизм дублирования партиций на нескольких брокерах для отказоустойчивости. Один брокер хранит leader-копию, остальные — follower.
ID: 1760615581956
END

START
math_basic_single
FRONT: Что такое Broker в Kafka?
BACK: Broker — сервер Kafka, хранящий партиции и обрабатывающий запросы от продюсеров и консумеров. Кластер состоит из нескольких брокеров.
ID: 1760615581960
END

START
math_basic_single
FRONT: Как Kafka обеспечивает параллелизм при обработке сообщений?
BACK: Параллелизм достигается за счёт партиционирования топика: разные партиции читаются разными консумерами в группе, что позволяет масштабировать обработку сообщений.
ID: 1760615581964
END
