# 个人项目：申请信用评分卡模型

本项目根据“天池O2O优惠券使用预测”提供的数据，对淘宝投放的优惠券是否消费进行预测。

项目将数据根据时间进行合理划分，在进行数据缺失值、重复值和异常值处理后，对原始数据进行特征衍生，共得56个衍生变量。在进行特征筛选（卡方检验、多重共线性检验、相关系数检验）后，分别用KNN模型、LR模型、AdaBoost模型和RF模型进行训练，并对优惠券是否消费进行预测。

通过各个模型ROC曲线和AUC值的比较，最终发现LR模型的精度（88%）最高。

本项目的不足之处在于时间划分的主观性和局限性，评价模型优劣的标准也过于单一。
