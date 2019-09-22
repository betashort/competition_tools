# 数値データ
1. 2値化  
2. 離散化
3. Standard(正規化)
4. MinMax(標準化)
5. $l^2$正規化
6. 対数変換
7. べき変換
8. Box-Cox変換


## 離散化
```python
from sklearn.preprocessing import Binarizer

#閾値を決める
binarizer = Binarizer(threshold)

#複数の閾値を決める
binarizer = Binarizer([th1, th2, th3])
```
## StandardScaler
```python
from sklearn.preprocessing import StandardScaler

sd = StandardScaler()
sd.fit(X)

X_sd = sd.transform(X)

X_sd = sd.fit_transform(X)
```

## MinMaxScaler
```python
from sklearn.preprocessing import MinMaxScaler

mm = MinMaxScaler()
mm.fit(X)

X_mm = mm.transform(X)

X_mm = mm.fit_transform(X)
```

## $l^2$正規化
```python
from sklearn.preprocessing import Normalizer
## l1の場合は、"l1"

normalizer = normalizer(norm="l2")
normalizer.transform(train)
```

## 対数変換
```python
np.log(X)
```

## Box-Cox変換
```python
from scipy import stats
## Attention : 0以下は、エラーになるので注意
train[i], _ = stats.boxcox(train[i] + alpha)
```

## 自作に変換器
```python
from sklearn.preprocessing import FunctionTransformer

def func_trans(x):
    return x

trans = FunctionTransformer(func_trans)

trans.transform(train)
```

## Kmeansで擬似クラス分け
'''python
from sklearn.cluster import KMeans

cluster = KMeans(n, random_state=0)
cluster.fit(X)
pred = cluster.predict(X)
'''
