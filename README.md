# OsvDistribution

Этот репозиторий содержит python-скрипт для распределения ОСВ (оборотно-сальдовые ведомости) нескольких компаний по папкам в соответствии с периодом, по которому они сформированы и их загрузки в базу данных PostgreSQL. В качестве исходных данных можно использовать ОСВ любого счёта из 1С за прошлый месяц и текущий день. При запуске скрипта "osv_distribution_by_folders.ipynb" все исходные файлы загружаются в БД. Если при повторном запуске скрипта исходные данные за аналогичный период, то они перезаписываются в БД.

## Использование

Сначала необходимо создать папку, например, "Исходные данные". Далее в папку поместить файлы с исходными данными из 1С с названием "предыдущий месяц_ОСВ_счёт в 1С_Название компании (XLSX)" и "текущий день_ОСВ_счёт в 1С_Названии компании (XLSX)". Далее запустить скрипт "osv_distribution_by_folders.ipynb". В результате выполнения скрипта будет создана папка с годом и месяцем, в которой появятся файлы для дальнейшей загрузки в базу данных PostgreSQL.

### Используемые технологии

Для подключения к PostgreSQL в переменной "db_config" в скрипте необходимо указать параметры подключения.

### Используемые технологии

- Python

### Автор

Пушин Илья

### Лицензия

MIT License
