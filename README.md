# Автоматизация подбора персонала 

### Результаты работы

- [Ноутбук](https://github.com/aefrt/automatization-recruiting/blob/main/scraping.ipynb)
- [Таблица с запросами](https://github.com/aefrt/automatization-recruiting/blob/main/resumes_all.csv)
- [Таблица с признаками](https://github.com/aefrt/automatization-recruiting/blob/main/resumes_features.csv)

### Прогресс

**Что сделано к 9.11:**

- Полностью готов скрейпер страницы с вакансиями. Он оформлен в отдельную аккуратную функцию, добавлена возможность перевода запроса на русском в транслит (в виде транслита он нужен для задания ссылки на выдачу), запущен скрейпер на всех 7 видах аналитиков и собраны вакансии по первым 10 страницам по каждому из 7 запросов, переделана часть кода для задания нормальных индексов в таблице (теперь это происходит уже после самого процесса скрейпинга).
- Скрейпинг отдельных резюме. Тоже создана отдельная функция для скрепинга, обнаружены ситуации, когда предыдущий код выдавал ошибку, и исправлены, теперь все должно работать исправно на любых резюме, переделан принцип обработки пропущенных данных. *Добавлен скрейпинг признаков ...*. Скрейпер собрал признаки для первых 100 собранных ссылок на вакансии в таблицу (так мало, поскольку пока мы просто тестируем его работу). 

### Что надо сделать

- *Разобраться с документами для ВКР (дедлайн: 20 ноября)*
- В скрейпинг запросов добавить возможность добавлять новые данные без удаления старых
- В скрейпинг запросов добавить возможность получить количество страниц на странице с запросом (сейчас он так не умеет и собирает фиксированно 10 страниц, что может приводить к ошибкам или сбору не всех данных)
- *В скрейпинг фичей?...*

### Как работать с `git`?

1. `git commit -m "Message" -a` ('-a', чтобы добавить все изменения)

2. `git push origin main`

3. Maybe: `git pull origin main` (если были внесены изменения на GitHub, и теперь их надо скачать удаленно)
