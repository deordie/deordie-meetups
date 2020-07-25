# DE or DIE #3

Дата мероприятия: 16.07.2020.  
Формат мероприятия: online.

## Доклады

### Разбор реального проекта: E2E пайплайн для прогнозирования закупок ингредиентов в пиццериях c помощью Spark Streaming

_Авторы:  
Ксения Томак, Дарья Буланова, Михаил Кумачев, Data Engineering Team, Dodo Pizza  
Иван Трусов, Solutions Architect, Databricks_

Материалы доклада:

- [Запись](https://youtu.be/OQv61WY_f88) выступления на YouTube.
- [Презентация](Dodo%20Pizza%20%26%20Databricks%20-%20Real%20project%20analysis.pdf) в формате PDF.
- [Демо](Spark%20Streaming%20Demo.ipynb). Jupyter notebook с примерами кода (Spark Streaming).

#### О чем первый доклад

Dodo Pizza совместно с Databricks сделали проект по решению задачи прогнозирования закупок ингредиентов в пиццериях. В рамках проекта был разработан набор near real-time и batch пайплайнов для сбора данных из источника, загрузки их в Delta Lake и подготовки витрин для использования в машинном обучении.

В рамках нашего выступления мы подробно разберем каждый из этапов и уделим особое внимание подводным камням при реализации проекта.

Часть 1:

- Описание проекта и базовой инфраструктуры
- Архитектура решения
- Change Data Capture из MySQL в EventHubs, используя Kafka Connect и Debezium

Часть 2:

- Data modeling с помощью DataVault 2.0. Переливка данных с помощью Spark Streaming
- Наполнение витрин данных
- Интеграция с ML-пайплайнами
- CI/CD для пайплайнов данных

#### Стек используемых технологий

- Cloud provider: Azure
- Data Source: Azure MySQL DB
- CDC pipeline: Kafka Connect + Debezium + Azure Event Hubs
- Processing: Spark + Spark Streaming on Databricks
- Storage layer: Delta Lake + Azure Data Lake Storage
- CI/CD: GitHub Actions + Databricks REST API
- Implementation language: Python
