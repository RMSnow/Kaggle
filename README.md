# Kaggle

## Titanic

### TODO

- Python

  - matplotlib
  - pandas

- Data Mining & Machine Learning

  - Feature Engineering
  - Cross Validation
  - Model Ensemble
    - Bagging


  - Random Forest

### Notes

- 通常遇到缺值的情况，我们会有几种常见的处理方式
  - 如果**缺值的样本占总数比例极高**，我们可能就直接**舍弃**了，作为特征加入的话，可能反倒带入noise，影响最后的结果了
  - 如果缺值的样本适中，而该属性**非连续值特征属性**(比如说类目属性)，那就把NaN作为一个新类别，加到类别特征中
  - 如果缺值的样本适中，而该属性为**连续值特征属性**，有时候我们会考虑给定一个step(比如这里的age，我们可以考虑每隔2/3岁为一个步长)，然后把它**离散化**，之后把NaN作为一个type加到属性类目中。
  - 有些情况下，缺失的值个数并不是特别多，那我们也可以试着根据已有的值，拟合一下数据，补充上。

- 对于任何的机器学习问题，不要一上来就追求尽善尽美，**先用自己会的算法撸一个baseline的model出来，再进行后续的分析步骤，一步步提高**。

  在问题的结果过程中：

  - **『对数据的认识太重要了！』**
  - **『数据中的特殊点/离群点的分析和处理太重要了！』**
  - **『特征工程(feature engineering)太重要了！』**
  - **『模型融合(model ensemble)太重要了！』**

- 用机器学习解决问题的大致过程：

  ![1](http://7xo0y8.com1.z0.glb.clouddn.com/2_titanic/process.png?imageView/2/w/700/q/100)

