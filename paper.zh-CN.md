
# 两个交换映射生成的极小作用可以没有半开的非恒等元

**2026 年 11 月 20 日** · [英文 PDF](semiopen-actions.pdf) · [LaTeX 源码](semiopen-actions.tex)

## 摘要

本文构造紧致、连通、可度量空间上的一个极小 $\mathbb{N}_0^2$ 作用。对每个非零元素 $(m,n)$，相应的连续满射都把某个非空开集映满同一个闭的无处稠密集。

这个系统是另一个极小系统的因子，后者的所有作用映射都是开映射。

构造回答了 Blahodatna、Detmold、Glasscock 和 Le 关于交换半群的问题，并对 Dai、Feng、Lv 和 Xie 关于极小半流因子映射的问题给出可度量情形的否定答案。

---

## 1. 问题与主定理

连续映射 $f:X\to Y$ 称为**半开**，如果每个非空开集 $U\subseteq X$ 都满足

$$
\mathrm{Int}_Y f(U)\neq\varnothing.
$$

离散半群 $S$ 在 $X$ 上的连续作用称为**极小**，如果对每个 $x\in X$ 都有

$$
\overline{Sx}=X.
$$

两个 $S$ 系统之间的因子映射是与作用交换的连续满射。

单个连续自映射若在紧致 Hausdorff 空间上生成极小系统，则它是半开的，见 Kolyada、Snoha 和 Trofimchuk 的定理 2.4(1) [5]。

由半开映射对复合的封闭性，它的每个迭代也都半开。

对于多个生成元，Blahodatna 等人在文献 [2] 第 1.2 节脚注 1 中给出了非交换的反例，并问交换半群能否出现这种现象。

### 定理 1

存在紧致、连通、可度量空间 $X$，两个交换的连续满射

$$
s,r:X\to X,
$$

以及闭的无处稠密集 $D\subset X$，使得

$$
(m,n)\cdot x=s^m r^n x
$$

定义一个极小的 $\mathbb{N}\_0^2$ 作用，并且对每个 $m+n>0$ 都存在非空开集 $U\_{m,n}\subset X$满足

$$
\boxed{s^m r^n(U_{m,n})=D.}
$$

Akin、Auslander 和 Nagar 在文献 [1] 的例 2.30 中用单侧移位和在一段区间上取常值的坐标映射构造了非半开映射。

他们例中的移位和逐坐标映射都保持常值序列集，因而无法在整个序列空间上生成极小作用。

下面先在一条完整纤维上实现稠密平移，再取一个只保留首坐标部分信息的因子。

---

## 2. 由开映射生成的极小作用

记

$$
\mathbb{T}=\mathbb{R}/\mathbb{Z},
\qquad
\mathbb{N}_0=\{0,1,\ldots\},
\qquad
\mathbb{N}=\{1,2,\ldots\}.
$$

所有乘积空间均取积拓扑。

令

$$
c(t)=\cos(2\pi t).
$$

选择无理数 $\alpha\bmod 1$，使得

$$
1,\ c(\alpha),\ c(2\alpha),\ c(3\alpha),\ldots
$$

在 $\mathbb{Q}$ 上线性无关。

这样的选择存在。

每个非平凡有限整数关系都要求三角多项式

$$
a_0+\sum_{j=1}^{k}a_j\cos(2\pi jt)
$$

为零。

由其傅里叶系数可知该多项式不恒为零。

令 $z=e^{2\pi it}$，乘以 $z^k$ 后得到关于 $z$ 的非零多项式，故它在圆周上只有有限个零点。

所有可能的有限整数关系可数，排除这些零点及有理点即可。

设

$$
K=\mathbb{T}^{\mathbb{N}_0},
\qquad
Z=\mathbb{T}\times K.
$$

对 $x=(x_j)_{j\ge 0}$ 定义

$$
\begin{aligned}
A(t,x)
&=
\bigl(t+\alpha,(x_{j+1})_{j\ge 0}\bigr),\\[6pt]
H(t,x)
&=
\bigl(t,(x_j+c(t+j\alpha))_{j\ge 0}\bigr),\\[6pt]
B&=HA.
\end{aligned}
$$

