---
title: Python菜鸟到大神之旅
date: 2018-01-18 10:32:02
tags: 
	- translation
  - getting started
  - python
---

Python菜鸟到大神之旅

也许你想要成为一个数据科学家或者已经作为数据科学家并想拓展一下知识库。那么你来对了，本篇文章旨在为想成为数据科学家的Python新手提供一个详尽的学习路径，并且提供了每一步的概要说明。如果你已经有些背景知识，或者不需要大而全的步骤，可以自行调整学习路径，记得分享给我你的学习路径哦。

你还可以看看这个迷你版的学习路径 -> [Quick Guide to learn Data Science in Python][1]

### 第0步：热热身

在开始本次路途开始之前，有个问题先问一下：

#### 0.1：为什么使用Python？

请观看来自乌克兰的DataRobot创始人Jeremy的这个于PyCon 2014的演讲的前30分钟，了解一下Python有多么实用。

### 第1步：环境搭建

现在你已经下定决心开始，是时候把环境搭建起来了。最简单的方法就是下载[Anaconda][2]，它把大部分你将来要使用到的程序包都准备好了。因为预装的程序包不一定都是最新的，所以这个方法最大的不足就是你需要等待所有包都更新完毕，有些底层的库可能也需要更新，但是这对于新手来说是可以忽略不计的。

当然，你在搭建环境的过程中可能会遇到问题，比如下载比较慢，你可以使用国内的镜像地址，比如[清华大学的开源镜像站][3]。

### 第2步：Python的基础知识学习

你需要从理解语言的基础开始，再就是程序库和数据结构等。这里推荐一个开启新手之旅的好地方——[DataCamp][4]上的交互式Python教程。通过四个小时的编码课程，让你明白如何使用Python助你开始进入数据科学领域，最终你将对这门语言的基础概念有一定的掌握。

**重要知识点**：List（列表），Tuples(元组)，Dictionaries（字典），List comprehensions（列表解析）， Dictionary comprehensions（字典解析）

**小任务**：拿下[DataCamp][5]里的题目

**备用课程**：如果你觉得DataCamp的课程不适合你，可以看看谷歌的 [Google Class for Python][6]，大概两天的系列课程，其中涵盖了后面我们将要介绍的知识点。

### 第3步：在Python中学习正则表达式

你将来会需要用到正则表达式做数据清洗，尤其是你在处理纯文本数据时。学习正则表达式的最好方法是学[Google的课程][7]，还有随手常备的[正则备忘单][8]。

### 第4部：学习Python中的数理库——NumPy，SciPy，Matplptlib和Pandas

好玩的才刚刚开始哦！下面会对这些库分别做简短的介绍，然后让我们开始练习一些常见的操作。

- 通过练习[NumPy教程][9]，特别是NumPy数组，这将为后面的学习打个好基础。
- 接下来，学习一下[SciPy 教程][10]。主要学习一下基础知识，其次再看看你感兴趣的点。
- 按套路接下来应该学Matplptlib教程了吧，事实并非如此哦。因为Matplptlib对目前的我们来说太宽泛了，可以先看[这份文档][11]，只要看到animations动画章节之前就可以了。
- 最后，让我们一起看看Pandas，Pandas提供了DataFrame（数据表）功能。这里需要确实的下一些功夫来练习。Pandas将会成为你做中型数据分析的得力工具。从看一个十分钟的[简介][12]开始吧，接下来就可以移步到[Pandas 教程][13]
- 最后也可以学一下DataCamp上关于[Pandas基础][14]的课程

需要更深入的学习的还可以看看[使用Pandas探索数据分析][15]和[使用Pandas改写数据][16]

**小任务**：解决[哈佛大学课程CS109中的习题][17]

### 第5步：给力的数据可视化

通过学习[课程CS109][18]（这个视频课程链接已经失效了，这里贴上课程链接），你可以跳过前两分钟，接下来的就牛逼了！通过这节课学习来完成这个[小任务][19]

在DataCamp上查看[通过Bokeh数据可视化教程][20]

### 第6步：学习Scikit-learn和机器学习

现在，我们来到了整个学习路径的关键步骤，[Scikit-learn][21]是一个非常实用的机器学习Python库。通过[哈佛大学的课程CS109][22]的第十节到第十八节课的学习，你将了解机器学习的基本概念。监督学习算法：例如回归、决策树和集成建模，非监督学习算法：比如聚类。跟随这些课程并练习每个课后习题。

**附加资源**：

