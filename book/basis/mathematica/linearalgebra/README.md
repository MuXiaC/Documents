# 线性代数

### 前言

- 关于矩阵
  - 矩阵是可以成表述两种不同基坐标转换关系
  
  - 矩阵其实是两坐标系源坐标分量关系，例如：B坐标系的X轴是A坐标系下X,Y,Z三轴的贡献率，B3轴的贡献即为矩阵AB，可表示为:
    $
    \left[
    \begin{matrix}
    {B_x/A_x}&{B_x/A_y}&{B_x/A_z}\\
    {B_y/A_x}&{B_y/A_y}&{B_y/A_z}\\
    {B_z/A_x}&{B_z/A_y}&{B_z/A_z}\\
    \end{matrix}
    \right] \tag{1}
    $
  
  - 从坐标系A转到坐标系B， 以A为原基坐标系，计算B坐标系对于A坐标系的关系(即A的单位坐标和B的单位坐标的倍率关系)，即矩阵A->B，矩阵AB是，如果是原A坐标系的P点，简称P_A，当矩阵ABxP_A时候代表P_A旋转缩放了矩阵AB，当矩阵ABxP_B(P_B类比P_A)，表示P_B点在A坐标系的点值，现在渲染流水所用的顶点变换的矩阵都是点ABxP_B，而点ABxP_A是用来做旋转缩放的

### [1.矩阵与高斯消元](MatricesAndGaussianElimination.md)

- 1.线性变换的几何解释

