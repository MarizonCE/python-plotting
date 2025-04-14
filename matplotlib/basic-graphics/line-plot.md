## 📊 1. 基础折线图（Line Plot）

这是最基础的一种图，用于展示连续数据的趋势。

```python
import matplotlib.pyplot as plt


plt.rcParams['font.family'] = 'SimHei'  # 设置为黑体
plt.rcParams['axes.unicode_minus'] = False  # 解决负号显示为方块的问题

# 模拟一些数据
x = [1, 2, 3, 4, 5]
y = [1, 4, 9, 16, 25]

# 创建图像和坐标轴
plt.figure(figsize=(8, 5))  # 设置图像大小
plt.plot(x, y, color='blue', linestyle='-', marker='o', label='y = x²')

# 添加标题和标签
plt.title('简单的折线图', fontsize=14)
plt.xlabel('X 轴')
plt.ylabel('Y 轴')

# 添加图例
plt.legend()

# 显示图像
plt.show()
```

> 📷 效果图如下：

![屏幕截图 2025-04-14 011659](http://img.marizonce.com//20250414103706577.png)
