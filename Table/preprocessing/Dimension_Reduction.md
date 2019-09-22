# 次元削減
1. PCA
2. Kernel PCA
可視化
3. MDS
4. t-SNE

## PCA
```python
from sklearn.decomposition import PCA

pca = PCA(n_components=2)
pca.fit(X)
X_pca = pca.fit_transform(X)

explained_variance_ratio_
```

## Kernel PCA
kernel : “linear” | “poly” | “rbf” | “sigmoid” | “cosine” | “precomputed”  

```python
from sklearn.decomposition import KernelPCA

kpca = KernelPCA(n_components=2, kernel='linear')
kpca.fit(X)
X_kpca = kpca.fit_transform(X)

```

## MDS
```python
from sklearn.manifold import MDS

mds = MDS(n_components=2)
X_mds = mds.fit_transform(X)
```

## t-SNE
```python
from sklearn.manifold import TSNE

tsne = TSNE(n_components=2)
X_tsne = tsne.fit_transform(X)
```
