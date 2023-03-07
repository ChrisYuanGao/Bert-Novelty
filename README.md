# Bert-Novelty

# 基础介绍
该项目以https://github.com/649453932/Bert-Chinese-Text-Classification-Pytorch 为基础框架进行了拓展。主要拓展内容（1）封装了原作者未完成的预测功能，（2）将Bert中的Embedding层输出，方便进一步使用sentence vector来进行similarity等操作。

# 使用方法：
## 1.数据与模型导入：
### 数据

必须和我THUCNews/data中的数据格式一致。分别替换成为你的数据即可。
### 模型

链接：https://pan.baidu.com/s/1jHF-zDibrDQZz5BZDRWpSA?pwd=5a8m 
提取码：5a8m 

导入的路径和操作看我上面引用的链接即可。也就是放到Pre_trained那个文件夹下
## 2.运行操作：
### 训练并测试：
（1）基础的bert


python run.py --model bert | tee embedding.txt


（2）bert + 其它（eg bert_CNN）


python run.py --model bert_CNN | tee embedding.txt


（3）ERNIE


python run.py --model ERNIE | tee embedding.txt

## 3.文件说明：
运行完成后embedding.txt即为文本的embedding层，THUCNews文件夹下的prediction_result.txt即为预测结果。(如果长度与对应的文本不匹配，可能是读取数据时出问题，删除该文件中的第一行即可）
