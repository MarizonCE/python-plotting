## ✅ 文件结构：`matplotlib/basics.md`

~~~markdown
# 🎯 Matplotlib 基础教程 | Basics of Matplotlib

`matplotlib` 是 Python 中最基础、最强大的绘图库之一。本节将带你快速入门它的核心用法，包括创建图像、绘制线图、添加标题/标签/图例，以及保存图像等内容。

---

## 📌 环境准备

确保你已经安装了 `matplotlib`，可以通过以下命令安装：

```bash
pip install matplotlib
~~~

------

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

> 📷 效果图如下（文件路径建议保存为 `images/line_plot_demo.png`）：

![折线图](https://chatgpt.com/images/line_plot_demo.png)

------

## 🧱 2. 多条线绘制（Multiple Lines）

你可以在一张图里画出多条线：

```python
import matplotlib.pyplot as plt

x = [1, 2, 3, 4, 5]
y1 = [1, 2, 3, 4, 5]
y2 = [1, 4, 9, 16, 25]

plt.plot(x, y1, label='线性', color='green')
plt.plot(x, y2, label='平方', color='red')

plt.title('多线绘图示例')
plt.xlabel('X')
plt.ylabel('Y')
plt.legend()
plt.grid(True)  # 添加网格线

plt.show()
```

------

## 🗂️ 3. 保存图像（Save to File）

你可以将图像保存成 PNG、SVG、PDF 等格式：

```python
plt.savefig('images/my_plot.png', dpi=300)  # 保存图像，确保文件夹存在
```

------

## 🔤 4. 中文字体支持（可选）

Matplotlib 默认不支持中文，需要额外设置字体：

```python
plt.rcParams['font.family'] = 'SimHei'  # 黑体
plt.rcParams['axes.unicode_minus'] = False  # 解决负号显示问题
```

> 📝 Windows 上建议使用 `'SimHei'`，Mac 用户可以尝试 `'Arial Unicode MS'` 或 `'PingFang SC'`。

------

## ✅ 小结

本节我们学习了：

- 如何用 `matplotlib` 绘制基础折线图
- 添加标题、标签、图例、网格
- 保存图像文件
- 中文显示设置（可选）

👉 下一节我们将介绍 **散点图、柱状图、子图（subplot）** 等进阶内容！

------

## 📎 延伸阅读

- 官方文档：https://matplotlib.org/stable/index.html
- 中文教程推荐：[廖雪峰的教程](https://www.liaoxuefeng.com/wiki/1016959663602400/1017639890281664)

------

