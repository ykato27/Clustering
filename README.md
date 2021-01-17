# Clustering
* クラスタリング全般のプログラム

## リポジトリ構成
```
.
├── README.md                 READMEファイル
├── Dockerfile                Dockerファイル
└── notebook                  jupyter notebook
```

## 環境構築
Dockderfileがあるホスト側のフォルダへ移動（例：Desktop/Clustering）
```
cd Desktop/Clustering
```
Dockerによる環境構築
```
docker build .
```
docker run実行（対象フォルダをマウントする／例：Desktop/Clustering）
```
docker run -p 8888:8888 -v ~/Desktop/Clustering/:/work --name Clustering <docker image>
```
ブラウザーを立ち上げてlocalhost:8888へアクセス
workフォルダ内が対象フォルダにマウントされている

## jupyter notebook説明
* Clustering_K_means.ipynb : クラスタリング(K-means法)のnotebook
* Hierarchical_Clustering.ipynb : クラスタリング（階層的クラスタリング）のnotebook

## 動作環境
マシンスペック（Mac)
- MacBook Air (Retina, 13-inch, 2018)
- 1.6 GHz デュアルコアIntel Core i5
- 8 GB 2133 MHz LPDDR3