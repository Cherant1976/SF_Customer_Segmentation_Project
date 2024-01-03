# <center> Учебный проект программы Data Science платформы [Skillfactory](http://skillfactory.ru) (Сегментация клиентов онлайн магазина подарков). </center>

## Оглавление  
[1. Описание учебного проекта](https://github.com/Cherant1976/SF_Customer_Segmentation_Project#Описание-учебного-проекта)   
[2. Краткая информация о данных](https://github.com/Cherant1976/SF_Customer_Segmentation_Project#Краткая-информация-о-данных)  
[3. Этапы выполнения заданий учебного проекта](https://github.com/Cherant1976/SF_Customer_Segmentation_Project#Этапы-выполнения-заданий-учебного-проекта)  
[4. Используемые библиотеки python](https://github.com/Cherant1976/SF_Customer_Segmentation_Project#Используемые-библиотеки-python)  
[5. Выводы и заключения](https://github.com/Cherant1976/SF_Customer_Segmentation_Project#Выводы-и-заключения)  
[6. Примечание к графикам plotly](https://github.com/Cherant1976/SF_Customer_Segmentation_Project#Примечание-к-графикам-plotly) 

### Описание учебного проекта    
Учебный проект: Сегментация клиентов онлайн магазина подарков на основании реальных транзакций за 2010 и 2011 годы [The UCI Machine Learning Repository](http://archive.ics.uci.edu/ml/index.php).

:arrow_up:[к оглавлению](https://github.com/Cherant1976/SF_Customer_Segmentation_Project#Оглавление)


### Краткая информация о данных:
Основной файл формата *csv* из-за значительного размера (около 450 МБ) не загружен на *github*, но он есть в открытом доступе на [**google disk**](https://drive.google.com/file/d/1aXc3Q5EgGfGGNq0DLYewLZSJbIvlLiN0/view?usp=sharing). В основном файле содержатся данные о транзакциях.

  
:arrow_up:[к оглавлению](https://github.com/Cherant1976/SF_Customer_Segmentation_Project#Оглавление)

### Этапы выполнения заданий учебного проекта:  
- Изучение структуры данных
- Преобразование, очистка и анализ данных
- Построение [**RFM**](https://www.investopedia.com/terms/r/rfm-recency-frequency-monetary-value.asp) таблицы
- Моделирование и оценка качества моделей
- Анализ полученной кластеризации/сегментации клиентов
  Примечание:
  Значительное время занял анализ предоставленного к проекту алгоритма по учету возвратов заказов.
  В работе показаны ошибки в работе предоставленного алгоритма и создан верный алгоритм.

:arrow_up:[к оглавлению](https://github.com/Cherant1976/SF_Customer_Segmentation_Project#Оглавление)


### Используемые библиотеки *python*:  
**pandas** *pd*, **numpy** *np*, **matplotlib.pyplot** *plt*, **seaborn** *sns*, **plotly.express** *px*, **sklearn**, **stats**, **statsmodels**, **re**
```python
import pandas as pd
import numpy as np
import matplotlib.pyplot as plt
import seaborn as sns

import plotly.graph_objs as go
import plotly.express as px
from plotly.subplots import make_subplots
import statsmodels.api as sm

import scipy.stats as stats

from sklearn import preprocessing
from sklearn.preprocessing import StandardScaler
from sklearn.pipeline import Pipeline
from sklearn.decomposition import PCA

from sklearn.cluster import KMeans
from sklearn.mixture import GaussianMixture
from sklearn.cluster import AgglomerativeClustering

from sklearn.metrics import silhouette_score

import re
```

:arrow_up:[к оглавлению](https://github.com/Cherant1976/SF_Customer_Segmentation_Project#Оглавление)

---
### Примечание к графикам **plotly**:  
Графики код для которых написан с использованием библиотеки **plotly** могут отображаться некорректно. Просмотр указанных графиков доступен в браузере, *html* файлы для этого находятся в папке [**plotly**](https://github.com/Cherant1976/SF_Customer_Segmentation_Project/tree/master/plotly)
Ссылки также доступны под соответсвующим кодом в файле [**PROJECT_6__Сегментация_клиентов_онлайн_магазина_Черников.ipynb**](https://github.com/Cherant1976/SF_Customer_Segmentation_Project/blob/master/PROJECT_6__Сегментация_клиентов_онлайн_магазина_Черников.ipynb)

Если у вас не получится просмотреть файлы в папке, для просмотра в  браузере используйте ссылки ниже:
- [**ГРАФИКИ пункт 2.3**](https://htmlpreview.github.io/?https://github.com/Cherant1976/SF_Customer_Segmentation_Project/blob/master/plotly/boxplot_rfm.html)
- [**ГРАФИКИ пункт 3.2.1**](https://htmlpreview.github.io/?https://github.com/Cherant1976/SF_Customer_Segmentation_Project/blob/master/plotly/scatter_3d_rfm.html)
- [**ГРАФИКИ пункт 3.2.2**](https://htmlpreview.github.io/?https://github.com/Cherant1976/SF_Customer_Segmentation_Project/blob/master/plotly/cluster_profile_rfm.html)

:arrow_up:[к оглавлению](https://github.com/Cherant1976/SF_Customer_Segmentation_Project#Оглавление)

