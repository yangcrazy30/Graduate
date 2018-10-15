# 第一讲 函数极限与连续

## 函数的概念与性质

1. $$y=f(x)$$  
   判断两个函数为同一函数
   1. 定义域
   2. 对应法则

2. 函数性质
   * 奇偶性：
   $$ 偶函数f(-x)=f(x)$$
   $$ 奇函数f(-x)=-f(x)$$
   >$$D_f(-t,t)$$
   >$$F(x)=f(x)+f(-x)偶$$
   >$$F(x)=f(x)*f(-x)奇$$
   * 周期性
   * 有界性
   * 单调性

## 函数的构成方式及类型

* 基本初等函数
  初等函数必连续。由基本初等函数经四则运算构成。
  包括：
  * 幂函数
  * 指数函数
  * 反三角函数
  * 对数函数
  * 三角函数
  >$$y=x^x幂指函数不是基本初等函数$$
* 分段函数
  * 绝对值函数
  * 取整函数
    $$y=[x]$$
    >$$\lim_{x \to 0}[x] 不存在$$
    >$$x-1<[x]\leqslant x$$
    >方法:站在该点向数轴左侧看
* 复合函数
* 符号函数
  $$
  sgn(x) =
        \begin{cases}
        -1,  & \text{ $x<0$ } \\
        0, & \text{ $x=0$ } \\
        1.& \text{ $x>0$ }
        \end{cases}
  $$
* 比较函数
* 反函数
  反函数导数为原函数导数的倒数
* 隐函数
  $$由方程F(x,y)=0确定的函数$$

## 函数极限的概念

* 邻域
  $$U(x_0,\varepsilon):0<|x-x_0|<\varepsilon$$
* 函数极限的表示

$$\lim{x \to x_0}f(x)=A\Leftrightarrow \forall\xi>0 \exists \varepsilon>0 $$
有
$$  0<|x-x_0|<\varepsilon 使 |f(x)-A|<\xi$$
>左极限：左邻域对应的极限
>右极限：右领域对应的极限

**极限存在：左极限等于右极限**

exp1、exp2、exp3

## 函数极限的性质

* 唯一性
  极限存在必唯一，不唯一不存在。

  * 无穷大与不确定值都叫不存在
  * 极限为无穷大说明左右极限都为无穷大
  
* 有界性
  若
  $$\lim_{x \to a}f(x)=A>0$$
  $$\exists M>0 使 f(x)\leqslant M$$

* 保号性
  若
  $$\lim_{x \to a}f(x)=A>0$$
  则在该点邻域内函数值大于0
  * 推论：
  $$若 x \to a ,f(x)>0 则 \lim_{x \to a}f(x)\geqslant A$$

  exp4

## 函数极限的计算规则

前提：打开的极限都存在
$$\lim_{x \to a}[f(x)\pm g(x)]=\lim_{x \to a}f(x) \pm \lim_{x \to a}g(x)$$
$$\lim_{x \to a}[f(x)*g(x)]=\lim_{x \to a}f(x)*\lim_{x \to a}g(x)$$
$$\lim_{x \to a}[\frac{f(x)}{g(x)}]=\frac{\lim_{x \to a}f(x)}{\lim_{x \to a}g(x)}$$

exp5、exp6

## 两个重要极限

## 无穷小，无穷大定义及性质

* 无穷小
  如果在某种趋势下
  $$\lim_{x \to a}f(x)=0$$
  则称f(x)为x趋向于a的无穷小
* 无穷大
  .........
   $$\lim_{x \to a}f(x)=\infty$$
  .........的无穷大
>1. 无穷小不一定是0，但是0一定是无穷小，0是最高阶无穷小
>2. 无穷小必局部有界
>3. 无穷大必局部有界
>4. 局部有界不一定是无穷大
>$$exp \lim_{x \to \infty}xsin(x)无界振荡$$

* 无穷小运算:不可推广大无穷大
  * 有限个无穷小和为无穷小
  * 有限个无穷小积为无穷小
  * 无穷小*有界函数=无穷小
  * 有限个无穷大的积为无穷大

* 无穷小的比较
  比的是阶数(趋向于0的速度)
  $$
  \lim_{x \to a} \frac{\alpha}{\beta} =
        \begin{cases}
        0,  & \text{alpha 是 beta 高阶无穷小} \\
        \infty, & \text{alpha 是 beta 低阶无穷小} \\
        c,  & \text{ 同阶 } \\
        1,  & \text{ 等价无穷小 }
        \end{cases}
  $$

  exp7,exp8

  >关于等价无穷小
  >$$\alpha \sim \beta \Leftrightarrow \alpha=\beta+o(\beta)$$

  exp9,exp10

  常见等价无穷小:
  
  $$x \to 0$$
  $$sin(x) \sim x$$
  $$arcsin(x)\sim x$$
  $$tan(x) \sim x$$
  $$arctan(x) \sim x$$
  $$ln(1+x) \sim x $$
  $$e^x-1 \sim  x$$
  $$a^x-1 \sim xlna$$
  $$1-cos(x) \sim \frac{x^2}{2}$$
  $$x-sin(x) \sim \frac{x^3}{6}$$
  $$x-arcsin(x) \sim \frac{-x^3}{6}$$
  $$x-ln(x+1) \sim \frac{x^2}{2}$$
  $$(1+x)^a-1 \sim ax$$
  $$x^2-sin(x)^2 \sim \frac{x^4}{3}$$
  $$x \to 1$$
  $$lnx \sim x-1$$

