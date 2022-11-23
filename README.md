# Автоматизация подбора персонала 

### Результаты работы

- [Ноутбук](https://github.com/aefrt/automatization-recruiting/blob/main/scraping.ipynb)
- [Таблица с запросами](https://github.com/aefrt/automatization-recruiting/blob/main/resumes_all.csv)
- [Таблица с признаками](https://github.com/aefrt/automatization-recruiting/blob/main/resumes_features.csv)

### О работе

Проект на стыке текстовой и HR-аналитики.

### Прогресс

**Что сделано к 23.11:**

- ...

**Что сделано к 16.11:**

- Исправил странность с образованием (это было из-за конфликта имен)
- Научил первый скрейпер собирать количество страниц
- Собрал все данные обоими скрейперами
- Опыт работы: число + 1–2 работа — добавил эти признаки
- Написан простой вариант функции для добавления новых данных к старым (могут ли быть ошибки? будет ли это долго?)

**Что сделано к 9.11:**

- Полностью готов скрейпер страницы с вакансиями. Он оформлен в отдельную аккуратную функцию, добавлена возможность перевода запроса на русском в транслит (в виде транслита он нужен для задания ссылки на выдачу), запущен скрейпер на всех 7 видах аналитиков и собраны вакансии по первым 10 страницам по каждому из 7 запросов, переделана часть кода для задания нормальных индексов в таблице (теперь это происходит уже после самого процесса скрейпинга).
- Скрейпинг отдельных резюме. Тоже создана отдельная функция для скрепинга, обнаружены ситуации, когда предыдущий код выдавал ошибку, и исправлены, теперь все должно работать исправно на любых резюме, переделан принцип обработки пропущенных данных. Добавлен скрейпинг признаков названия вакансии, а также 4 признаков, связанных с образованием, начата работа над справочником вузов. Скрейпер собрал признаки для первых 100 собранных ссылок на вакансии в таблицу (так мало, поскольку пока мы просто тестируем его работу). 

### Что надо сделать?

- *Разобраться с документами для ВКР (дедлайн: 20 ноября)* и названием
- В скрейпинг запросов добавить возможность добавлять новые данные без удаления старых. В скрейпинг фичей также добавить возможность обновления таблицы с сохранением предыдущих данных (простой способ уже написан, нужен ли более сложный? после него надо еще не забывать править индексы)
- В скрейпинг фичей добавить справочник образований, топовость итд. См звонок 16.11.
- Дособирать данные с использованием п. 2.
