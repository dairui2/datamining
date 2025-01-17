NLP/TF-IDF(客服对话分析)；K-Means聚类(客户价值分析,广告效果分析)；Lasso回归(SVR销售预测分析)；Apriori关联(商品组合分析); IsolationForest异常检测

NLP/TF-IDF 客服对话分析
1. 对语料进行分词处理
2. 添加自定义词典/jieba.add_word()
3. 生成停用词/excluded_flag = []
4. 关键词提取/TF-IDF
5. 词云
   <img width="1279" alt="image" src="https://github.com/dairui2/dataMining/assets/31460898/d5dd526d-ffe9-4e0d-ac3b-44abaa66be0d">


K-Means聚类 客户价值分析，广告效果分析
1. 读入数据并进行数据预处理
2. 数据标准化
   2.1 读入数据
   2.2 提取特征列并改索引
   2.3 标准化
4. 使用K-Means聚类算法对客户进行分析
   3.1 肘部法确定K值
   3.2 K-Means聚类分析
   3.3 提取整合聚类结果
   3.4 分析两种K值结果
   3.5 将类别与客户数据对应
   3.6 保存聚类分析好的数据
5. 数据可视化及数据分析
   <img width="1279" alt="image" src="https://github.com/dairui2/dataMining/assets/31460898/3ec0a513-77a4-4e87-9f5d-ffeb1b331b65">




Lasso回归 销售预测分析

0. 回归分析的过程：0.1 收集一组包含因变量(目标y)和自变量(预测器x)的数据；0.2 根据因变量和自变量之间的关系，初步设定回归模型；0.3 求解合理的回归系数；
   0.4进行相关性检验，确定相关系数；0.5 利用模型对因变量做出预测，并计算预测值的置信区间。
1. 应用场景：当原始特征中存在多重共线性时，Lasso回归可以有效的对存在多重共线性的特征进行删选。
2. 基本原理：以缩小特征集为思想，将特征系数进行压缩，将惩罚项由L2范数变为L1范数，将一些不重要的回归系数缩减为0，进而达到特征选择的目的(寻求模型稀疏表达)。
   <img width="810" alt="image" src="https://github.com/dairui2/dataMining/assets/31460898/31bc58df-d148-4f7f-a9a2-271f71a45daa">




Apriori关联(商品组合分析 套餐SKU, CF协同过滤推荐)

1. 应用场景：购物篮分析(捆绑销售、商品陈列设计、页面促销设计、推荐系统等)，通过分析用户同时购买了哪些商品来分析用户购物习惯。
2. 频繁规则：关联结果中 支持度Support = P((A,B)|ALL) = P(B&A)/P(ALL) 和 置信度Confidence = P(B|A) = P(B&A)/P(A)都比较高的规则。
3. 有效规则：关联规则中真正能促进规则中的前(A)/后(B)项的提升。
4. 提升度：Lift = P(B|A)/P(B)。
   4.1 当提升度为1时，说明应用关联规则和不应用关联规则产生相同的结果；
   4.2 当提升度大于1时，说明应用关联规则比不应用关联规则产生更好的结果；
   4.3 当提升度小于1时，说明关联规则具有负相关(互斥)的作用，该规则是无效规则。

![image](https://github.com/user-attachments/assets/5e3e0c4a-e8c9-4416-a568-ede1f02427f1)



IsolationForest异常检测(网站广告流量的异常识别与检测)
1. 应用场景：异常订单识别，黄牛识别，风险预警，欺诈检测
<img width="973" alt="image" src="https://github.com/user-attachments/assets/534b8e14-0dca-41c2-86d9-9c58dea168f0">


