# Anomaly_Detection
* 異常検知モデル全般のプログラム

## リポジトリ構成
```
.
├── README.md                 READMEファイル
└── Dockerfile                Dockerファイル
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
* Regression_Models.ipynb : 回帰モデル全般のnotebook
* SHAP.ipynb : SHAPのnotebook(機械学習モデルを解釈するためのライブラリー)
* NGBoost.ipynb : XGBoostのnotebook(不確かさを扱える新しい勾配ブースティング)

## 動作環境
マシンスペック（Mac)
- MacBook Air (Retina, 13-inch, 2018)
- 1.6 GHz デュアルコアIntel Core i5
- 8 GB 2133 MHz LPDDR3