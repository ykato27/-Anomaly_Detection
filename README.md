# Anomaly_Detection
* 異常検知モデル全般のプログラム

## リポジトリ構成
```
.
├── README.md                 READMEファイル
├── Dockerfile                Dockerファイル
└── data                      dataファイル
```

## 環境構築
### Dockderfileがあるホスト側のフォルダへ移動（例：Desktop/Anomaly_Detection）
```
cd Desktop/Anomaly_Detection
```
### Dockerによる環境構築
```
docker build .
```
docker run実行（対象フォルダをマウントする／例：Desktop/Anomaly_Detection）
```
docker run -p 8888:8888 -v ~/Desktop/Anomaly_Detection/:/work --name Anomaly_Detection <docker image>
```
ブラウザーを立ち上げてlocalhost:8888へアクセス
workフォルダ内が対象フォルダにマウントされている

## jupyter notebook説明
* ChangeFinder.ipynb                       : 変化検知(ChangeFinder)のnotebook
* KNearestNeighbors_AnomalyDetection.ipynb : 変化点検知(K近傍法)の異常検知notebook
* ANACONDA.ipynb                           : 異常状態検知(疎構造学習による異常検知)のnotebook
* GraphLasso.ipynb                         : 異常状態検知(疎構造学習による異常検知)のnotebook
* MSPC.ipynb                               : 異常状態検知(多変量統計的プロセス管理)のnotebook

## 動作環境
マシンスペック（Mac)
- MacBook Air (Retina, 13-inch, 2018)
- 1.6 GHz デュアルコアIntel Core i5
- 8 GB 2133 MHz LPDDR3