- 你必须要读的一本书——[集体智慧编程][23]经典，如今看来仍是首选
- 另外，你还可以学习最好的机器学习课之一[“Machine Learning course from Yaser Abu-Mostafa.”][24]。如果你需要更多的详细清晰的技术讲解，你可以学习Andrew Ng的[机器学习系列课程][25]，里面的练习都可以使用Python完成。

**小任务**：在Kaggle上试试这个[挑战][26]

### 第7步：练习，练习，还是练习

祝贺你，终于来到这里，相信你可以做到了上面六步！

现在你拥有了所有需要的技能，关键就是练习了，相信没有什么比在Kaggle上与数据科学家一同竞赛的练习更棒的了。走，参加Kaggle上正在举行的比赛去，一展所学！

### 第8步：深度学习

现在你学到了很多机器学习的技术技能，那么是时候接触“深度学习”了，也许你已经知道什么是深度学习了，但是这里还是做了一个[简介][27]，也许看了有收获哦。

我也是一个深度学习方面的新手，所以以下建议仅供参考。最详尽的资料资源在[deeplearning.net][28]。你将找到你需要的一切，课程，数据集合，挑战，教程。您也可以试试[Geoff Hinton的课程][29]，以了解神经网络的基础知识。

开启Python之旅：[一个完整的从头开始使用Python学习数据科学的教程][30]

PS:如果你要使用大数据处理库，可以试试Pydoop和PyMongo。大数据处理就是另外一个话题了不在此展开了。

原文链接：[https://www.analyticsvidhya.com/learning-paths-data-science-business-analytics-business-intelligence-big-data/learning-path-data-science-python/][31]

  [1]: https://www.analyticsvidhya.com/blog/2015/05/infographic-quick-guide-learn-python-data-science/
  [2]: https://store.continuum.io/cshop/anaconda/
  [3]: https://mirrors.tuna.tsinghua.edu.cn/help/anaconda/
  [4]: https://www.datacamp.com/courses/intro-to-python-for-data-science
  [5]: https://www.datacamp.com/courses/intro-to-python-for-data-science
  [6]: https://developers.google.com/edu/python/
  [7]: https://developers.google.com/edu/python/regular-expressions
  [8]: https://www.debuggex.com/cheatsheet/regex/python
  [9]: https://docs.scipy.org/doc/numpy-dev/user/quickstart.html#
  [10]: http://docs.scipy.org/doc/scipy/reference/tutorial/
  [11]: http://nbviewer.jupyter.org/github/jrjohansson/scientific-python-lectures/blob/master/Lecture-4-Matplotlib.ipynb
  [12]: http://pandas.pydata.org/pandas-docs/stable/10min.html
  [13]: http://www.gregreda.com/2013/10/26/intro-to-pandas-data-structures/
  [14]: https://www.datacamp.com/courses/pandas-foundations2013/10/26/intro-to-pandas-data-structures/
  [15]: https://www.analyticsvidhya.com/blog/2016/01/complete-tutorial-learn-data-science-python-scratch-2/
  [16]: https://www.analyticsvidhya.com/blog/2014/09/data-munging-python-using-pandas-baby-steps-python/
  [17]: http://nbviewer.jupyter.org/github/cs109/2014/blob/master/homework/HW1.ipynb
  [18]: http://cs109.github.io/2014/pages/schedule.html
  [19]: http://nbviewer.jupyter.org/github/cs109/2014/blob/master/homework/HW2.ipynb
  [20]: https://www.datacamp.com/courses/interactive-data-visualization-with-bokeh
  [21]: https://www.analyticsvidhya.com/blog/2015/01/scikit-learn-python-machine-learning-tool/
  [22]: http://cs109.github.io/2014/pages/schedule.html
  [23]: https://www.amazon.cn/s/ref=nb_sb_ss_c_1_9?__mk_zh_CN=%E4%BA%9A%E9%A9%AC%E9%80%8A%E7%BD%91%E7%AB%99&url=search-alias=aps&field-keywords=Programming%20Collective%20Intelligence&sprefix=python%20ke,aps,161&crid=1006JKT7AW9KZ
  [24]: https://www.edx.org/course/learning-data-introductory-machine-caltechx-cs1156x-0
  [25]: https://www.coursera.org/course/ml
  [26]: http://www.kaggle.com/c/data-science-london-scikit-learn
  [27]: https://www.analyticsvidhya.com/blog/2014/06/deep-learning-attention/
  [28]: http://deeplearning.net/
  [29]: https://www.coursera.org/course/neuralnets
  [30]: https://www.analyticsvidhya.com/blog/2016/01/complete-tutorial-learn-data-science-python-scratch-2/
  [31]: https://www.analyticsvidhya.com/learning-paths-data-science-business-analytics-business-intelligence-big-data/learning-path-data-science-python/