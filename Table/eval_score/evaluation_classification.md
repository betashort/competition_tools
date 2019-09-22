# 分類の評価

1. TP:
2. TN:
3. FP:
4. FN:


## Accuracy 精度
```python
from sklearn.metrics import accuracy
accuracy(y_val, y_pred)
```

## Precision 適合率
```python

```
## Recall 再現率
```python

```

## 混合行列(Confusion Matrix)

```python
from sklearn.metrics import confusion_matrix

matrix = confusion_matrix(test, pred)
mat_df = pd.DataFrame(matrix, index=class_name, columns=class_name)

sns.heatmap(mat_df)
plt.show()
```

## ROC

## AUC

# 参照
https://scikit-learn.org/stable/modules/classes.html#module-sklearn.metrics
