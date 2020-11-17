# MovieLens1M 基于深度学习的电影推荐系统
使用MovieLens1M数据集（data can be downloaded from https://grouplens.org/datasets/movielens/)
，实现了Auto Encoder (AE), Variational Auto Encoder (VAE), BERT提取电影名特征3种方法，对评分矩阵进行填补，继而对用户做出推荐。

代码建议在Google Colab环境下运行，代码中的目录请根据自己的实际目录进行修改。  

本代码主目录和子目录如下：  

/content/drive/Movie_lens/  
--------- ml-1m (包含数据集的文件夹)  
--------- auto encoder.ipynb  
--------- BERT-based-recommender.ipynb  

## **1 Models:**

### 1.1 Auto Encoder
<img src="https://github.com/YJiangcm/Movielens1M-Movie-Recommendation-System/blob/main/pictures/auto%20encoder.png" width="400" height="300">

### 1.2 Variational Auto Encoder
<img src="https://github.com/YJiangcm/Movielens1M-Movie-Recommendation-System/blob/main/pictures/variational%20auto%20encoder.png" width="400" height="300">

### 1.3 BERT-based
<img src="https://github.com/YJiangcm/Movielens1M-Movie-Recommendation-System/blob/main/pictures/bert-based.PNG" width="600" height="300">

## **2 Experiment Results:**

### 2.1 MSE of training loss and validation loss of Auto Encoder
<img src="https://github.com/YJiangcm/Movielens1M-Movie-Recommendation-System/blob/main/pictures/auto%20encoder%20result.png" width="460" height="280">

### 2.2 MSE of training loss and validation loss of Variational Auto Encoder
<img src="https://github.com/YJiangcm/Movielens1M-Movie-Recommendation-System/blob/main/pictures/variational%20auto%20encoder%20result.png" width="450" height="280">

### 2.3 MSE of training loss and test loss of BERT-based
<img src="https://github.com/YJiangcm/Movielens1M-Movie-Recommendation-System/blob/main/pictures/bert-based%20result.png" width="800" height="300">

### 2.4 test MSE loss of different models
 Model | test MSE loss  
 ---- | -----  
 Auto Encoder  | 1.0837
 Variational Auto Encoder  | 0.9956
 BERT-based  | **0.7507**
