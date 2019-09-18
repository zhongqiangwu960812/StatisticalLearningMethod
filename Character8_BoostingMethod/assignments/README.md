## AdaBoost集成算法编程实践
> 这次作业分两部分，第一部分是根据AdaBoost思想自己编程实现AdaBoost算法进行分类， MyAdaboost.ipynb是自编程实现的代码，重点是理解思想，这个代码
展现了numpy的重大功能。
> 
> MyAdaBoost.ipynb文件：
>> * 初始化样本权值w
>> * 求第一个弱分类器G1： 找到使加权分类误差率最低的阈值v
>> * 根据分类误差率计算G1的系数α1
>> * α1G1+α2G2对训练数据进行训练
>>> * 如果分类误差率在可接受范围内，迭代停止
>>> * 如果分类误差率不可接受，更新样本权值w， 进行下一次迭代
>
> AdaBoost.skl文件是基于sklearn.ensembles 下面的AdaBoostClassifier分类器， 并且复习了一下Python实践的评估方法，这个模型的参数不是太多，
要会使用。
>
> 笔记链接：http://note.youdao.com/noteshare?id=f21ee24670710232efd9633d19085b96&sub=0C69D88B6C154F96A776D09F7C969E5D