* 关于高阶无穷小的运算规则
   $$O(x^m)+O(x^n)=O(x^c) c=min(m,n)$$
   $$O(x^m)*O(x^n)=O(x^{m+n})$$
   $$x^m*O(x^n)=O(x^{m+n})$$
   $$O(x^m)=O(kx^m)=kO(x^m)(k\not=0)$$
* 洛必达
  若
  $$ 若\lim_{x \to a} \frac{f(x)'}{g(x)'}=A$$
  $$ 则\lim_{x \to a} \frac{f(x)}{g(x)}=A$$

>振荡不可用洛必达法则
>$$如 \lim_{x \to \infty} \frac{x-sin(x)}{x}$$
>由求导的极限推原函数极限，不能由原函数极限推出求导后的极限

## 专题 关于未定式函数极限的计算

过程：定类型->简形式->用工具

$$
求极限 = \begin{cases}
   \frac{0}{0} ,\frac{\infty}{\infty} &\text{ } b \\
   0*\infty &\text{ } b \\
   \infty-\infty &\text{ } b \\
   1^{\infty},0^0,\infty^0 &\text{ } b \\
\end{cases}
$$

* 函数极限计算、应用的综合问题

  1. 关于泰勒公式在函数极限求解中的应用
   $$sin(x)=x-\frac{x^3}{6}+o(x^3)$$
   $$tan(x)=x+\frac{x^3}{3}+o(x^3)$$
   $$cos(x)=1-\frac{x^2}{2}+o(x^3)$$
   $$e^x=1+x+\frac{x^2}{2}+o(x^2)$$
   $$(1+x)^a=1+ax+\frac{a(a-1)x^2}{2}+o(x^2)$$
   $$acrsin(x)=x+\frac{x^3}{6}+o(x^3)$$
   $$arctan(x)=x-\frac{x^3}{3}+o(x^3)$$
   $$ln(1+x)=x-\frac{x^2}{2}+o(x^2)$$




## 数列极限的概念，性质和定理

1. 数列极限的定义
   $$\lim_{x \to \infty}X_n=A \Leftrightarrow $$
   $$\forall \varepsilon >0 \exists N>0 when, n>N 恒有|X_n-A|<\varepsilon$$
2. 数列极限与列极限的关系
   $$\lim_{x \to \infty}X_n=A \Leftrightarrow 任何一个子列均收于A$$
3. 收敛数列的性质
   * 唯一性：收敛必唯一
   * 有界性：收敛数列必有界，指整体有界，有界不一定收敛
   * 保号性
  $$\lim_{x \to \infty}X_n=A \Leftrightarrow \exists N>0当n>N时X_n>0$$
4. 数列极限运算规则（同函数极限）

5. 数列极限的存在准则
   * 夹逼定理
   * 单调有界原则：若{xn}满足单调递增有上界或单调递减有下界则{xn}满足收敛（先证明极限存在再求极限）单调有界准则证数列极限是否存在

## 函数的连续与间断

1. 定义
   $$若f(x)在x_0处连续 \Leftrightarrow$$
   $$\lim_{x \to x_0}f(x)=f(x_0)$$
   >左连续
   >$$\lim_{x \to x_0^-}f(x)=f(x0)$$
   >右连续
   >$$\lim_{x \to x_0^+}f(x)=f(x0)$$
2. 函数在区间上连续
   $$f(x)在(a,b)上连续 \Leftrightarrow 在(a,b)上每点都连续$$
   $$f(x)在(a,b)上连续 \Leftrightarrow 在(a,b)上每点都连续且点a右连续，点b左连续$$
3. 间断点的定义与分类
   $$A: \lim_{x \to x_0^+}$$
   $$B: \lim_{x \to x_0^-}$$
   $$C:f(x)$$
   第一类间断点：
   若A，B均存在，但A不等于B，为跳跃间断点
   若A，B均存在，但A等于B不等于C，为可去间断点
   第二类间断点：
   若A，B至少有一个不存在，且为无穷大，为无穷间断点
   若A，B至少有一个不存在，且为振荡不存在，为振荡间断点
   >关于间断点的问题一般涉及以下两类
   >1.初等函数：无定义点（一定是间断点因为无定于）
   >2.分段函数：无定义点，分段处

## 闭区间连续的性质

1. （有界定理）若f(x)在[a,b]上连续，必在[a,b]上有界
2. （最值定理）设f(x)在[a,b]上连续，则f(x)在[a,b]上必有最大值和最小值
3. （介值定理）若f(x)在[a,b]上连续，且最大值和最小值分别为M和m，则对于任意u介于m和M之间，至少存在e属于[a,b]使f(e)=u;
4. (零点定理)若函数闭区间连续，且两端点异号，至少存在u使f(u)=0

>关于‘有界定理’的推广与说明
>若f(x)在(a,b)连续且a的右极限，b的左极限存在。则f(x)在[a,b]有界

>关于‘零点定理’的说明
>方程f(x),g(x)在(a,b)至少存在一个实根，则存在u属于(a,b)使f(u)=g(u)，即F(x)=g)(x)*f(x)在(a,b)至少有一个零点
