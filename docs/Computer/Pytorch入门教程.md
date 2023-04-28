---
comments: true

---

参考[csdiy.wiki](https://csdiy.wiki)的教程模板制作: )
# PyTorch深度学习快速入门教程（小土堆）

## 教程简介

- 编程语言：Python
- 教程难度：🌟
- 预计学时：

教程从数据加载开始，介绍了Tensorboard的使用、Transform对Tensor数据进行转化，也介绍了神经网络的搭建过程、常用的损失函数、常用的优化器等内容。教程可以作为PyTorch入门教程使用，对于初学者比较友好，可用于学习理论以后动手实操的开始。

## 教程资源

- 教程网站：[【PyTorch深度学习快速入门教程（绝对通俗易懂！）【小土堆】】](https://www.bilibili.com/video/BV1hE411t7RN/?p=23&share_source=copy_web&vd_source=8d1c3033412c6507322ab8cb464a1a5c)
- 其他资源见视频简介部分。

## 教程笔记（部分）

???+ danger "danger"
    笔记尚未构建完成



### Loss function 损失函数
计算结果和目标结果的误差，称为损失函数。torch.nn中几个常见的损失函数，可以参见[官方文档](https://pytorch.org/docs/stable/nn.html#loss-functions)：

- L1Loss（平均绝对误差MAE，mean absolute error）
- MSELoss（均方误差MSE，mean squared error）
- CrossEntropyLoss（交叉熵）
	- The input is expected to contain the unnormalized logits for each class.

损失函数也可以为更新输出提供一定的依据，此方法为反向传播。
### 常见的优化器

