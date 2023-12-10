# C-MPASS FD001 RUL Prediction

A simple reproduction of this paper with PyTorch:

## Requirements

[![Python badge](https://img.shields.io/badge/Python-3.10-blue.svg)](https://www.python.org/)
[![PyTorch badge](https://img.shields.io/badge/PyTorch-1.12.1-green.svg)](https://pytorch.org/)
[![NumPy badge](https://img.shields.io/badge/Numpy-1.21.6-yellow.svg)](https://numpy.org/)  

## Usage

1. Run *data process.ipynb*
2. Run *main.ipynb*

## Network Architecture

![Structure_00](C:\Users\20329\Desktop\NWPU\zd论文\5.2023基于特征融合的航空发动机寿命预测 推进技术\图\Structure_00.png)

## Eval Metrics

- RMSE
- Score

## Result

1. Prediction:

![1702188177992](C:\Users\20329\AppData\Roaming\Typora\typora-user-images\1702188177992.png)

2. Comparison:

| Model                 | *RMSE* | *Score* |
| --------------------- | ------ | ------- |
| DLSTM[18]             | 18.33  | 655     |
| LSTM[19]              | 16.14  | 338     |
| DBN[20]               | 15.04  | 334     |
| LSTMBS[21]            | 14.89  | 481     |
| ES-XGBoost[22]        | 13.74  | 286     |
| Autoencoder-BLSTM[23] | 13.63  | 261     |
| DCNN[24]              | 12.61  | 274     |
| SAE-DeepAR[10]        | 12.52  | 205     |
| AGCNN[25]             | 12.42  | 226     |
| F2Net (Ours)          | 11.11  | 173     |

## Acknowledgments

Our code is based on [this](https://github.com/zhmou/Turbofan-engine-RUL-prediction). We sincerely appreciate their contributions and authors for releasing source codes. 

