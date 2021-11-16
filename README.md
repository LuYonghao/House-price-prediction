# House-price-prediction
This is a project from Kaggle "Housing Prices Competition for Kaggle Learn Users"
From url: https://www.kaggle.com/c/home-data-for-ml-course/data


What i do:
  - use Mutual Information to calculate how important each column is to the target and delete unwanted column
  - use Imputation and one-hot encoding to further clean the data
  - use grid search to select best option for model
as of 2021.11.15, ranking 251/27633 on leaderBoard (top 1%)
  
<br/>
<br/>
<br/>


这是一个在Kaggle上的， 提供给学习数据分析者的项目<br/>
关于项目的具体信息，你可以在这里找到：https://www.kaggle.com/c/home-data-for-ml-course/data<br/>
<br/>
描述：<br/>
  让购房者描述他们梦想中的房子，他们可能不会从地下室天花板的高度或与东西铁路的接近程度开始。但是这个游乐场比赛的数据集证明，与卧室数量或白色栅栏相比，对价格谈判的影响要大得多。<br/>
  凭借 79 个解释变量（几乎）描述了爱荷华州艾姆斯住宅的各个方面，这项竞赛挑战您预测每栋房屋的最终价格。<br/>
  <br/>
实际目标：<br/>
  清理杂乱的，有缺失的数据，建立有效模型，根据已有房型数据，预测房价。<br/>
<br/>
我在这个项目中做了什么：<br/>
  &nbsp;&nbsp;-通过Mutual Information计算了数据中的每一列（即一个标签，比如“房子的面积”）对于目标（即预测对象，如“房子的价钱”）之间的联系，对无效的信息进行去除<br/>
  &nbsp;&nbsp;-使用SimpleImputer对部分缺失信息进行填充，然后将数据进行One-hot encodeing （独热编码）进一步清理了数据。<br/>
  &nbsp;&nbsp;-利用grid search尝试并选取了最有效的模型选项，减少了训练模型中的大量误差。<br/>
经过重复的尝试，截至2021.11.15(加拿大时间)，我在kaggle上的该项目的排名为251/27633 （top 1%）<br/>
 
![alt text](https://github.com/LuYonghao/House-price-prediction/blob/main/House%20Data/img/HouseRank.png)

<br/>
<br/>

# 关于 Mutual Information
使用了 sklearn.feature_selection
在 feature_selection 中，有 mutual_info_regression 和 mutual_info_classif 两个选项， 
由于本数据集的目标是预测价钱，而非分类，故选用 mutual_info_regression 打出分数，
然后使用 matplotlib.pyplot 来制作图像，以方便比对和展示：
![alt text](https://github.com/LuYonghao/House-price-prediction/blob/main/House%20Data/__results___files/__results___7_0.png)
![alt text](https://github.com/LuYonghao/House-price-prediction/blob/main/House%20Data/__results___files/__results___7_1.png)
![alt text](https://github.com/LuYonghao/House-price-prediction/blob/main/House%20Data/__results___files/__results___8_0.png)
![alt text](https://github.com/LuYonghao/House-price-prediction/blob/main/House%20Data/__results___files/__results___8_1.png)
<br/>
然后去除最糟糕选项

<br/>

文件列表(file list):<br/>
  -house-price-prediction.ipynb (全部代码，步骤，包括comment)<br/>
  -House Data<br/>
        &nbsp;-results_files (储存资料图片）<br/>
        &nbsp;-img（储存其他图片）<br/>
        &nbsp;data_description.txt (数据类型的描述）<br/>
        &nbsp;submission.csv(最后需要提交的结果)<br/>
        &nbsp;test.csv（测试数据，用来生成结果）<br/>
        &nbsp;train.csv（训练用数据）<br/>
         





