PS Невозможно прикрепить файл > 25mb
# Восьмой проект: Определение стоимости автомобилей

| Название проекта | Описание | Используемые библиотеки |
|------------------|----------|--------------------------|
| [autos](autos.csv)<br>| Сервис по продаже автомобилей с пробегом «Не бит, не крашен» разрабатывает приложение для привлечения новых клиентов. В нём можно быстро узнать рыночную стоимость своего автомобиля. В вашем распоряжении исторические данные: технические характеристики, комплектации и цены автомобилей. Вам нужно построить модель для определения стоимости.<br>Заказчику важны:<br><br> - качество предсказания;<br><br> - скорость предсказания;<br><br> -время обучения.<br>| <br>import pandas as pd<br><br>import numpy as np<br> <br>import matplotlib.pyplot as plt<br><br>import seaborn as sns<br><br>from math import sqrt<br><br>from sklearn.impute import SimpleImputer<br><br>from sklearn.pipeline import Pipeline<br><br>from sklearn.preprocessing import OneHotEncoder, OrdinalEncoder, StandardScaler, MinMaxScaler, RobustScaler, LabelEncoder<br><br>from sklearn.metrics import roc_auc_score, mean_squared_error<br><br>from sklearn.model_selection import RandomizedSearchCV, GridSearchCV, train_test_split<br><br>from sklearn.compose import ColumnTransformer<br><br>from lightgbm import LGBMRegressor<br><br>from sklearn.linear_model import LinearRegression<br><br>from sklearn.tree import DecisionTreeRegressor<br><br>from sklearn.ensemble import GradientBoostingRegressor<br><br>import phik<br><br>from phik import phik_matrix<br><br>from phik.report import plot_correlation_matrix<br><br>from warnings import simplefilter<br><br>simplefilter(action='ignore', category=FutureWarning)<br><br>import ydata_profiling<br>|
