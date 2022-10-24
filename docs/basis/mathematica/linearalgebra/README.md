# 线性代数

#### 1.前言

- “线性”，指的就是如下的数学关系：

  <font size = 5>$f(x+y) = f(x) + f(y)$</font>

  。其中，$f$叫线性算子或线性映射。所谓“代数”，指的就是用符号代替元素和运算，也就是说：我们不关心上面的*x*，*y*是实数还是[函数](https://baike.baidu.com/item/函数/301912?fromModule=lemma_inlink)，也不关心*f*是[多项式](https://baike.baidu.com/item/多项式?fromModule=lemma_inlink)还是微分，我们统一把他们都抽象成一个记号，或是一类矩阵。合在一起，线性代数研究的就是：满足线性关系

  <font size = 5>$f(x+y) = f(x) + f(y)$</font>

  的[线性算子](https://baike.baidu.com/item/线性算子?fromModule=lemma_inlink)$f$都有哪几类，以及他们分别都有什么性质(摘自百度百科)

#### 2.个人理解

- 关于矩阵
  - 矩阵是可以成表述两种不同基坐标转换关系
  - 矩阵其本质是某一正交基(x,y互不影响)对另一正交基的分量贡献比值，是研究向量的一门学科
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
  - 在三维空间内，物体的forward，up，right为矩阵三轴，只要单独把缩放乘进去就能获取起转换坐标

### [1.矩阵与高斯消元](MatricesAndGaussianElimination.md)

- 1.线性变换的几何解释

