# 快速开始
* 下载数据集解压到`input/movielens-20m-dataset`文件夹下，此文件夹下有六个CSV文件
* 先在Jupyter NoteBook 下运行`Codes`下的DataProcess.ipynb文件
* 再随意运行另外两个文件
# 描述
## 数据集描述
采用的是 20M 的Movie Lens数据集，共有6个CSV文件，2000多万条影评数据。 
下载地址是：https://www.kaggle.com/grouplens/movielens-20m-dataset/download
数据集介绍地址：http://grouplens.org/datasets/movielens/
## 工具描述
主要使用了以下工具和包：
* jupyter NoteBook: 开发平台
* Pandas
* Numpy
* sklearn：Kmeans库
* matplot：绘图
* wordcloud：绘制词云
* jieba：统计词数         
## 文件描述
* **Codes：** 这个文件夹下包含的是3个noteBook文件
* **input：** 包括的是20M的电影相关的数据集
* **output：** 包括项目运行中输出的图片和处理后的数据集
## 硬件平台
* 要运行此代码，建议机器运行内存16GB以上（如果不够，请在`Codes/DataProcess.ipynb`降低采样率）
# 代码
代码部分三块
* DataProcess.ipynb：主要用来做数据的读取，预处理（join数据到一起并输出到`output/`中）、OneHot编码、采样数据集等
* visualizationDataset.ipynb：主要挖掘数据之间的内在联系，通过图表的方式，并且通过 Kmeans 聚类进行了数据探索
* recommendation.ipynb：建立两个推荐模型，一个是基于用户的协同过滤的模型，一个是基于风格的协同过滤的模型，并在这两个模型的基础上绘制了P-R曲线
其中`Codes/data`文件夹下存储的是训练集、测试集和总数据集的字典。他们的key（UserID）都是相同的，value（MovieId）则不同。
# 项目后续
* 这个项目本人还会持续维护
* 后续可能会做一些基于tag的协同过滤
* 引入神经网络
* ...