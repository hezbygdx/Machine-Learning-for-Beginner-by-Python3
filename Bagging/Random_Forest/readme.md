# Random Forest

+ **随机森林步骤**

   1. **构建多个数据集**

    在包括N个样本的数据集中，采用有放回的抽样方式选择N个样本，构成中间数据集，然后在这个中间数据集的所有特征中随机选择几个特征，作为最终的数据集。以上述方式构建多个数据集；
    
   2. **为每个数据集建立完全分裂的决策树**
      
     利用CART为每个数据集建立一个完全分裂的决策树，最终得到多个CART决策树；
     
   3. **预测新数据**
   
     得到每一个决策树对于这个新数据的预测值。回归问题：采用多棵树的平均值。分类问题：采用投票计数的方法，票数大的获胜，相同的随机选择。可以把树的棵树设置为奇数避免这一问题。

+ **随机森林文件说明**

  + **回归问题：北京市pm2.5预测**
  
     + 数据处理：[pm25_RF_Data.py](https://github.com/Anfany/Machine-Learning-for-Beginner-by-Python3/master/Bagging/Random_Forest/pm25_RF_Data.py)
     
     + 模型建立：[pm25_RF_Regression.py](https://github.com/Anfany/Machine-Learning-for-Beginner-by-Python3/master/Bagging/Random_Forest/pm25_RF_Regression.py)
     
     + 结果图示
     
         + 方法选择
         
         ![image](https://github.com/Anfany/Machine-Learning-for-Beginner-by-Python3/master/Bagging/Random_Forest/method.jpg)
         
        + 预测真实值与输出值对比曲线
         
         ![image](https://github.com/Anfany/Machine-Learning-for-Beginner-by-Python3/master/Bagging/Random_Forest/duibi.jpg)
         
  
  
  + **分类问题：成年人收入**
    
     + 数据处理：
     
     + 模型建立
     
     + 结果图示