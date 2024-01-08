模型都未进行调参，未能使模型的准确率达到最高
# 项目名称：
使用 bert 模型来对中文进行分类，即文本分类

# 项目环境：
pytorch、python   
相关库安装
```
pip install -r requirement.txt
```
# 模型训练
`python main.py`

# 模型预测
`python predict.py`

# 训练自己的数据集
train.txt、dev.txt、test.txt 的数据格式：文本\t标签（数字表示）
class.txt：标签类别（文本）
## 修改内容：
在配置文件中修改长度、类别数、预训练模型地址    
parser.add_argument("--bert_pred", type=str, default="./bert-base-chinese")   
parser.add_argument("--class_num", type=int, default=10)   
parser.add_argument("--max_len", type=int, default=38)

  
