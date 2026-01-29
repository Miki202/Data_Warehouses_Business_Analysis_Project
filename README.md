# Проект по Складове от данни и Бизнес Анализ

![PostgreSQL](https://img.shields.io/badge/PostgreSQL-316192?style=for-the-badge&logo=postgresql&logoColor=white)
![Power BI](https://img.shields.io/badge/Power%20BI-F2C811?style=for-the-badge&logo=powerbi&logoColor=black)
![Neon](https://img.shields.io/badge/Neon-00C7B7?style=for-the-badge&logo=data:image/svg+xml;base64,PHN2ZyB4bWxucz0iaHR0cDovL3d3dy53My5vcmcvMjAwMC9zdmciIHdpZHRoPSIxNiIgaGVpZ2h0PSIxNiIgdmlld0JveD0iMCAwIDE2IDE2Ij48cGF0aCBkPSJNOC4wMDUgMGMuMjQyIDAgLjQ4LjA5LjY2LjI2bDUuMDc0IDQuNjkzYy4zNC4zMTMuMzcuODIuMDYuMTE2bC0uMDAxLjAwMS0uMDAxLjAwMWMtLjMxLjM0LS44Mi4zNy0xLjE2LjA2bC00LjY5My01LjA3NGMtLjM4LS4zNi0uOTYtLjM2LTEuMzQgMGwtNC42OTMgNS4wNzRjLS4zNC4zMS0uODUuMjgtMS4xNi0uMDZsLS4wMDEtLjAwMS0uMDAxLS4wMDFjLS4zMS0uMzQtLjI4LS44NS4wNi0xLjE2bDUuMDc0LTQuNjkzYy4xOC0uMTcuNDItLjI2LjY2LS4yNnoiIGZpbGw9IiMwMUM3QjciLz48L3N2Zz4=)

## Какъв е този проект
Този проект се фокусира върху изграждането и анализа на Data Warehouse по метода на Kimball за набора от данни Berka, за да подпомогне бизнес процесите и вземането на стратегически решения. Той включва скриптове, схеми и данни за създаване и управление на Data Warehouse, както и анализ и визуализация на данните.

## Защо проектът е полезен
- **Централизирано управление на данни**: Консолидира данни от множество източници в единно хранилище.
- **Бизнес прозрения**: Позволява ефективно изпълнение на заявки и генериране на отчети за бизнес анализ.
- **Скалируема архитектура**: Осигурява основа за разширяване на операциите с данни според нуждите на бизнеса.

## Документация
Документацията `DW_Project_Documentation.docx` представлява описание на проекта като цяло, моделите и ETL процесът. Предоставени са и визуализация на данните, както и няколко репорта с бизнес цел.

## Как да започнете

### Предварителни изисквания
- **Система за управление на бази данни**: PostgreSQL 18 или съвместима база данни.
- **Инструменти**: SQL клиент (например pgAdmin, DBeaver) за взаимодействие с базата данни.

### Настройка на Neon PostgreSQL база данни
1. Проверете файла `secrets/Neon_Connection.json` за необходимите данни за свързване към базата данни.

2. Използвайте скрипта, предоставен в `DataWarehouse/bank_dw_neon.zip`, за да заредите данните в Neon PostgreSQL базата данни.

### Разархивиране на файлове с данни
Използвайте следните команди, за да разархивирате файловете с данни в съответните директории:

```bash
unzip Data/data_berka.zip -d Data/
unzip DataWarehouse/bank_dw_neon.zip -d DataWarehouse/
```

### Стартирайте скрипта с PostgreSQL клиент
Изпълнете следната команда, за да стартирате скрипта за създаване на базата данни:

```bash
psql -h $HOST -p $PORT -U $USERNAME -d $DATABASE -f DataWarehouse/create_script_local.sql
```

### Важни бележки
- Файлът `create_script_local.sql` съдържа ръчно добавени заявки за създаване на Data Warehouse. Възможно е да има грешки, затова прегледайте и валидирайте заявките преди да ги изпълните или използвайте neon скрипта.


## Екип
ФМИ, спец. "Анализ на данни"
- Михаела Папаринова
- Димана Маринова
- Силвия Войнска



