---
tags: конспект
---
links: [[Лекция]], [[🗑Garbage Collection]]

---

[Владимир Иванов — G1 Garbage Collector](https://www.youtube.com/watch?v=iGRfyhE02lA)


- Слабая гипотеза о поколениях:
    - - большинство объектов временные
    - - старые объекты редко ссылаются на молодые
- Нетривиальное замечание:
    -  - сложность сборки мусора в молодом поколении не зависит от его размера, а зависит от объема данных в нем
- Характеристики производительности GC
    - - Throughput. объем вычислительных ресурсов на gc
    - - Предсказуемость. На какое время прерывает
    - - Footprint. Объем используемой памяти
- Можно выбрать только две характеристики
- Stop the World vs Инкрементальная сборка
- GC в Hotspot JVM
- - Serial GC
-     - последовательная сборка молодого и старого поколений
- - Parallel GC
-     - максимальный throughput
-     - параллельная сборка молодого и старого поколений
- - CMS
-     - предсказуемость
-     - по возможности, сборка мусора в фоновом режиме
- - G1
-     - предсказуемость
-     - слабо подвержен фрагментации
- 
- G1
- Три варианта сборки:
    - - только молодое
    - - смешанное
    - - full
- gchisto
