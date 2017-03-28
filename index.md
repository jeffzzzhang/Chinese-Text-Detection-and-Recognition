**中文字符识别**
==

组员： 蔡玮 陈利 程伟 王新旺

 ---
 
# **Introduction**

Historically, Chinese character recognition has been extensively studied . In the mobile internet era, the research on the robust recognition of handwritten Chinese characters in an unconstraint manner has become increasingly popular due to the application demand. In terms of the task complexity, the offline handwritten Chinese text recognition is the most challenging task due to the lack of trajectory information and the free writing style, which is also the topic of this study.

---

## **reference paper:**
1、[A CNN Based Scene Chinese Text Recognition Algorithm With Synthetic Data Engine](https://arxiv.org/pdf/1604.01891.pdf)
2、[Neural Network Classifiers for Optical Chinese Character Recognition](http://www.cs.cmu.edu/afs/cs.cmu.edu/project/pcvision/www/papers/chinese/final.html)

---

## **Week 3**

1、制作网页

2、查找参考文献

## **Week 4**
------

检索有关字符识别的方法资料，并尝试理清其实现方案。学习其中方法并找出可借鉴性。
其中有一篇名为《手写数字字符识别》的文章，和所选课题有比较相似的地方，于是借此学习理解，并尝试将代码调试通过，观察识别结果。
具体的实现思路以及结果如下：

> * 项目名称：手写字符识别
> * 主流程如下图所示

 ![image1](https://raw.githubusercontent.com/pukitoto/Chinese-Text-Detection-and-Recognition/master/1.png)
 
 > * 详细流程如下图所示
 
 ![image2](https://raw.githubusercontent.com/pukitoto/Chinese-Text-Detection-and-Recognition/master/2.png)
 
 > * 实现结果如下图所示
 
 ![image3](https://raw.githubusercontent.com/pukitoto/Chinese-Text-Detection-and-Recognition/master/3.jpg)
 
 ![image4](https://raw.githubusercontent.com/pukitoto/Chinese-Text-Detection-and-Recognition/master/4.jpg)
 
 > * 本文的识别方法采用knn近邻分类法。这个算法首先贮藏所有的训练样本，然后通过分析（包括选举，计算加权和等方式）一个新样本周围K个最近邻以给出该样本的相应值。这种方法有时候被称作“基于样本的学习”，即为了预测，我们对于给定的输入搜索最近的已知其相应的特征向量。
  
> * 借鉴性
“基于样本的学习“方法是本文的核心思想，并检索有关的项目、文献资料，确实有很多此方面用于中文识别的论文研究。首先提取中文汉字的特征信息，再归纳整理成字符识别器，再将待识别字符与字符识别器中的样本进行对比。特征点的提取步骤就成了重难点之一，后面加深对这一块的理论学习与研究，并敲定实现方法。
