# DE or DIE #5

Дата мероприятия: 24.12.2020.  
Формат мероприятия: online.

## Доклады

### Использование Scala UDF в PySpark

_Автор: Андрей Титов, Senior Spark Engineer, NVIDIA._

Материалы первого доклада:

- [Запись](https://youtu.be/eHcJPWTh2oU) выступления на YouTube.
- [Презентация](Andrey%20Titov%20–%20Advanced%20usage%20patterns%20of%20Scala%20UDF%20in%20PySpark.pdf) в формате PDF.

#### О чем первый доклад

В своем докладе я поделюсь своим опытом использования пользовательских функций в высокопроизводительных PySpark приложениях.

При использовании PySpark часто забывают о возможности использования UDF, написанных на Scala/Java. А ведь это отличный способ увеличить производительность вашего приложения.

К сожалению, в официальной документации приводится самый базовый вариант их применения, который  имеет ряд ограничений и не раскрывает всех возможностей применения Scala/Java UDF в PySpark.

В своем докладе я расскажу, как:

- заставить PySpark автоматически выводить тип данных, возвращаемых в UDF;
- создать pyspark.sql.Column на базе UDF вместо использования spark.sql(…);
- использовать Singleton Pattern для сохранения данных между вызовами функций и работы с внешними источниками из UDF;
- избежать повторного вызова UDF на одних и тех же данных;
- настроить логирование с помощью встроенного log4j.

### Мой первый Data Lake

_Автор: Дмитрий Шалин, Data Engineer, СБЕР._

Материалы второго доклада:

- [Запись](https://youtu.be/pIbNThAtFdA) выступления на YouTube.
- [Презентация](Dmitry%20Shalin%20–%20My%20first%20Data%20Lake.pdf) в формате PDF.
- [Демо](https://github.com/Shldm/de_mit). Код создания ETL + примеры контроля качества, про которые рассказывается в докладе.

#### О чем второй доклад

Если зайти в YouTube и забить data lake, получим большое количество докладов от сотрудников крупных компаний, которые имеют в своем арсенале большие деньги, широкую экспертизу, численность под реализацию end-to-end процесса работы с данными и самое главное – время.

В своем докладе я расскажу историю, как будучи сотрудником стартапа, в сжатые сроки, как и главное зачем, собирал хранилище и какие шаги позволили избежать проблемы масштабирования в будущем. Покажу по шагам (1,2,3) как уже в первую неделю, не имея глубоких знаний языка программирования, хранилищ, облачных сервисов, заложить фундамент.

Основное внимание будет уделено базе по ETL, качеству (как идеи, что это часть ETL) и основам баз данных.