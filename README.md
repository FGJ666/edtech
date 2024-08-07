# edtech
## A/B тестирования и SQL

**Цель:** 
- Проанализировать результаты A/B теста, проведенного для новой механики оплаты.
- Написать SQL запросы для получения информации о пользователях и их поведении.

**Структура репозитория:**

```
├── data
│   ├── active_studs.csv
│   ├── checks.csv
│   ├── groups.csv
│   └── groups_add.csv
└── test_and_sql.ipynb

```

**Описание файлов:**

- `test_and_sql.ipynb`: Jupyter Notebook с решением задания. 
- `data/`: Папка с данными:
    - `groups.csv`: Информация о принадлежности пользователя к контрольной (A) или тестовой (B) группе.
    - `groups_add.csv`: Дополнительный файл с информацией о пользователях.
    - `active_studs.csv`: Информация о пользователях, заходивших на платформу во время эксперимента.
    - `checks.csv`: Информация об оплатах пользователей во время эксперимента.

**Описание решения:**

**A/B тестирование:**

1. **Загрузка и подготовка данных:** Объединение данных из всех файлов, обработка пропусков, создание dummy-переменных.
2. **Анализ данных:** 
    - Расчет ключевых метрик (конверсия, средний чек) для контрольной и тестовой групп.
    - Визуализация распределений метрик.
    - Проверка статистических гипотез для определения значимости различий между группами.
3. **Выводы:** На основе анализа данных делаем выводы о том, стоит ли запускать новую механику оплаты на всех пользователей.

**SQL запросы:**

1.  Написать запрос для определения количества "очень усердных студентов" (тех, кто решил более 20 задач за месяц).
2.  Написать запрос для расчета ARPU, ARPAU, CR и других метрик для пользователей, разделенных на группы.

**Инструкции по запуску:**

1. Склонируйте репозиторий: `git clone https://github.com/ваш_логин/test_task.git`
2. Откройте Jupyter Notebook `test_and_sql.ipynb`
3. Запустите все ячейки для просмотра решения.


**Используемые библиотеки:**

- `pandas`
- `numpy`
- `matplotlib`
- `seaborn`
- `pingouin`
- `scipy`
- `requests`
- `urllib`
- `json`
- `pandahouse`
