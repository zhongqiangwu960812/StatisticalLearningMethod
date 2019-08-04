## KNN编程实践
> 本次编程作业，也是就课本上的一个例题， 给出6个训练样本，一个测试样本， 通过自编程调包实现对测试样本的分类
>本次作业两个文件：<br> 
>>1. MyKNN.ipynb文件是用线性扫描算法自编程实现的K近邻算法，分为下面几个步骤：<br>
  * 计算欧式距离
  * 欧式距离排序
  * 取前K个最小距离， 对应训练数据点的类型y
  * 对k个y值进行统计
  * 返回频率出现最高的y值
>>然后对基本的线性回归算法进行改进， 并附加了kd树的算法， 并且学习了Python的几个模块： time， collection， linalg, heapq, concurrent模块的使用
>>
>> 2. skl_KNN.ipynb 是调用了sklearn.neighbors的KNeighborsClassifier模块， 对测试点进行预测。<br> 主要就是模块的参数和方法要会用，知道含义
>
> 笔记链接：http://note.youdao.com/noteshare?id=68ff9f335c7254cb3790ac6a70fa8d54&sub=E0481A1F1AD44D1DAEF2EF0F2358DC6C
