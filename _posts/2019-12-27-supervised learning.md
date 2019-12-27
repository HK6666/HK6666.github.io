---
layout:     post                    # 使用的布局（不需要改）
title:      有监督学习            # 标题
subtitle:   Hello AI #副标题
date:       2019-12-27            # 时间
author:     hk                      # 作者
header-img: img/post-bg-2015.jpg    #这篇文章标题背景图片
catalog: true                       # 是否归档
tags:                               #标签
    - 机器学习入门
---

1.什么时候使用有监督学习，什么时候使用无监督学习

    有可靠的样本的时候采用有监督学习，对于一些比较简单的训练可采用肉眼观察的方式观察出样本？

2.监督学习的问题主要有两种，分别是分类classification和回归regression。

    分类： 分类问题的目的是预测类别标签class label，这些标签来自预定义的可选列表。
    回归： 回归任务的目的是预测一个连续值，也叫作浮点数floating-point number，即预测值不是一个类别而是一个数字值。打个比方，假如要根据一个人的年龄学历等feature来预测这个人的收入，那么预测值为一个金额，可以在给定范围内任意取值。

3.区分分类与回归

    最好的办法就是看输出是否具有某种连续性，如果在可能的结果之间具有连续性，那么它就是一个回归问题。

泛化 generalize：

    如果一个模型能对没有见过的数据做出准确的预测，那么就表明这个模型能从训练集generalize到测试集。

过拟合 overfitting 欠拟合 underfitting：

    如果我们总想找到最简单的模型，构建与一个对于现有信息量过于复杂的模型，即在拟合模型的时候过分关注训练集的细节，得到了一个与训练集上表现很好但是不能泛化到新数据上的模型，那么就是overfitting过拟合。反之，如果模型过于简单，无法抓住数据的全部内容以及数据中的变化，甚至在训练集上表现就很差，那么就是underfitting欠拟合。
    所以，在二者之间存在一个最佳位置，找到这个位置就是我们最想要的模型

![冲冲冲](https://timgsa.baidu.com/timg?image&quality=80&size=b9999_10000&sec=1577420892401&di=712e018341a9ba985bf75cba553920df&imgtype=0&src=http%3A%2F%2Fwww.koudai8.com%2Fnewbbs%2Fdata%2Fattachment%2Falbum%2F201502%2F26%2F022510oh9gaghjg8y30yjg.png)