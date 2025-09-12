# itpm-statistical-helpers
Учебный проект по управлению ИТ-проектами. Коллективная разработка Python-пакета для статистического анализа.
# Statistical Helpers (itpm-statistical-helpers)

Учебный проект по курсу "Управление ИТ-проектами". Цель проекта — коллективная разработка Python-пакета для базового статистического анализа данных с использованием полного цикла Git/GitHub workflow.

## 🎯 Цель проекта

На практике освоить инструменты и процессы коллективной разработки:
1.  Работа с Git (ветки, коммиты, слияние).
2.  Работа с GitHub (Fork, Issues, Pull Requests, Code Review).
3.  Написание тестируемого и документированного кода.
4.  Настройка CI/CD (автоматические тесты).

## 📋 Список задач (To-Do)

Каждый студент должен выбрать **одну задачу** из списка ниже, реализовать ее и оформить Pull Request. Задачи представлены в виде GitHub Issues.

**Общий список функций для реализации:**

*   `mean(data: list) -> float` - Среднее арифметическое.
*   `median(data: list) -> float` - Медиана.
*   `mode(data: list) -> list` - Мода (список наиболее частых значений).
*   `variance(data: list, sample: bool = True) -> float` - Дисперсия.
*   `std_dev(data: list, sample: bool = True) -> float` - Стандартное отклонение.
*   `correlation(x: list, y: list) -> float` - Корреляция Пирсона.
*   `confidence_interval(data: list, confidence: float = 0.95) -> tuple` - Доверительный интервал.
*   `hypothesis_ttest(sample1: list, sample2: list) -> tuple` - T-тест для двух выборок.
*   `simple_linear_regression(x: list, y: list) -> tuple` - Простая линейная регрессия (угол наклона и intercept).
*   `load_dataset_from_csv(filename: str) -> list` - Загрузка данных из CSV.
*   `create_histogram(data: list, filename: str = "histogram.png")` - Построение гистограммы.
*   `create_boxplot(data: list, filename: str = "boxplot.png")` - Построение boxplot.

**Внимание!** Перед началом работы **найдите нужную Issue в разделе "Issues"** и оставьте комментарий "I'm working on this", чтобы закрепить задачу за собой.

## 🚀 Инструкция по работе (Workflow)

1.  **Fork:** Нажмите кнопку "Fork" в правом верхнем углу этого репозитория. Это создаст его полную копию в вашем аккаунте на GitHub.
2.  **Clone:** Склонируйте **ваш форк** на локальный компьютер:
    `git clone https://github.com/ВАШ_АККАУНТ/itpm-statistical-helpers.git`
3.  **Branch:** Создайте новую ветку для вашей задачи. Назовите ее понятно, например `feature/mean-calculation`:
    `git checkout -b feature/name-of-your-feature`
4.  **Code:** Реализуйте свою функцию в файле `statistical_helpers/helpers.py`. Не забудьте написать документацию (docstring) и тесты в `tests/test_helpers.py`.
5.  **Commit:** Закоммитьте изменения с осмысленным сообщением:
    `git add .`
    `git commit -m "feat: add mean function with tests"`
6.  **Push:** Отправьте вашу ветку в **ваш форк** на GitHub:
    `git push origin feature/name-of-your-feature`
7.  **Pull Request (PR):**
    *   На сайте GitHub в **вашем форке** перейдите в раздел "Pull requests".
    *   Нажмите "New pull request".
    *   В качестве `base repository` выберите **ЭТОТ репозиторий** (`ваше_имя/itpm-statistical-helpers`), а `base` — ветку `main`.
    *   В качестве `head repository` выберите **ВАШ форк**, а `compare` — вашу новую ветку.
    *   Опишите, что вы сделали. Ссылайтесь на номер Issue (например, `Closes #5`).
    *   Нажмите "Create pull request".

## 🧪 Требования к коду

*   Код должен быть написан на Python.
*   Функции должны быть размещены в файле `statistical_helpers/helpers.py`.
*   **Обязательно** должны быть написаны тесты (используем `pytest`) в файле `tests/test_helpers.py`.
*   **Обязательно** наличие документации (docstring) для каждой функции по стандарту (например, Google Style).
*   Код должен быть чистым и читаемым (рекомендуется использовать линтер, например `flake8`).

## 📝 Лицензия

Этот проект распространяется под лицензией MIT. Подробнее см. в файле `LICENSE`.
