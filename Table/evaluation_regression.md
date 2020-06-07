# 回帰の評価"

## 平均絶対誤差
$$
MAE=\frac{1}{n} \sum_{i=0}^{n-1}\left|y_{i}-\hat{y}_{i}\right|
$$

```python
from sklean.metrics import mean_absolute_error
mean_absolute_error(y_val, y_pred)
```

## 平均二乗誤差(MSE)

$$
MSE = \frac{1}{n} \sum_{i=0}^{n-1}\left(y_{i}-\hat{y}_{i}\right)^{2}
$$
```python
from sklearn.metrics import mean_squared_error

mean_squared_error(y_val, y_pred)
```

## 二乗平均平方根誤差(RMSE)
$$
RMSE = \sqrt{\frac{1}{n} \sum_{i=0}^{n-1}\left(y_{i}-\hat{y}_{i}\right)^{2}}
$$
```python
from sklearn.metrics import mean_squared_error
np.sqrt(eman_squared_error(y_val, y_pred)
```

## 決定係数 $R^2$
$$
1-\frac{\sum_{i=0}^{n-1}\left(y_{i}-\hat{y}_{i}\right)^{2}}{\sum_{i=0}^{n-1}\left(y_{i}-\overline{y}\right)^{2}}
$$

```python
from sklearn.metrics import r2_score
r2_score(y_val, y_pred)
```
