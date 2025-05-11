# Games101 Experiment5

## 实验内容

- 实现Whitted style ray tracing。
- 本次实验中比较关键的两个函数，一个即为Render, 第二个即为rayTriangleIntersect函数。
- 其中，Render里面主要实现如何计算从摄像机发射到像素的光线的向量。主要思路即为，首先将屏幕坐标转变为裁剪空间中，近平面上的坐标。之后首尾相减，即可获得光线的向量
- rayTriangleIntersect函数主要用于判断光线是否和三角形相交。如果相交，同时还返回交点的中心坐标，以及光线的tNear。判断的方法主要是使用Möller Trumbore算法。



## 实验结果

- <img src="C:\Users\i love china\AppData\Roaming\Typora\typora-user-images\image-20250511170424537.png" alt="image-20250511170424537" style="zoom:67%;" />
- 可以看到，Whitted style ray tracing 比较好地处理了折射和反射的效果。