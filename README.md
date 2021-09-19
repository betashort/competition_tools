# data_tools_repository

Kaggleなどで使ったコードを貯めていきます。  

# anaconda
pipで管理する。(condaの方がいい？)  

## 仮想環境を作る

### default
* medical-image
* NLP

```
conda env export > medical-image.yml
```

### defaultから作業用の仮想環境を再構築
```
conda env create -n {new_env} -f medical-image.yml
```
もしくは、
```
conda create -n {new_env} --clone medical-image
```

### 仮想環境を起動する。
```
conda activate {new_env}

#for mac
source activate {new_env}
```

### 仮想環境を閉じる
```
conda deactivate
```

# 1. Table competition

## preprocessing
* [pandas](./Table/preprocessing/pandas_memo.md)
* [numeric_data](./Table/preprocessing/numeric_data.md)
* [category_data](./Table/preprocessing/category_data.md)
* [text_data](./Table/preprocessing/text_data.md)
* [time_data](./Table/preprocessing/time_data.md)
* [Dimension_Reduction](./Table/preprocessing/Dimension_Reduction.md)
* [missing and Outlier]()
* [unbalanced]()

## model

## Evaluation
* [Regression](./Table/eval_score/evaluation_regression.md)
* [Classification](Table/eval_score/evaluation_classification.md)
* []
