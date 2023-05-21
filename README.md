# Bert for sentence embedding

# 基础介绍 Intro
该借鉴了https://github.com/649453932/Bert-Chinese-Text-Classification-Pytorch 构建的BERT基础框架。

# 使用方法：
## 1.数据与模型导入：
### 数据 data preparation
必须和我THUCNews/data中的数据格式一致。分别替换成为你的数据即可。
Must be in the same form of my data.

### 模型 model preparation

链接：https://pan.baidu.com/s/1jHF-zDibrDQZz5BZDRWpSA?pwd=5a8m 提取码：5a8m
下载后全部放到Pre_trained那个文件夹下。

## 2.运行操作：
### 训练并测试：

python run.py --model bert


## 3.后续分析文件说明：


3.1 check.ipynb


读取embedding结果，并且进行cosine similarity计算等任务


3.2 embedding_from_package.ipynb


通过package导入embedding结果，可以作为本项目的备选。该项目更加完善
