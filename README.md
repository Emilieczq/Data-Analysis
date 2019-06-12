# 数据分析学习笔记

该谷仓中的代码和部分笔记摘自《Python 数据分析实战》（Fabio Nelli 著，杜春晓译，人民邮电出版社）。

## sklearn_examples
该文件夹主要涉及 scikit-learn 库的运用。

**环境准备:**
在 Python 3 中下载 scikit-learn 和 matplotlib 包，numpy 包应该会在下载 scikit-learn 时自动下载，若下载出现问题可以查看我的一篇文章<a href="https://www.cnblogs.com/zhenqichai/p/fix-pip-install-sklearn-problem.html">《Python：安装sklearn包出现错误的解决方法》</a>。

根据数据和所要创建的模型的类型，学习问题可以分为两大类：**有监督学习**和**无监督学习**。

### 有监督学习
训练集好汉作为预测结果的额外的属性信息。这些信息可以这哦模型对新数据作出跟已有数据类似的预测结果。

### 用 scikit-learn 实现有监督学习

#### 利用 scikit-learn 中的 Iris 数据集学习

1. 根据鸢尾花的萼片长宽分类
运行`python3 iris_sepal.py`，得到以下结果。
<p align="center">
 <img src="sklearn_examples/iris_sepal.png" width="500"/>
</p>

2. 根据鸢尾花的花瓣长宽分类
运行`python3 iris_petal.py`，得到以下结果。
<p align="center">
 <img src="sklearn_examples/iris_petal.png" width="500"/>
</p>

3. 主成分分析法（Principal Component Analysis, PCA）。该方法可以减少系统的维度，保留足以描述各数据点特征的信息，其中新生成的各维叫作主成分。
运行`python3 iris_PCA.py`，得到以下结果。
<p align="center">
 <img src="sklearn_examples/iris_PCA.png" width="500"/>
</p>

## javascript_ipython_examples
该文件夹主要涉及如何通过在 IPython Notebook 中嵌入 JavaScript 库 D3 来扩展其表示图像的能力。该库有多种图像制作的功能，甚至可以实现连 matplotlib 库都无法实现的图像效果。

**环境准备:**
在 Python 3 中下载 jupyter notebook、numpy、pandas、matplotlib、urllib3。其余的库在 IPython Notbook 中会有提示下载。
**注意：**
urllib3是我选择下载的库，在书中（第253页）提示要求下载 urllib2，该库已经过时，无法下载，下载之后的import语句也发生改变，详细情况请看代码。

### 条形图
运行 IPython Notbook 第一部分的代码，可以得到 2018 年美国人口最多的前五个洲的人口统计条形图。
<p align="center">
 <img src="javascript_ipython_examples/output_1.png" width="500"/>
</p>

### 簇状条形图
运行 IPython Notbook 第一部分的代码，前面五个国家的 2015-2018 四年的人口统计簇状条形图。
<p align="center">
 <img src="javascript_ipython_examples/output_2.png" width="500"/>
</p>

### 地区分布图
运行 IPython Notbook 第一部分的代码，可以得到美国人口地区分布图。
<p align="center">
 <img src="javascript_ipython_examples/output_3.png" width="500"/>
</p>