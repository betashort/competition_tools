# pandasのメモ

## pandasの表示する列と行の最大値の設定
```python
pd.options.display.max_columns = None
pd.options.display.max_rows = None
```

## 集約(値による行のグループ分け)
```python
#列によるグループ分けの平均
pd.groupby('列').mean()

#２つの列の値による行のグループ分けの、列nのデータ
pd.groupby(['列1', '列2'])['列n']
```

## 列のすべての要素に対して関数を適用する
```python
def function(x):
    return(x)

#関数の適用
pd.apply(x)

#ラムダ式
pd.apply(lambda x : x + 1)
```

## DataFrameの連結
```python
#列方向に連結
pd.concat([df1, df2], axis=1)

#行方向に連結
pd.concat([df1, df2], axis=0)
```

## idと一致するようなDataFrameの連結(マージ)
```python
pd.merge(df1, df2, on='id')
```

## ソート
昇順は、ascending=True  
降順は、ascending=False  
```python
pd.sort_values('指定の列', ascending=True)
```

## ユニークな値
```python
pd['列'].unique()
```

## ユニークな値とその値が現れた回数
```python
pd['列'].value_counts()
```

## ユニークな値の数
```python
pd.nunique()
```

## 欠測の確認
```python
pd.isnull().sum()

pd.isnull().sum().sort_values(ascending=False)
```

# Seriese 列名の変更
```python
Series.rename('列名')

Seriese.name = '列名'
```


```python

```

```python

```

```python

```
