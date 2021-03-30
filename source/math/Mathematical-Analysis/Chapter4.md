---
title: 数学分析 - 第四章  
type: math  
comments: false  
top_img: false  
mathjax: true  
katex: true  
aside: true  
aplayer: false  
permalink:  
---

qwq

********

## 习题4.1

### 1. 略.

### 2. 略.

### 3. 解:

#### (1)

由题意易知 $f \left(x \right)$ 在 $\mathbb{R}\backslash \left\{2 \right\}$ 上有定义, 且  
$$\begin{aligned}
    & \lim\limits_{x \rightarrow 2} f \left(x \right)
    = \lim\limits_{x \rightarrow 2} \frac{x ^ 3 - 8}{x - 2}
    = \lim\limits_{x \rightarrow 2} \frac{\left(x - 2 \right)\left(x ^ 2 + 2x + 4 \right)}{x - 2} \\
    \\
    & = \lim\limits_{x \rightarrow 2} \left(x ^ 2 + 2x + 4 \right)
    = 2 ^ 2 + 2 \times 2 + 4
    = 12
\end{aligned}$$  

为使 $f \left(x \right)$ 在 $\mathbb{R}$ 上连续, 可令 $f \left(2 \right) = 12$, 则  
$$f \left(x \right) = \begin{cases}
    \frac{x ^ 3 - 8}{x - 2}, x \ne 2 \\
    \\
    12, x = 2
\end{cases} = x ^ 2 + 2x + 4$$


#### (2)

由题意易知 $f \left(x \right)$ 在 $\mathbb{R}\backslash \left\{0 \right\}$ 上有定义, 且  
$$\begin{aligned}
    & \lim\limits_{x \rightarrow 0} f \left(x \right) = \lim\limits_{x \rightarrow 0} \frac{1 - \cos x}{x ^ 2} = \lim\limits_{x \rightarrow 0} \frac{2 \sin ^ 2 \frac{x}{2}}{x ^ 2} = \frac{1}{2}
\end{aligned}$$  

为使 $f \left(x \right)$ 在 $\mathbb{R}$ 上连续, 可令 $f \left(0 \right) = \frac{1}{2}$, 则  
$$f \left(x \right) = \begin{cases}
    \frac{1 - \cos x}{x ^ 2}, x \ne 0 \\
    \frac{1}{2}, x = 0
\end{cases}$$


#### (3)

由题意易知 $f \left(x \right)$ 在 $\mathbb{R}\backslash \left\{0 \right\}$ 上有定义, 且  
$$\lim\limits_{x \rightarrow 0} f \left(x \right) = \lim\limits_{x \rightarrow 0} x \cos\frac{1}{x} = 0$$  

为使 $f \left(x \right)$ 在 $\mathbb{R}$ 上连续, 可令 $f \left(0 \right) = 0$, 则  
$$f \left(x \right) = \begin{cases}
    x \cos\frac{1}{x}, x \ne 0 \\
    0, x = 0
\end{cases}$$  


### 4. 证: 

若 $f$ 在点 $x_0$ 处连续, 则 $\forall\varepsilon\gt 0, \exist{\mathring{U}\left(x_0 \right)}, s.t. \forall x \in \mathring{U}\left(x_0 \right), \left|f \left(x \right) - f \left(x_0 \right) \right| \le\varepsilon$, 则 $\left| \left| f \left(x \right) \right| - \left| f \left(x_0 \right) \right| \right| \le \left|f \left(x \right) - f \left(x_0 \right) \right| \le\varepsilon, \left| f^2 \left(x \right) - f^2 \left(x_0 \right) \right| = \left| f \left(x \right) + \left(x_0 \right) \right| \cdot \left| f \left(x \right) - \left(x_0 \right) \right| \le \left| f \left(x \right) + \left(x_0 \right) \right| \cdot \varepsilon$, 由此得 $\left| f \right|$ 和 $f^2$ 也在 $x_0$ 处连续.  
$\square$  

令 $f \left(x \right) = \left| f \left(x \right) \right| \cdot \left[2D \left(x \right) - 1 \right] = \sqrt{f^2 \left(x \right)} \cdot \left[2D \left(x \right) - 1 \right]$, 其中 $D \left(x \right)$ 是狄利克雷函数, 则可说明 $\left| f \right|$ 或 $f^2$ 在 $I$ 上连续不能推出 $f$ 在 $I$ 上连续.  


### 5. 证:

设 $f$ 与 $g$ 都在 $x = 0$ 处连续, 则由函数连续性、极限唯一性和保不等式性得  
$$f \left(0 \right) = \lim\limits_{x \rightarrow 0} f \left(x \right) = \lim\limits_{x \rightarrow 0} g \left(x \right) = g \left(0 \right)$$  

这与 $f \left(0 \right) \ne g \left(0 \right)$ 矛盾, 故 $f$ 与 $g$ 之中至多有一个在 $x = 0$ 处连续.  
$\square$  


### 6. 证:

