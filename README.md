# DS-SF-EDA--HR-
Проект в рамках обучения в SF на DS.
## Исследования для HR-агентства
## Постановка задачи  
HR-агентство изучает тренды на рынке труда в IT. Необходимо провести исследование на основе данных о зарплатах в сфере Data Science за 2020–2022 годы.  
Вопросы:  
1. Выяснить, какие факторы влияют на зарплату специалиста Data Scientist.
2. Ответить на ключевые вопросы HR-агентства:
- Наблюдается ли ежегодный рост зарплат у специалистов Data Scientist?
- Как соотносятся зарплаты Data Scientist и Data Engineer в 2022 году?
- Как соотносятся зарплаты специалистов Data Scientist в компаниях различных размеров?
- Есть ли связь между наличием должностей Data Scientist и Data Engineer и размером компании?
 
 Использовать разные тесты для проверки статистической значимости сделанных выводов:

- тесты для количественного признака:
    - для одной выборки;
    - для двух выборок;
    - для нескольких выборок;
- тест для категориальных признаков.
Данные содержат следующие столбцы:  
- work_year	- Год, в котором была выплачена зарплата  
- experience_level	- Опыт работы на этой должности в течение года со следующими возможными значениями:  
    - EN — Entry-level/Junior;  
    - MI — Mid-level/Intermediate;   
    - SE — Senior-level/Expert;  
    - EX — Executive-level/Director.  
- employment_type - Тип трудоустройства для этой роли:
    - PT — неполный рабочий день;  
    - FT — полный рабочий день;  
    - CT — контракт;  
    - FL — фриланс.  
- job_title	- Роль, в которой соискатель работал в течение года.  
- salary - Общая выплаченная валовая сумма заработной платы.  
- salary_currency -	Валюта выплачиваемой заработной платы в виде кода валюты ISO 4217.  
- salary_in_usd	- Зарплата в долларах США (валютный курс, делённый на среднее значение курса доллара США за соответствующий год через fxdata.foorilla.com).  
- employee_residence - Основная страна проживания сотрудника в течение рабочего года в виде кода страны ISO 3166.  
- remote_ratio - Общий объём работы, выполняемой удалённо. Возможные значения:
    - 0 — удалённой работы нет (менее 20 %);  
    - 50 — частично удалённая работа;  
    - 100 — полностью удалённая работа (более 80 %).  
- company_location - Страна главного офиса работодателя или филиала по контракту в виде кода страны ISO 3166.  
- company_size - Среднее количество людей, работавших в компании в течение года:  
    - S — менее 50 сотрудников (небольшая компания);  
    - M — от 50 до 250 сотрудников (средняя компания);  
    - L — более 250 сотрудников (крупная компания).
      Источник датасета: [“Data Science Job Salaries” (kaggle.com)](https://www.kaggle.com/datasets/ruchi798/data-science-job-salaries)

      ## В работе проведен описательный анализ данных, сделаны предварительыне выводы.
      ## Проведены тесты:
      * критерий Краскела-Уоллиса
      * U-критерий Манна — Уитни
      * критерий ${\chi}^2$ (хи-квадрат)
      * Двухвыборочный t-критерий
