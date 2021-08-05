# AI-Studio-飞桨常规赛：遥感影像地块分割 - 7月第5名方案 

## 项目描述
利用PaddleSeg套件完成遥感影像地块分割Baseline

（1）模型构建思路及调优过程：
 a. 尝试了Unet、Attention Unet、SETR模型，最后发现Attention Unet精度可以达到最好精度0.51，SETR训练多个epoch后只有0.4+，Unet最低
 b. batch_size依次尝试2、4、8、16... 根据显存能力尽量选取最高的batch_size
 c. 训练集数据采用随机翻转进行增强

（2）参考代码：
[10分钟上手PaddleSeg](https://aistudio.baidu.com/aistudio/projectdetail/1672610?channelType=0&channel=0)

（3）代码内容说明见notebook

注：由于当初想把这个比赛方案作为公开项目baseline，所以提交结果后就没有保留模型参数，项目中暂存结果文件均为示例数据和模型
## 项目结构
```
-|data
-|work
-README.MD
-xxx.ipynb
```
## 使用方式
在AI Studio上[运行本项目](https://aistudio.baidu.com/aistudio/projectdetail/2224724)

