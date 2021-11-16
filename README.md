# House-price-prediction
This is a project from Kaggle "Housing Prices Competition for Kaggle Learn Users"
From url: https://www.kaggle.com/c/home-data-for-ml-course/data


What i do:
  - use Mutual Information to calculate how important each column is to the target and delete unwanted column
  - use Imputation and one-hot encoding to further clean the data
  - use grid search to select best option for model
  




这是一个在Kaggle上的， 提供给学习数据分析者的项目，
关于项目的具体信息，你可以在这里找到：https://www.kaggle.com/c/home-data-for-ml-course/data

我在这个项目中做了什么：
  -通过Mutual Information计算了数据中的每一列（即一个标签，比如“房子的面积”）对于目标（即预测对象，如“房子的价钱”）之间的联系，对无效的信息进行去除
  -使用SimpleImputer对部分缺失信息进行填充，然后将数据进行One-hot encodeing （独热编码）进一步清理了数据。
  -利用grid search尝试并选取了最有效的模型选项，减少了训练模型中的大量误差。
  -经过重复的尝试，截至2021.11.15(加拿大时间)，我在kaggle上的该项目排名为251/27633 （top 1%）
  

