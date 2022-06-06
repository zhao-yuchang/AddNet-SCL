# AddNet-SCL
Code for paper: Patient-Specific Seizure Prediction via Adder Network and Supervised Contrastive Learning

## About the paper
* Title: [Patient-Specific Seizure Prediction via Adder Network and Supervised Contrastive Learning](https://ieeexplore.ieee.org/document/9787538)
* Authors: Yuchang Zhao, Chang Li, Xiang Liu, Ruobing Qian, Rencheng Song, Xun Chen
* Institution: Hefei University of Technology
* Published in: IEEE Transactions on neural systems and rehabilitation engineering
## Instructions
* Before running the code, please download the CHBMIT dataset, unzip it and place it into the right directory. Generate 4s samples using data_process.py.  Each .hickle data file contains the EEG signals and consponding labels of a subject. There are 2 arrays in the file: **data** 
and **labels**. The shape of **data** is (32, 1, 1024, 22). The shape of **label** is (32,1). 
* Using AddNet-SCL.py to train and test the model (leave one out cross-validation), result will be saved in a /results file.
* The CHBMIT dataset can be found [here](https://physionet.org/content/chbmit/1.0.0/).
* The usage on Kaggle dataset is the same as above. The Kaggle dataset can be found [here]( https://www.kaggle.com/c/seizure-prediction/data).

## Requirements
+ Pyhton3.7
+ pytorch (1.10.1 version)
* If you have any questions, please contact yuchangzhao@mail.hfut.edu.cn

## Reference
* [huawei-noah/AdderNet](https://github.com/huawei-noah/AdderNet)
* [HobbitLong/SupContrast](https://github.com/HobbitLong/SupContrast)
