## 📊 1. 基础折线图（Line Plot）

这是最基础的一种图，用于展示连续数据的趋势。

```python
import matplotlib.pyplot as plt

# 设置中文字体和负号正常显示
plt.rcParams['font.family'] = 'SimHei'  # 黑体
plt.rcParams['axes.unicode_minus'] = False  # 负号

# 数据
x = [1, 2, 3, 4, 5]
y = [1, 4, 9, 16, 25]

# 绘图
plt.figure(figsize=(8, 5))
plt.plot(x, y, color='blue', linestyle='-', marker='o', label=r'$y = x^2$')  # 使用 LaTeX 表达式显示上标

# 标题和标签
plt.title('简单的折线图', fontsize=14)
plt.xlabel('X 轴')
plt.ylabel('Y 轴')

# 图例
plt.legend()

# 显示
plt.show()

```

> 📷 效果图如下：

![image-20250414110344632](http://img.marizonce.com//20250414110344924.png)
