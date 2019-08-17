## 决策树编程实践
> 本次作业，课本上的题目练习， 15个训练样本， 3个测试样本， 通过调sklearn.tree.DecisionTreeClassifier模型实现，自编程实现了一下，有点繁琐，这次重点
主要是会调用包，理解参数。自己写的话太费时间。
>> 1. MyDecisionTree.ipynb文件是自编程实现的决策树模型，根据信息增益或者信息增益比规则进行的特征选择，包括决策树的生成和预测，剪枝部分没有写
>> 2. Skl_DT.ipynb是基于sklearn.tree.DecisionTreeClassifier模型是实现决策树，并通过tree.graphviz可视化决策树，主要思路：<br>
>> (1)根据表构造数据集<br>
>> (2)由于训练集中的特征都是字符串，所以这里需要一个数据预处理，转成数字表示<br>
>> (3)调用sklearn包建立决策树模型<br>
>> (4)用得到的模型在测试集上进行预测，输出结果<br>
>> (5)可视化决策树模型<br>
>
>重点就是调包的参数需要知道并且会用， 可视化那里简单的看一下，数据预处理也是重点，因为如果碰到数据集的特征是字符串的时候（决策树这里的问题普遍都是字符串）
这时候，需要先进性数据预处理，也就是先把字符串特征进行数字化度量，比如年龄特征{青年，中年，老年}，用LabelEncoder对象编码之后，就是（0,1,2）。这样每个
特征进行编码之后，再进行训练预测等操作。 当然，编码也有两种方法，一种是基于每个特征的编码，一个是基于整体特征的编码，在第二个文件中都有给出。这个
是重点。 有的模型在处理之前还需要OneHotEncoder编码，这个不需要。 调用模型的时候，一定要看好模型处理什么样的数据。
>
>笔记链接：http://note.youdao.com/noteshare?id=59a848dbe286b4215137a8121c070dcf&sub=091C5AA30AF4456B87E6B28DF632B8A1