圆周坐标的加法均按模 $1$ 计算。

$AH$ 和 $HA$ 的第 $j$ 个序列坐标都是

$$
x_{j+1}+c(t+(j+1)\alpha),
$$

底坐标也相同，故 $A,B$ 交换。

单侧移位是满射，并把基本开柱集映成开柱集，因此 $A$ 是开满射。

$H$ 的逆映射在每个坐标上减去对应的增量，故 $H$ 是同胚，$B$ 也是开满射。

### 引理 2

$A$ 和 $B$ 在 $Z$ 上生成的正向作用极小。

**证明。**

任意非空闭的正向不变集都包含一个按包含关系极小的非空闭正向不变子集 $M$。

这是因为任一降链由紧性具有非空交，可以应用佐恩引理。

由于 $A,B$ 交换，$A(M)$ 和 $B(M)$ 都是 $M$ 内的非空紧致正向不变集。

由极小性得到

$$
A(M)=M=B(M).
$$

从而

$$
H(M)=H(A(M))=B(M)=M.
$$

$M$ 在底圆周上的投影是无理旋转下的非空闭正向不变集，故等于整个圆周。

特别地，$M$ 与底点为 $\alpha$ 的纤维相交。

在这条纤维上，$H$ 按向量

$$
\bigl(c((j+1)\alpha)\bigr)_{j\ge 0}
$$

平移。

由 $\alpha$ 的选择和 Kronecker 定理 [4，定理 2.39]，这条纤维内每个点的正向轨道投影到任意有限初始坐标块后都稠密。

有限坐标块决定积拓扑，故轨道稠密于整条纤维。

$M$ 是闭的且 $H(M)=M$，于是

$$
\{\alpha\}\times K\subseteq M.
$$

单侧移位满射，所以 $A$ 把每条完整纤维映满下一条。

于是对每个 $k\ge 1$，都有

$$
\{k\alpha\}\times K\subseteq M.
$$

这些纤维的并在 $Z$ 中稠密，所以

$$
M=Z.
$$

把这个论证用于任意点的正向轨道闭包，就得到联合极小性。$\square$

---

## 3. 使非零元素失去半开性的因子

定义连续满射

$$
p:\mathbb{T}\to[0,1]
$$

为

$$
p(v)=\max\{0,c(v)\}.
$$

它在开弧

$$
J=(1/4,3/4)\subset\mathbb{T}
$$

上恒为零。

令

$$
X=\mathbb{T}\times[0,1]\times\mathbb{T}^{\mathbb{N}},
$$

并定义

$$
q(t,x_0,x_1,\ldots)
=
(t,p(x_0),x_1,x_2,\ldots).
$$

可数积 $X$ 紧致、可度量且道路连通。

$A$ 和 $B$ 都丢弃旧坐标 $x_0$，所以 $qA$ 和 $qB$ 在 $q$ 的每条纤维上各自为常值。

$q$ 是紧空间到 Hausdorff 空间的连续满射，因而是商映射。

由此得到连续映射

$$
s,r:X\to X
$$

满足

$$
sq=qA,
\qquad
rq=qB.
$$

由满射性和 $AB=BA$ 可知 $s,r$ 也是交换的满射。

由引理 2，$Z$ 中每条联合轨道稠密，其在 $q$ 下的像在 $X$ 中稠密，故 $s,r$ 的联合正向作用极小。

### 定理 1 的证明

第一个生成元可写成

$$
s(t,u,x_1,x_2,\ldots)
=
(t+\alpha,p(x_1),x_2,x_3,\ldots).
$$

所以它把开柱集 $x_1\in J$ 映满

$$
D=\mathbb{T}\times\{0\}\times\mathbb{T}^{\mathbb{N}}.
$$

下面说明同一个 $D$ 适用于所有非零元素。

固定

$$
d=m+n>0.
$$

在 $Z$ 上有

