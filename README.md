# 🎯 目标编码（Target Encoding）演示项目

本项目演示了如何使用 Python 实现分类变量的目标编码（Target Encoding）方法，适用于机器学习建模前的特征工程阶段。

---

## 📌 项目内容

本项目包含以下内容：

- 分类变量的目标编码原理简介
- 使用 Pandas 实现简易的目标编码函数
- 演示在样例数据中对目标列进行编码转换
- 探索编码结果对建模的影响（可扩展）

---

## 📁 文件结构

```
target-encoding-demo/
├── 目标编码Target Encoding 函数.ipynb  # Jupyter Notebook 主体
├── README.md                             # 项目说明文件（本文件）
```

---

## 📊 什么是 Target Encoding？

目标编码是一种将分类变量转换为数值特征的方式，常用于树模型（如 XGBoost、LightGBM）中特征工程。其原理是：

> 对每一个类别，使用该类别对应的目标值（如回归目标的均值，或分类目标的概率）进行替换。

优点包括能保留分类变量对目标变量的预测性，缺点是容易过拟合，需配合正则化或交叉验证策略使用。

---

## 🚀 快速开始

确保你已安装如下环境：

```bash
pip install pandas numpy scikit-learn
```

打开 `目标编码Target Encoding 函数.ipynb` 即可运行全部单元格，了解目标编码函数的定义与应用过程。

---

## 🧠 拓展方向（建议）

- 引入交叉验证内的目标编码实现，避免数据泄漏
- 将目标编码封装为 sklearn 风格的转换器
- 比较编码前后的模型性能差异

---

## 📎 项目用途

- 适合用于教学、面试准备、特征工程入门训练
- 可扩展为更完整的建模 pipeline 模板

---

## 📌 作者说明

由 ChatGPT 辅助生成与结构优化，适用于数据科学初学者、机器学习课程项目等。

---
