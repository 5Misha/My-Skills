# Мой практический опыт работы в Data Science

Чуть ниже находится основная краткая информация, представленная в виде таблицы, про мои проекты.
Табличка состоит из ткаих столбцов как:
* Номер проекта с сылкой на папку проекта с его описанием
* Название проекта
* Уровень сложности проекта - это оценка по моему субъективному мнению, которая зависит от кол-ва шагов,
  использованных библиотек, инструментов, функций и т.п. в проекте. Диапазон оценивания от 1 до 3. Чем больше число, тем сложнее проект.
* Задача проекта
* Инструменты, используемые в проекте

| № | Название | Сложность | Задача                                                                                | Инструменты                                                               |
| -- | ----- | -- | ------------------------------------------------------------------------------------- | ---------------------------------------------------------------------------------- |
| 1   | [Анализ<br/>видеоигр](https://github.com/5Misha/My-Skills/tree/main/Анализ_видеоигр) | 1 | С помощью данных о продажах, оценках и жанрах игр нужно провести исследовательский анализ, проверить гипотезы, составить портрет каждого пользователя в разных регионах. Найти причины, которые помогают играм стать популярными, чтобы предугадать потенциально популярный продукт | import pandas as pd import numpy as np import missingno as msno import matplotlib.pyplot as plt from scipy import stats as st 
| 2  | [Анализ сервиса аренды самокатов GoFast](https://github.com/5Misha/My-Skills/tree/main/Аренда_самокатов) | 1 | У нас есть данные популярного сервиса аренды самокатов GoFast о некоторых пользователях из разных городов,а также об их поездках. Нужно проанализировать данные и проверить некоторые гипотезы, которые могут помочь бизнесу вырасти. Узнать, есть ли отличия между информацией от людей, которые купили подписку, и тех, кто этого не сделал. | os, pandas, numpy, scipy.stats, binom, poisson, matplotlib, math, scipy |
| 3 | [Выбор локации для скважины](https://github.com/5Misha/My-Skills/tree/main/Выбор_локации_скважины) | 1 | Нам предоставлены пробы нефти в трёх регионах и их характеристики для каждой скважины. Нужно построить модель для определения региона, где добыча принесёт наибольшую прибыль, и проанализировать возможную прибыль и риски техникой Bootstrap. Это поможет выбрать лучший регион для бурения новых скважин, который будет удовлетворять условиям... | pandas, numpy, seaborn, matplotlib.pyplot, sklearn.linear_model, train_test_split, LinearRegression, StandardScaler, mean_squared_error | 
| 4 | [Цены квартир в Санкт-Петербурге](https://github.com/5Misha/My-Skills/tree/main/Квартиры_Питера) | 1 | С помощью данных сервиса Яндекс.Недвижимость определить рыночную стоимость объектов недвижимости и найти их интересные особенности и зависимости. | pandas |
| 5 | [Оптимизация управления персоналом для компании "Работа с заботой"](https://github.com/5Misha/My-Skills/tree/main/Откат_сотрудников)| 1 | Первая — построить модель, которая сможет предсказать уровень удовлетворённости сотрудника на основе данных заказчика. Вторая задача — построить модель, которая сможет на основе данных заказчика предсказать то, что сотрудник уволится из компании | pandas, numpy, matplotlib.pyplot, seaborn, from phik import resources, report, Pipeline, OneHotEncoder, OrdinalEncoder, StandardScaler, MinMaxScaler,, LabelEncoder, ColumnTransformer, SimpleImputer, RandomizedSearchCV, Regression, KNeighbors, DecisionTree, SVC, make_scorer, roc_auc_score |
| 6 | [Оценка стоимости автомобилей](https://github.com/5Misha/My-Skills/tree/main/Оценка_авто)| 1 | На основе имеющихся данных требуется разработать модель, способную прогнозировать цену автомобиля на основе его характеристик. Это обеспечит удобство при продаже или покупке автомобилей и поспособствует привлечению новых клиентов | pandas, numpy, matplotlib.pyplot, seaborn, scipy, os, DecisionTreeRegressor, LinearRegression, LGBMRegresso, train_test_split, GridSearchCV, StandardScaler, OneHotEncoder, OrdinalEncoder, make_scorer, mean_squared_error, mean_squared_error, cross_val_score, KFold, time, DummyRegressor |
| 7 | [Персонализированные предложения для клиентов интернет-магазина «В один клик»](https://github.com/5Misha/My-Skills/tree/main/Персональные_предложения)| 1 | Помочь сохранить интернет-магазину "В один клик" сохранить клиентов с помощью разработанной модели для предсказания вероятности снижения покупательской активности и с помощью предложений, сформированных на данных, для выгодных персональных предложений клиентам | pandas, seaborn, scipy, scikit-learn, numpy, kendalltau, ColumnTransformer, Pipeline, OptunaSearchCV, OneHotEncoder, OrdinalEncoder, StandardScaler, SimpleImputer, MinMaxScaler, RandomizedSearchCV, DecisionTreeClassifier, LogisticRegression, SVC, KNeighborsClassifier, roc_auc_score, accuracy_score, f1_score, optuna, optuna-integration, shap | 
