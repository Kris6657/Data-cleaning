# 📊 数据清洗实践指南

## 🌟 概述
### 1. 数据清洗核心任务
- 🛠 **错误处理**  
  修正格式错误、异常值与逻辑矛盾（如负年龄、错误日期格式）。  
- 🕳 **缺失值处理**  
  分析缺失模式，采用插补、删除或标记策略，保留数据完整性。  
- 🔄 **重复数据处理**  
  识别并移除冗余记录，确保数据唯一性。  
- 📏 **数据标准化**  
  统一单位、格式与数据类型（如货币转换、日期标准化）。  
- 🧩 **数据整合**  
  合并多源数据，解决字段冲突与结构差异。

---

### 2. 推荐数据集资源
#### 🔍 权威平台
[![UCI](https://img.shields.io/badge/UCI_ML_Repo-经典数据集-003f5c)](https://archive.ics.uci.edu/)  
[![Kaggle](https://img.shields.io/badge/Kaggle-社区数据集-F37626)](https://www.kaggle.com/datasets)

#### 💡 使用提示
- 🌸 **Kaggle 访问问题**  
  若验证码无法加载，参考 [解决方案](https://blog.azurezeng.com/recaptcha-use-in-china/) 配置网络环境。  
- 📥 **数据下载技巧**  
  使用 Kaggle API 或浏览器插件快速获取数据，详见 [知乎指南](https://zhuanlan.zhihu.com/p/266570781)。

---

## 📚 案例概览
### 🚢 案例一：泰坦尼克生存预测
**技术亮点**  
- 删除低信息量特征（如船舱号）  
- 多维度处理缺失值（年龄插补 vs 登船港口删除）  
- 基于业务逻辑筛选有效特征  

**数据来源**  
[Kaggle 竞赛数据集](https://www.kaggle.com/c/titanic)

---

### 📖 案例二：古籍元数据清洗
**技术亮点**  
- 正则表达式提取出版年份  
- 条件替换实现地名标准化（如 "London" 与 "Oxford" 统一）  
- 类型转换优化存储效率  

**参考实现**  
[mramshaw/Data-Cleaning](https://github.com/mramshaw/Data-Cleaning)

---

### 🚕 案例三：纽约出租车轨迹分析
**技术亮点**  
- 地理坐标异常值过滤（基于纽约地理边界）  
- 蒙特卡洛模拟补全缺失坐标  
- 热力图可视化出行热点分布  

**数据来源**  
[纽约市出租车委员会](https://www.nyc.gov/site/tlc/about/tlc-trip-record-data.page)

---

## 🙌 致谢
- **案例一** 灵感来自 [agconti/kaggle-titanic](https://github.com/agconti/kaggle-titanic)  
- **案例二** 参考 [RealPython 数据清洗教程](https://realpython.com/python-data-cleaning-numpy-pandas/)  
- **案例三** 数据由 NYC TLC 官方公开提供  

---

## 🛠️ 工具依赖
```bash
# 核心库
pandas numpy matplotlib

# 进阶功能
folium>=0.14.0  # 地理可视化
geopy           # 地理坐标计算
```

---
## ✨ 整理：KrisZheng @ GitHub
📅 更新日期：2024-01-20
