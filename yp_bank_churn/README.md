# Предсказание оттока клиентов

[Просмотр ноутбука](https://nbviewer.org/github/ootho/data_science/blob/main/yp_bank_churn/bank_churn.ipynb)   

Источник данных: [kaggle.com/barelydedicated/bank-customer-churn-modeling](https://www.kaggle.com/barelydedicated/bank-customer-churn-modeling)

## Цель и задачи проекта

Для проекта по анализу оттока клиентов из банка необходимо сделать прогноз, уйдет ли клиент в ближайшем будущем или нет. Имеются исторические данные о поведении клиентов и расторжении договоров с банком.

Нужно спрогнозировать, уйдёт клиент из банка в ближайшее время или нет.

## Вывод

**В процессе работы были проделаны следующие шаги:**
  - исходная выборка была подготовлена к работе;
  - модель была протестирована на несбалансированных данных;
  - модель была обучена на выборках сбаллансированных различными способами;
  - в ходе работы была использована функция подбирающая модели и гиперпараметры моделей;
  - лучшая модель была апробирована на тестовой выборке;
  - подобран threshold по AUC-ROC.

Лучшая модель для решения задачи пронозирования ухода клиента - `CatBoostClassifier` с параметрами:
  `max_depth` = 4  
  `l2_leaf_reg` = 2  
  `learning_rate` = 0.05  
  `iterations` = 200  
  `threshold` = 0.19

Полученная модель будет успешно определять клиента банка прежде, чем он откажется от услуг в 80% случаев.