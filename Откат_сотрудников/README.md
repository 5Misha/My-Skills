# Оптимизация управления персоналом для компании "Работа с заботой"
https://github.com/5Misha/My-Skills/blob/main/Откат_сотрудников/Откат_сотрудников.ipynb 

## Задача проекта
Первая — построить модель, которая сможет предсказать уровень удовлетворённости сотрудника на основе данных заказчика.
Вторая задача — построить модель, которая сможет на основе данных заказчика предсказать то, что сотрудник уволится из компании

## Используемые интсрументы
pandas, numpy, matplotlib.pyplot, seaborn  
from phik import resources, report  
Pipeline  
OneHotEncoder, OrdinalEncoder, StandardScaler, MinMaxScaler, LabelEncoder  
ColumnTransformer, SimpleImputer, RandomizedSearchCV  
Regression, KNeighbors, DecisionTree, SVC  
make_scorer, roc_auc_score  

## Используемые функции 
* analiz - для вывода различной информации о таблице
* optimize_memory_usage - для оптимизации числовых типов данных
* numbers_plot - функция для построения гистограмм и ящиков с усами для каждого признака
* kategory_col - для зображения категориальных признаков в виде столбчатых диаграмм
* smape - для создания новой метрики
* best_model - при передаче трех датафреймов находит лучшую модель и считает метрику (пайплайн)

## Основные шаги
### Задача 1
* Предобработка данных  
* Исследовательский анализ данных
* Корреляционный анализ
* Создание пайплайна

### Задача 2
* Предобработка данных  
* Исследовательский анализ данных
* Анализ признаков
* Портрет уволившегося сотрудника
* Проверка влияния job_satisfaction_rate на новый целевой признак
* Добавление нового признака
* Создание пайплайна

## Общий вывод
Проект выдался большим, так как состоял из двух частей. Первая - предсказание уровня удовлетворённости сотрудника. Вторая - предсказание увольнения сотрудника из компании. Для этого нужно было получить две итоговые модели разных типов. Одна - модель регрессии, а другая - классификации. И во всех была проведена предобработка данных, исследовательский анализ, содержащий столбчатые, круговые диаграммы и ящики с усами. Была создана новая метрика - SMAPE (симметричное среднее абсолютное процентное отклонение). Во второй задаче был создан портрет уволившегося сотрудника, то есть по худшим показателям графиков описывался человек, работащий в компании. Еще был добавлен новый выявленный признак, который помог улучшить итоговую метрику. Дальше шел корреляционный анализ, осуществляемый с помощью scatter, где были выделены сегменты другим цветом, и phik_matrix. Ну и наконец создавался пайплайн. В обеих моделях были использованы модели с перебором различных гиперпараметров регрессии, дерева решений и метод ближайших соседей. Во второй задаче добавился еще и SVC. Предложения компании получились такими: для уменьшения кол-ва увольнений, компании "Работа с заботой" можно посоветовать увеличить зарплату, но это может быть не так прибыльно, поэтому нужно повысить уровень удовлетворённости сотрудника работой в компании, так как от этого признака больше всего зависит будущее сотрудника. Это можно сделать с помощью увеличения длительности работы сотрудников. Их нужно как-то заманивать оставаться подольше в компании, чем дольше человек находится в компании, тем вероятнее, что он останется подольше. Еще можно чаще повышать своих сотрудников. Данные признаки неплохо связаны с job_satisfaction_rate, а сам признак с целевым quit.
