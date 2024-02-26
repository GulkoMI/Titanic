# Titanic

🎯***Цель:*** данное исследование предполагает построение модели для решения задачи классфикации выживших/не выживших пассажиров парахода "Титаник", в зависимости от их индивидуальных особенностей

__Данные: https://www.kaggle.com/competitions/titanic/overview__

📅***Стадии решения:***
1. Загрузка данных
2. Разведочный анализ (EDA)
3. Предварительная обработка данных (Preprocessing)
4. Обучение моделей и прогнозирование класса на основе тестовой выборки

📚***Убедитесь, что у вас установлены все библиотеки, необходимые для реализации проекта:***
```python
pip install matplotlib
pip install pandas
pip install numpy
pip install seaborn
pip install plotly
pip install scikit-learn
```
## ℹ️Ознакомительная информация 

Все этапы решения проекта подробно описаны и проккоментированы в файле [Titanic](Titanic.ipynb)
### Использованные модели классификации: 
- Logistic regression
- Logistic regression with RFECV
- Decision tree
- Random forest
- XGBoost
- LightGBM
- CatBoost
- Gradient Boosting

### 📈Использованные метрики оценки:

- Accuracy
- F1
- Roc Auc

## Результаты

| Модель                     | Accuracy | F1        | Roc Auc   |
|----------------------------|----------|-----------|-----------|
| Logistic regression        | 0.854962 | 0.813725  | 0.891797  |
| Logistic regression with RFECV | 0.858779 | 0.817734  | 0.876746  |
| Decision tree              | 0.854962 | 0.808081  | 0.870930  |
| Random forest              | 0.843511 | 0.798030  | 0.873928  |
| XGBoost                    | 0.854962 | 0.808081  | 0.883462  |
| LightGBM                   | 0.854962 | 0.808081  | 0.891647  |
| CatBoost                   | 0.843511 | 0.793970  | 0.878605  |
| Gradient Boosting          | 0.854962 | 0.808081  | 0.887270  |

## Вывод

- Исследование успешно завершено, и его цель была полностью достигнута. В ходе выполнения проекта были выполнены все этапы решения задачи.
- Модель логистической регрессии выделяется среди остальных как лучшая. Она достигла наивысшего значения метрики ROC AUC, хотя в метриках Accuracy и F1 она заняла второе место. Помимо этого логистическая регрессия имеет несколько преимуществ по сравнению с другими моделями:
1. Простота интерпретации
2. Меньше склонна к переобучению
3. Высокая скорость выполнения
4. Демонстрирует хорошие показатели даже без необходимости подбора гиперпараметров методом RandomizedSearchCV
