NLP/TF-IDF(客服对话分析)；K-Means聚类(客户价值分析,广告效果分析)；Lasso回归(SVR销售预测分析)；Apriori关联(商品组合分析)

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
   <img width="799" alt="image" src="https://github.com/dairui2/dataMining/assets/31460898/624e053c-da76-48c9-b181-48bf96a770e8">

Lasso回归 销售预测分析
   <img width="810" alt="image" src="https://github.com/dairui2/dataMining/assets/31460898/31bc58df-d148-4f7f-a9a2-271f71a45daa">


Apriori关联(商品捆绑销售)

应用场景：购物篮分析(捆绑销售、商品陈列设计、页面促销设计、推荐系统等)，通过分析用户同时购买了哪些商品来分析用户购物习惯。

频繁规则：关联结果中 支持度Support = P((A,B)|ALL) = P(B&A)/P(ALL) 和 置信度Confidence = P(B|A) = P(B&A)/P(A)都比较高的规则。

有效规则：关联规则中真正能促进规则中的前(A)/后(B)项的提升。

提升度：Lift = P(B|A)/P(B)。
当提升度为1时，说明应用关联规则和不应用关联规则产生相同的结果；
当提升度大于1时，说明应用关联规则比不应用关联规则产生更好的结果；
当提升度小于1时，说明关联规则具有负相关(互斥)的作用，该规则时无效规则。
<img width="589" alt="image" src="https://github.com/dairui2/dataMining/assets/31460898/58c459ef-ac89-4e20-a70d-348e178ea0ea">