设 $f$ 在 $\mathring{U}\left(x_0, \delta\right)\bigcup\left\{x_0 - \delta, x_0 + \delta\right\}$ 有定义, 则根据 $f \left(x \right)$ 的单调性可知, $\forall{x_1 \in \mathring{U}_- \left(x_0, \delta\right), x_2 \in \mathring{U}_+ \left(x_0, \delta\right)}, f \left(x_0 - \delta\right) \le f \left(x_1 \right) \le f \left(x_2 \right) \le f \left(x_0 + \delta\right)$, 则 $f \left(x_0 - \delta\right) \le \lim\limits_{x \rightarrow x_0^-} f \left(x \right) \le \lim\limits_{x \rightarrow x_0^+} f \left(x \right) \le f \left(x_0 + \delta\right)$, 则 $x_0$ 必是 $f$ 的第一类间断点.  
$\square$  


### 7. 证:

设 $f$ 定义在 $I = D \backslash \bigcup\left\{x_i \right\}, i = 1, 2, \cdots, n$, 其中 $I$ 是分别以 $x^-, x^+$ 为左右端点的区间 , 则根据 $f$ 的分段连续性, 有 $\forall{x \in I}, g \left(x \right)=\lim\limits_{y \rightarrow x} f \left(y \right) = f \left(x \right)$, 而 $\forall x_i, g \left(x_i \right)$

********

## 习题 4.2

### 1. 略.

### 2. 证:

#### (1)

由连续性和大小关系可知  
$$\lim\limits_{x \rightarrow x_0} f \left(x \right) = f \left(x_0 \right) \lt g \left(x_0 \right) = \lim\limits_{x \rightarrow x_0} g \left(x \right)$$  

则由连续函数的局部的保序性可知题设成立.  
$\square$  


#### (2) 略.

### 3. 证:

由题意, 易知  
$$\begin{aligned}
    F \left(x \right) = \dfrac{f \left(x \right) + g \left(x \right)}{2} + \left|\dfrac{f \left(x \right) - g \left(x \right)}{2} \right| \\
    \\
    G \left(x \right) = \dfrac{f \left(x \right) + g \left(x \right)}{2} - \left|\dfrac{f \left(x \right) - g \left(x \right)}{2} \right|
\end{aligned}$$  

根据连续函数的四则运算及复合运算规则, 结论显然成立.  
$\square$  


### 4. 证:

由上一题易得  
$$\begin{aligned}
    F \left(x \right) & = \dfrac{-c + \min\left\{c, f \left(x \right) \right\}}{2} + \left|\dfrac{c + \min\left\{c, f \left(x \right) \right\}}{2} \right| \\
    \\
    & = \dfrac{-c + \dfrac{c + f \left(x \right)}{2} - \left|\dfrac{c - f \left(x \right)}{2} \right|}{2} + \left|\dfrac{c + \dfrac{c + f \left(x \right)}{2} - \left|\dfrac{c - f \left(x \right)}{2} \right|}{2} \right|
\end{aligned}$$  

由上题结论, $F \left(x \right)$ 显然在 $\mathbb{R}$ 上连续.  
$\square$  


### 5. 略.

### 6. 略.

### 7. 能.

### 8. 解:

#### (1)

$$\begin{aligned}
    & \lim\limits_{x \rightarrow \frac{\pi}{4}} \left(\pi - x \right)\tan{x} \\
    \\
    = & \left(\pi - \frac{\pi}{4} \right) \tan{\frac{\pi}{4}} \\
    \\
    = & \frac{3 \pi}{4}
\end{aligned}$$  


#### (2)

$$\begin{aligned}
    & \lim\limits_{x \rightarrow 1^+} \frac{x \sqrt{1 + 2x} - \sqrt{x^2 - 1}}{x + 1} \\
    \\
    = & \frac{1 \cdot \sqrt{1 + 2 \cdot 1} - \sqrt{1^2 - 1}}{1 + 1} \\
    \\
    = & \frac{\sqrt{3}}{2}
\end{aligned}$$  


### 9. 证:

(依靠介值定理)


### 10. 证:

(两侧无穷极限和介值定理)


### 11. 证:

记 $f_1 = f, f_2 = g$, 由题意可知$\forall \varepsilon \gt 0, \exist \delta_1, \delta_2 \gt 0, s.t. \forall x_1, x_2 \in I$, 若 $\left|x_1 - x_2 \right| \le \delta_i$, 则 $\left|f_i \left(x_1 \right) - f_i \left(x_2 \right) \right| \le \varepsilon \left(i = 1, 2\right)$; 令 $\delta = \min\left\{\delta_1 + \delta_2 \right\}$, 则 $\forall x_1, x_2 \in I$, 若 $\left|x_1 - x_2 \right| \le \delta$, 则 $\left|\left[f_1 \left(x_1 \right) + f_2 \left(x_1 \right) \right] - \left[f_1 \left(x_2 \right) + f_2 \left(x_2 \right) \right] \right| \le \left|f_1 \left(x_1 \right) - f_1 \left(x_2 \right) \right| + \left|f_2 \left(x_1 \right) - f_2 \left(x_2 \right) \right| \le 2 \varepsilon$  

则 $f + g = f_1 + f_2$ 也在 $I$ 上一致收敛.  
$\square$
