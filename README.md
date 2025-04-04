# Анализ данных о задержках рейсов в Аляске и Техасе

Этот проект посвящен анализу данных о задержках авиарейсов в двух штатах США: Аляске и Техасе. Целью является сравнение количества задержек в разных климатических условиях и выявление зависимости задержек от различных факторов, таких как сезонность и особенности региона.

## Описание данных

- **Источники данных**: [Bureau of Transportation Statistics](https://www.transtats.bts.gov/OT_Delay/OT_DelayCause1.asp?20=E&fry=N&Nv42146=QSj&Nv42146_anzr=Qnyyn5/S146%20j146u,%20gk:%20Qnyyn5/S146%20j146u%20V06r40n6v10ny).
- **Период**: Январь 2020 - Декабрь 2024.
- **Данные**: Содержат информацию о задержках рейсов в двух международных аэропортах — аэропорте Анкориджа в Аляске и аэропорте Даллас/Форт-Уэрт в Техасе. Для анализа используется информация о количестве задержек рейсов по месяцам.
- **Ключевое различие**: Аляска — северный штат с холодным климатом, Техас — южный штат с теплым климатом. Это может оказывать влияние на количество задержек.

## Задачи

1. **Предобработка данных**:
    - Извлечение данных из CSV файлов.
    - Преобразование данных для анализа (суммирование количества задержек по месяцам).
  
2. **Статистический анализ**:
    - Расчет основных статистических показателей для каждой выборки (минимум, максимум, математическое ожидание, дисперсия и т. д.).
  
3. **Визуализация данных**:
    - Построение гистограмм, графиков распределений, коробчатых графиков (boxplot) и QQ-plot для оценки нормальности распределения данных.
    - Анализ сезонных изменений и вариативности задержек.

## Структура репозитория

- `alyaska.csv`: Данные о задержках рейсов для Аляски.
- `texas.csv`: Данные о задержках рейсов для Техаса.
- `analysis.ipynb`: Основной ноутбук, содержащий код для анализа данных.
- `a_data.csv`: Обработанные данные о задержках для Аляски (после фильтрации и преобразования).
- `t_data.csv`: Обработанные данные о задержках для Техаса (после фильтрации и преобразования).


## Результаты

1. **Статистический анализ**:
    - Сравнение основных статистик задержек для Аляски и Техаса.
    - Выявлены значительные различия в среднем числе задержек, дисперсии и сезонных колебаниях.
  
2. **Графики**:
    - Гистограммы, показывающие распределение задержек.
    - Эмпирические функции распределения (ECDF) для оценки характера распределения.
    - Коробчатые графики (boxplot) для сравнения варьируемости данных.
    - QQ-plot для проверки нормальности распределения.

3. **Выводы**:
    - Задержки в Техасе значительно выше, с меньшей вариативностью и устойчивым сезонным характером.
    - В Аляске задержки более переменные, что может быть связано с погодными условиями и меньшей загруженностью аэропортов.

