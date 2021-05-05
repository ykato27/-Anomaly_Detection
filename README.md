# Anomaly-Detection
* 異常検知モデル全般のプログラム

## リポジトリ構成
```
.
├── README.md                 READMEファイル
├── .dockerignore        
├── Dockerfile                Dockerファイル
├── docker-compose.yml
├── notebook                  jupyter notebook
└── data                      dataファイル
```

## 環境構築

* Dockderfileがあるホスト側のフォルダへ移動（例：Desktop/Anomaly-Detection）
```
cd Desktop/Anomaly-Detection
```

* Dockerによる環境構築（フォルダをマウント：Desktop/Anomaly_Detection）
```
docker-compose up --build
```

* ブラウザーを立ち上げてlocalhost:8888へアクセス
* ローカルフォルダがマウントされている

## jupyter notebook説明
* [ANACONDA.ipynb](https://github.com/ykato27/Anomaly-Detection/blob/main/notebook/ANACONDA.ipynb) : 異常状態検知(疎構造学習による異常検知)のnotebook
* [ChangeFinder.ipynb](https://github.com/ykato27/Anomaly-Detection/blob/main/notebook/ChangeFinder.ipynb) : 変化点検知(ChangeFinder)のnotebook
* [GraphLasso.ipynb](https://github.com/ykato27/Anomaly-Detection/blob/main/notebook/GraphLasso.ipynb) : 異常状態検知(疎構造学習による異常検知)のnotebook
* [HMM.ipynb](https://github.com/ykato27/Anomaly-Detection/blob/main/notebook/HMM.ipynb) : 変化点検知(状態空間モデル)のnotebook
* [KNearestNeighbors_AnomalyDetection.ipynb](https://github.com/ykato27/Anomaly-Detection/blob/main/notebook/KNearestNeighbors_AnomalyDetection.ipynb) : 変化点検知(K近傍法)のnotebook
* [LSTM_Keras.ipynb](https://github.com/ykato27/Anomaly-Detection/blob/main/notebook/LSTM_Keras.ipynb) : 変化点検知(LSTM)のnotebook
* [MSPC.ipynb](https://github.com/ykato27/Anomaly-Detection/blob/main/notebook/MSPC.ipynb) : 異常状態検知(多変量統計的プロセス管理)のnotebook
* [Singular_Spectrum_Transformation.ipynb](https://github.com/ykato27/Anomaly-Detection/blob/main/notebook/Singular_Spectrum_Transformation.ipynb) : 変化点検知(特異スペクトル変換法)のnotebook

## 参考文献
* ANACONDA : [https://www.ibm.com/downloads/cas/AVQZBQ2L](https://www.ibm.com/downloads/cas/AVQZBQ2L)
* ChangeFinder : [データマイニングによる異常検知](https://www.amazon.co.jp/%E3%83%87%E3%83%BC%E3%82%BF%E3%83%9E%E3%82%A4%E3%83%8B%E3%83%B3%E3%82%B0%E3%81%AB%E3%82%88%E3%82%8B%E7%95%B0%E5%B8%B8%E6%A4%9C%E7%9F%A5-%E5%B1%B1%E8%A5%BF-%E5%81%A5%E5%8F%B8/dp/4320018826)（書籍）
* GraphLasso : [https://www.ibm.com/downloads/cas/AVQZBQ2L](https://www.ibm.com/downloads/cas/AVQZBQ2L)
* HMM : [異常検知と変化検知](https://www.amazon.co.jp/%E7%95%B0%E5%B8%B8%E6%A4%9C%E7%9F%A5%E3%81%A8%E5%A4%89%E5%8C%96%E6%A4%9C%E7%9F%A5-%E6%A9%9F%E6%A2%B0%E5%AD%A6%E7%BF%92%E3%83%97%E3%83%AD%E3%83%95%E3%82%A7%E3%83%83%E3%82%B7%E3%83%A7%E3%83%8A%E3%83%AB%E3%82%B7%E3%83%AA%E3%83%BC%E3%82%BA-%E4%BA%95%E6%89%8B-%E5%89%9B/dp/4061529080)（書籍）
* KNearestNeighbors_AnomalyDetection : [異常検知と変化検知](https://www.amazon.co.jp/%E7%95%B0%E5%B8%B8%E6%A4%9C%E7%9F%A5%E3%81%A8%E5%A4%89%E5%8C%96%E6%A4%9C%E7%9F%A5-%E6%A9%9F%E6%A2%B0%E5%AD%A6%E7%BF%92%E3%83%97%E3%83%AD%E3%83%95%E3%82%A7%E3%83%83%E3%82%B7%E3%83%A7%E3%83%8A%E3%83%AB%E3%82%B7%E3%83%AA%E3%83%BC%E3%82%BA-%E4%BA%95%E6%89%8B-%E5%89%9B/dp/4061529080)（書籍）
* LSTM_Keras : [異常検知と変化検知](https://www.amazon.co.jp/%E7%95%B0%E5%B8%B8%E6%A4%9C%E7%9F%A5%E3%81%A8%E5%A4%89%E5%8C%96%E6%A4%9C%E7%9F%A5-%E6%A9%9F%E6%A2%B0%E5%AD%A6%E7%BF%92%E3%83%97%E3%83%AD%E3%83%95%E3%82%A7%E3%83%83%E3%82%B7%E3%83%A7%E3%83%8A%E3%83%AB%E3%82%B7%E3%83%AA%E3%83%BC%E3%82%BA-%E4%BA%95%E6%89%8B-%E5%89%9B/dp/4061529080)（書籍）
* MSPC : [http://manabukano.brilliant-future.net/research/report/Report2005_MSPC.pdf](http://manabukano.brilliant-future.net/research/report/Report2005_MSPC.pdf)
* Singular_Spectrum_Transformation : [https://ide-research.net/papers/2004_JSSST_Ide.pdf](https://ide-research.net/papers/2004_JSSST_Ide.pdf)

## 動作環境
マシンスペック（Mac)
- MacBook Air (Retina, 13-inch, 2018)
- 1.6 GHz デュアルコアIntel Core i5
- 8 GB 2133 MHz LPDDR3
