## g2o的基本框架结构

![Alt text](image.png)


<https://mp.weixin.qq.com/s?__biz=MzIxOTczOTM4NA==&mid=2247486992&idx=1&sn=ecb7c3ef9bd968e51914c2f5b767428d&chksm=97d7eb87a0a062912a9db9fb16a08129f373791fd3918952342d5db46c0bc4880326a7933671&cur_album_id=1361700104461467649&scene=189#wechat_redirect>

边通常表示误差项
来优化非线性误差函数的c++框架



LM
<https://blog.csdn.net/u010881576/article/details/119810518>


LM算法（Levenberg-Marquardt算法）是一种用于非线性最小二乘问题的优化算法。它可以用于求解参数估计、曲线拟合等问题。

LM算法可以被看作是一种混合了一阶和二阶方法的算法。具体来说，它在迭代过程中结合了Gauss-Newton方法（一阶方法）和Levenberg方法（二阶方法）。

在每次迭代中，LM算法首先计算一阶导数（雅可比矩阵）和二阶导数（海森矩阵）的近似值。然后，根据这些近似值，通过求解一个修正的线性方程组来更新参数。修正的线性方程组结合了一阶和二阶信息，以平衡收敛速度和稳定性。

总的来说，LM算法在迭代过程中同时利用了一阶和二阶信息，以实现更快的收敛速度和更好的稳定性。因此，可以说LM算法是一种同时利用了一阶和二阶的优化算法。

