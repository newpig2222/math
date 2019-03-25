# (PART) 高数 {-}

# 极限 {#intro}

## 核心考点：

- 定义（4’）
- 性质（4‘）
- 计算（10’+4‘）
- 应用（4’）

说明：

 >1. 4'是小题的意思
 >2. 10'是大题的意思

## 极限的定义 {#liter}                         

### （一）、24种极限定义：

1. 原始定义：给出连续函数f(x)，$\lim_{x \to x_0}f(x)=A$ 等价于f(x)极限为A，转化为数学语言为：

$\forall$ $\xi$ >0, $\exists$ $\delta$ >0,当0<|x-$ x_0$|< $\delta$ ,|f(x)-A|< $\xi$  ,具体来说：

> 1. $\xi$  表示无论多小的正数，相当于衡量的尺度
> 2. 0<|x-$x_0$ |<$\delta$  表示以$x_0$ 为中心的去心领域，如下图：**其中$\delta$ 表示附近一个不大的正数。**![$x_0$](https://github.com/newpig2222/photo/raw/master/1609735006.jpg)
> 3. f(x）和A的距离要小于给出的任意尺度（即$\xi$ ）。

- 拓展极限定义：
  - 左极限：$\forall$ $\xi$ >0, $\exists$ $\delta$ >0,当0<$ x_0$-x< $\delta$ ,|f(x)-A|< $\xi$时，|f(x)-A|< $\xi$,即在$x_0$的左领域也成立极限
  
  - 右极限：$\forall \xi >0$, $\exists\delta >0$,当$0<x-{x_0}$ < $\delta$ ,|f(x)-A|< $\xi$时，|f(x)-A|< $\xi$ ,即在$x_0$的右领域叶成立。

1. $\lim_{x\to \infty}f(x)=A$ 转化为数学语言为：

$\forall \xi >0$, $\exists$X>0,当|x|>X时 ,|f(x)-A|< $\xi$ ，具体来说：

> 1. $\xi$  表示无论多小的正数，相当于衡量的尺度
> 2. |x|>X表示x向X和-X两个方向无限趋向无穷大，即这个$\exists$X>0表示远方，很大的正数。如图：
>
> ![X](https://github.com/newpig2222/photo/raw/master/3.jpg)

- 拓展定义：
  - 左极限：$\forall \xi$ ,$\exists X$,当x<-x时，|f(x)-A|<$\xi$。
  - 右极限：$\forall\xi$  ,$\exists$ X,当$x$>x时，|f(x)-A|<$\xi$ 。 

以上六个定义，为基本定义，即其极限是属于存在的数，这个数是唯一的。

------

1. $\lim_{x\to *}f(x)=\infty/+\infty/-\infty$ :

   > 1. $x\to *$的意思是包含六种情况：分别是$x\to x_0/{x_0}^+/{x_0}^-/\infty/-\infty/+\infty$
   > 2. $\infty/+\infty/-\infty$ 表示***特殊的不存在 的数***，一旦题目中给出了存在有界，即表明是指分割线前六种情况。

   具体的定义来说：

   - $\lim_{x \to *}f(x)=\infty$: $\forall$ M, (          ),     当(      ) 时，|f(x)|>M即无论给出的多大的M，f(x)到原点的距离总是大于M，其中两个括号为根据六种不同的情况填写（$x \to *$）
     - 左极限为: $\forall$ M, (        ),当（     ）时，f(x)<-M
     - 右极限为：$\forall$ M，（       ），当（    ）时，f(x)>M
   - 根据六种不同的情况填入两个括号，可得18种定义。

   1. 例题：

      - 例题1.证明若$x \to +\infty$及$x \to -\infty$时，函数f(x)的极限都存在且等于A，则$\lim _{x \to \infty}f(x)=A$

        > 【分析】本题实际上就是说左右极限均存在且相等，则总极限存在，因此我们应该从定义出发，通过定义展开条件，得出极限的定义条件。
        >
        > 【证明】$\lim _{x \to +\infty}f(x)=A$ 得出  $\forall \xi$,  $\exists$  X，当x >X时，f(x)-A<$ \xi$ 
        >
        > $\lim _{x \to  -\infty}f(x)$ =A 得出 $\forall \xi$, $ \exists$  X,当x<-X时，f(x)-A>- $\xi$ 
        >
        > 因此得出，$\forall \xi$  , $\exists $ X,当|x|>X时，|f(x)-A|< $\xi$,即$\lim_{x \to \infty}f(x)=A$

      - 例题2，证明函数f(x),当$x \to {x_0}$时，极限存在的必要条件是左右极限各自存在并相等。

        > 【分析】极限存在则可以推出左右极限存在且相等，该题则是反向证明。
        >
        > 【证明】$\lim_{x \to {x_0}^-}f(x)=A$，则推出$\forall \xi$ ,$\exists {\delta}_1$当 >0,当$0<x_0 -x< {\delta}_1$时，|f(x)-A|< $\xi$ ,
        >
        > $\lim_{x \to {x_0}^+}f(x)=A$ ，则推出$\forall \xi$   ,$\exists {\delta}_2$ >0,当0<x-$x_0 <{\delta}_2$ 时，|f(x)-A|< $\xi$ 。
        >
        > ***根据极限的定义*** ，取$\delta$ = min{${ \delta }_1$,${ \delta }_2$ },使得$|x-x_0|< \delta$ ,即得证。
        >
        > 如图：![分析图](https://github.com/newpig2222/photo/raw/master/12.jpg)

      - 例题3试给出$x \to \infty$ 时函数极限局部有限性的定理，并加以证明，若$\lim _{x \to \infty}f(x)$ 存在则存在X>0及M>0使得 $\forall  |x|>X均有|f(x)| \le M$。

        > 【分析】$\lim_{x \to *}f(x)=A  \Rightarrow$ 当 $x \to *$ 时 $|f(x)|  \le   M$。即f(x)距离原点不超过M，才是有界性。如图  
        >
        > ![有限性分析图](https://github.com/newpig2222/photo/raw/master/2019030701.jpg)
        >
        > 【证明】$\lim_{x \to \infty}f(x)=A \Rightarrow   \forall  \xi$ , $\exists X>0$ ,|x|>X时 ，$|f(x)-A| < \xi$ 。
        >
        > 已知 |f(x)-A|< $\xi$ ,目标为 |f(x)| $\le$ M
        >
        > ***根据中学数学重要不等式之一*** ：$|a \pm b| \le |a| +|b|$
        >
        > $|f(x)|=|f(x)+A-A| \le  |f(x)+A|+|A|$,由上得知，$|f(x)-A| < \xi$ ,故 $f(x) \le \xi   +|A|$，根据题意，$\xi >0$， |A| $\ge$  0。因 $\xi$ 为任意大于零的正数，故令 $\xi$ =2019,则 f(x) $\le$ 2019+|A|。因2019+|A|为一个确定的正数，故令M=2019+|A|，得证 f(x) $\le$ M。

   ### (二)数列极限：

   1. $\forall  \xi >0$， $\exists$ N>0, 当 n>N时，{$x_n$}收敛于A $\Leftrightarrow$  $\lim_{n \to \infty}{x_n}=A$ 。***注意：***

   数列{$x_n$} 决定了n必须是正的自然数，因此n只能趋向于$+\infty$ **即数列的极限是趋向于远方的**。

   **定义：** $\lim_{x \to \infty} {x_n}=A \Leftrightarrow \forall  \xi$ , $\exists$ N,当n>N时，$|x_n -A|< \xi$ 。

   1. 例题4 $\lim_{n \to \infty }{u_n}=a$ ,证明 $\lim_{n \to \infty}{|u_n|}=|a|$ ,并举例证明。如果数列{|$x_n$|} 有极限 但数列{$x_n$}未必有极限。

      > - 【分析】本题应从定义展开，然后利用中学重要不等式定理推导证明。
      >
      > 【证明】 $\lim_{n \to \infty}u_n=a \Leftrightarrow  \forall  \xi$  ,$\exists$ N,当 n>N，时 $|u_n-a| < \xi$ 。
      >
      > **根据中学重要不等式定理：**||a|-|b|| $\le$  |a-b| 这个定理实际上是a、b到原点距离和各自离原点距离的远近关系。如图：
      >
      > ![a、b与原点关系图](https://github.com/newpig2222/photo/raw/master/20190307002.jpg)
      >
      > **当a、b 位于原点的同侧时，等号成立！** 
      >
      > ![等号成立情况之一](https://github.com/newpig2222/photo/raw/master/20190307003.jpg)
      >
      > 
      >
      > 故可得，$|u_n -a |  \ge | | u_n  | -|a||$，已知$|u_n -a| <  \xi$ ，可得$||u_n|-|a||< \xi$ ,从而可得：$\lim_{n \to \infty }|u_n|$=a。
      >
      > ***注意利用中学关于重要不等式定理！,这些题目主要考察对定理的理解，往往由已知条件展开定理，然后利用中学重要不等式定理求证！*** 
      >
      > - 如数列${x_n}=(-1)^n$ 其值是在-1和1之间跳动，故无极限，而$|{x_n}|=|(-1)^n|$ 的值为常数1,而常数的极限即为本身，故其极限为1。

      例题5.对于数列{$x_n$}，若$x_{2k-1} \rightarrow a ( k \to \infty)$,$x_{2k}   \rightarrow  a( k \to \infty )$，证明$x_n \rightarrow a (n \to \infty)$ 。  

      > 
      >
      > 【分析】本题已知条件实际上是指数列的奇数项和偶数项均有相等的极限，求证整个数列有极限，**应从定义出发，进行条件构造。**
      >
      > 【证明】$x_{2k-1} \to a (k \to \infty)  \Rightarrow  \forall  \xi , \exists N_1$ ，当2k-1> $N_1$时，$|x_{2k-1}-a|< \xi$ 。（1）式
      >
      > $x_{2k } \to  a (k \to \infty )  \Rightarrow  \forall  \xi  , \exists N_2$ ，当2k>$N_2$时，$|x_{2k}-a|<  \xi$ 。（2）式。
      >
      > 根据图分析，取N=max{$N_1,N_2$}时，$\exists N >0$，当n>N时，$|x_n|-a<  \xi$ 即 $\lim_{n \to \infty  }{x_n}=a$。
      >
      > 如图：![**数列极限实际上就是比远方，故取两种情况的最远方即可满足条件，此题注意和例题2作比较**](https://github.com/newpig2222/photo/raw/master/20190307004.jpg)
      >
      > 
      >
      >  

   **本节主要是将24+1共25种定义掌握，能够推导即可** 
