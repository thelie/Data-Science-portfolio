# Прогнозирование оттока клиентов банка

**Задача:**
По историческим данным поведения клиентов и расторжении договоров спрогнозировать возможный уход клиента.

**Использованные библиотеки:** 
Pandas, NumPy, Scikit-learn, Matplotlib, Catboost, различные модели классификации, подбор параметров, балансировка классов.

**Вывод:**
1. Наибольший результат получен с помощью классификатора `Catboost` с параметром автоматического вычисления весов для классов.
Второй по результату классификатор `RandomForestClassifier` с уменьшением в выборки доли отрицательных результатов, можно попробовать улучшить результат модели подбором параметров модели.
2. По результатам тестирования модели выделены две с наибольшими результатами. 
Это случайны лес `RandomForestClassifier`с уменьшением в выборке доли отрицательных результатов и CatBoost `CatBoostClassifier`. 
Обе модели показали значение F1-меры выше требуемого значения.
