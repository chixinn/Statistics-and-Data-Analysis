# 充分统计量｜MSE｜有效估计｜渐近正态性｜Fisher信息量｜均匀分布的各种特殊性｜指数分布族

## 充分统计量与估计的充分性原则

1. 应用因子分解定理计算充分统计量的步骤：

$f(x_1,x_2,...,x_n)=g(t,\theta)h(x_1,x_2,...,x_n),T=T(x_1,x_2,...,x_n)$，这里$T=T(x_1,x_2,...,x_n)$是统计量的定义。

- 写出联合概率密度函数

- 把所有与$T(X),\theta$相关的因子都写出来

- 剩下的都只与$h(X)$有关

- 与已知样本的充分统计量T有一一对应关系的统计量

2. 充分统计量与Fisher信息量：

   设$T=T(X)$是样本的充分统计量，$g(t,\theta)$是统计量T的概率密度函数。那么$I_T(\theta)=I_x(\theta)$



## 均匀分布的各种特殊性

### 均匀分布的数理统计定义

$p(x;\theta_1,\theta_2)=\begin{cases}\frac{1}{\theta_2-\theta_1}&& \theta_1<x<\theta_2\\0&&Otherwised  \end{cases} $

$p(x;\theta_1,\theta_2)=\frac{1}{\theta_2-\theta_1}\Pi_i^n I(\theta_1<x<\theta_2)=\frac{1}{\theta_2-\theta_1}I(x_{(1)>\theta_1})I(x_{(n)<\theta_2})$



## Fisher信息量

1. 针对偏导求期望和方差，是针对x求的，而不是$\theta$
2. 求一个估计参数的函数的Fisher信息 ![[公式]](https://www.zhihu.com/equation?tex=I%28g%28%5Ctheta%29%29+%3D+I%28%5Ctheta%29+%28%5Cfrac%7Bd%5Ctheta%7D%7Bdg%28%5Ctheta%29%7D%29%5E2) 
3. 



## 指数分布族

[References](https://www.datalearner.com/blog/1051550130370543#:~:text=%E6%8C%87%E6%95%B0%E5%88%86%E5%B8%83%E6%97%8F%E6%98%AF%E4%B8%80,%E5%A4%9A%E9%A1%B9%E5%BC%8F%E5%88%86%E5%B8%83(multivariate)%E7%AD%89%E3%80%82&text=%E6%8C%87%E6%95%B0%E5%88%86%E5%B8%83%E6%97%8F%E4%B8%AD%E7%9A%84%E5%85%B1%E8%BD%AD%E7%BB%8F%E5%B8%B8%E7%94%A8%E4%BA%8E,%E7%94%A8%E4%BA%8E%E5%8F%98%E5%88%86%E6%8E%A8%E7%90%86%E3%80%82)

指数分布族是一系列分布的统称，包含连续和离散的相关分布。如，正态，泊松，二项指数Gamma和多项式分布等。
$$
p(X|\eta)=h(x)exp(\eta^TT(x)-A(\eta))
$$
$\eta$是可以是向量形式的自然参数，T(x)是充分统计量

## UMVUE

设总体的概率函数为$p(x;\theta)$，$x_1,x_2,...,x_n$为样本，$T=T(x_1,x_2,...,x_n)$是充分统计量，那么对于$\theta$的任一无偏估计$\hat{\theta}$， ![[公式]](https://www.zhihu.com/equation?tex=\tilde+\theta+%3D+E(\hat+\theta+|+T))

对比这个新的估计，偏差保持不变，方差只小不大。

