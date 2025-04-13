## 📊 1. 基础折线图（Line Plot）

这是最基础的一种图，用于展示连续数据的趋势。

```python
import matplotlib.pyplot as plt

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

![折线图](https://chatgpt.com/images/line_plot_demo.png)