$$
A^mB^n=H^nA^d.
$$

在 $X$ 上，$s^mr^n$ 的底坐标为

$$
t+d\alpha,
$$

区间坐标为

$$
p(x_d+n c(t+d\alpha)),
$$

第 $j$ 个尾坐标为

$$
x_{d+j}+n c(t+(d+j)\alpha),
\qquad j\ge 1.
$$

因此，下列开集的像包含于 $D$：

$$
U_{m,n}
=
\left\{
(t,u,x_1,\ldots)\in X
\;\middle|\;
x_d+n c(t+d\alpha)\in J
\right\}.
$$

给定 $D$ 中任一点

$$
(t',0,y_1,y_2,\ldots),
$$

取

$$
t=t'-d\alpha,
$$

选择 $x_d$ 使

$$
x_d+n c(t')\in J,
$$

并对每个 $j\ge 1$ 取

$$
x_{d+j}=y_j-n c(t'+j\alpha).
$$

其余输入坐标任取，就得到了该点在 $U_{m,n}$ 中的原像。

这同时证明了 $U_{m,n}$ 非空且像恰为 $D$：

$$
\boxed{s^mr^n(U_{m,n})=D.}
$$

由于 $\{0\}$ 在 $[0,1]$ 中闭且内部为空，$D$ 在 $X$ 中闭且无处稠密。$\square$

---

## 4. 两个推论

### 推论 3

紧致度量极小 $\mathbb{N}_0^2$ 系统之间的连续等变满射可以失去半开性，即使该映射是系统的自映射。

**证明。**

取

$$
\pi=s:X\to X.
$$

因为 $s,r$ 交换，$\pi$ 与整个作用交换。

$\pi$ 满射，而定理 1 中 $(m,n)=(1,0)$ 时的开集说明它不半开。$\square$

这回答了文献 [3] 问题 5.2.4 的可度量分支。

该文定理 3.2 的正面结果含有逐纤维满射（fiber-onto）假设，要求每个作用元素 $g$ 和每个 $y$ 满足

$$
g(\pi^{-1}(y))=\pi^{-1}(gy).
$$

在本例中取 $g=\pi=s$，左边等于 $\{y\}$，右边却包含将 $y$ 的区间坐标任意改变而得到的所有点。

### 推论 4

存在所有作用映射都开的紧致度量极小交换半群作用，其因子中的每个非恒等作用映射都不半开。

**证明。**

$Z$ 上的每个作用映射 $A^mB^n$ 都是开映射的复合。

$q$ 将其诱导为 $X$ 上的 $s^mr^n$，结论由定理 1 得到。$\square$

---

## 形成说明

本文反例及初步证明由 OpenAI 的 ChatGPT 在回应所提研究问题时生成。ChatGPT 也参与了稿件整理。

---

## 参考文献

1. E. Akin, J. Auslander, A. Nagar. *Variations on the concept of topological transitivity*. Studia Mathematica **235** (2016), 225–249. [DOI](https://doi.org/10.4064/sm8553-7-2016)

2. A. Blahodatna, L. Detmold, D. Glasscock, A. N. Le. *The regionally proximal relation for commutative semigroup actions*. 2026. [arXiv:2610.10397v1](https://arxiv.org/abs/2610.10397v1)

3. X. Dai, L. Feng, C. Lv, Y. Xie. *On semi-openness of fiber-onto extensions of minimal semiflows and quasi-separable maps*. 2026. [arXiv:2601.03380v2](https://arxiv.org/abs/2601.03380v2)

4. T. Eisner, B. Farkas, M. Haase, R. Nagel. *Operator Theoretic Aspects of Ergodic Theory*. Graduate Texts in Mathematics **272**, Springer, 2015. [DOI](https://doi.org/10.1007/978-3-319-16898-2)

5. S. Kolyada, Ľ. Snoha, S. Trofimchuk. *Noninvertible minimal maps*. Fundamenta Mathematicae **168** (2001), 141–163. [DOI](https://doi.org/10.4064/fm168-2-5)
