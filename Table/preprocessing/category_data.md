# カテゴリデータ(エンコード)
1. LabelEncoding
2. One-Hot Encoding
3. dummy Encoding
4. target Encoding

## マップ
```python
map_dict = {'before1': after1, 'before2': after2}

pd.replace(map_dict)
#もしくは
pd.map(map_dict)
```

## Label Encoding
```python
from sklearn.preprocessing import LabelEncoder

le = LabelEncoder()
le.fit(train[i])
train[i] = le.transform(train[i])
```

## One-Hot Encoding
```python
# pandasを使用する
## dummy_na=True で欠測値あり指定
train = pd.concat([train, pd.get_dummies(train[i])], axis=1, join='inner')
```

## Dummy Encoding
```python
## pandasを使用する
## dummy_na=True で欠測値あり指定

train = pd.concat([train, pd.get_dummies(train[i], drop_first=True)], axis=1, join='inner')
```

```python

```
