# Bert-Novelty

# 基础介绍
该项目以https://github.com/649453932/Bert-Chinese-Text-Classification-Pytorch 为基础框架进行了拓展。主要拓展内容（1）封装了原作者未完成的预测功能，（2）将Bert中的Embedding层输出，方便进一步使用sentence vector来进行similarity等操作。

# 使用方法：
## 1.数据使用：
必须和我THUCNews中的数据格式一致。分别替换成为你的数据即可。
## 2.运行操作：
### 训练并测试：
（1）基础的bert


python run.py --model bert | tee embedding.txt


（2）bert + 其它（eg bert_CNN）


python run.py --model bert_CNN | tee embedding.txt


（3）ERNIE


python run.py --model ERNIE | tee embedding.txt

## 3.文件说明：
运行完成后embedding.txt即为文本的embedding层，THUCNews文件夹下的prediction_result.txt即为预测结果。
