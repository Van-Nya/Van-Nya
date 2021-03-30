---
title: 解析几何 - 第二章  
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

## 习题 2.1

### 1. 略.

### 2. 略.

### 3. 证：

设平面 $\pi$ 满足 $P_1, P_2, P_3 \in\pi$, 则 $\forall{P \left(x, y, z \right) ^ T \in\pi}$, 有  
$$\overrightarrow{PP1} \cdot \overrightarrow{PP_2} \times \overrightarrow{PP_3} = 0$$  

即  
$$\begin{vmatrix}
    x_1 - x & x_2 - x & x_3 - x \\
    y_1 - y & y_2 - y & y_3 - y \\
    z_1 - z & z_2 - z & z_3 - z
\end{vmatrix} = 0$$  

则易得  
$$\begin{vmatrix}
    x & x_1 - x & x_2 - x & x_3 - x \\
    y & y_1 - y & y_2 - y & y_3 - y \\
    z & z_1 - z & z_2 - z & z_3 - z \\
    1 & 0 & 0 & 0
\end{vmatrix} = - \begin{vmatrix}
    x_1 - x & x_2 - x & x_3 - x \\
    y_1 - y & y_2 - y & y_3 - y \\
    z_1 - z & z_2 - z & z_3 - z
\end{vmatrix} = 0$$  

通过初等变换得  
$$\begin{vmatrix}
    x & x_1 & x_2 & x_3 \\
    y & y_1 & y_2 & y_3 \\
    z & z_1 & z_2 & z_3 \\
    1 & 1 & 1 & 1
\end{vmatrix} = 0$$  

即为需证明的结论.  
$\square$  


### 4. 解：

设 $P_0 \left(x_0, y_0, z_0 \right) \in \pi$, 则  
$$\frac{x_0}{a} + \frac{y_0}{b} + \frac{z_0}{c} = 1$$  

令 $y_0 = z_0 = 0$, 解得 $x_0 = a$, 此时 $\overrightarrow{OP_0} = \left(a, 0, 0 \right) ^ T$, 同理易知 $a, b, c$ 为 $\pi$ 在三个坐标架上的截距.  


### 5. 略.

### 6. 略.

### 7. 证：

平面 (记为$\pi$) $Ax + By + Cz + D = 0$ 的法向量 $\boldsymbol{v_t} = \left(A, B, C\right) ^ T$, 设 $P_0 \left(x_0, y_0, z_0 \right)$, 则 $\forall P \left(x, y, z \right) ^ T \in\pi$, 有  
$$\boldsymbol{v_t} \cdot \overrightarrow{P_0P} = \left(A, B, C \right) ^ T \cdot \left(x - x_0, y - y_0, z - z_0 \right) ^ T = 0$$  

即  
$$A \left(x - x_0 \right) + B \left(y - y_0 \right) + C \left(z - z_0 \right) = 0$$  

即为需证明的结论.  
$\square$  


### 8. 略.

### 9. 证：

记三个平面分别为 $\pi_1, \pi_2, \pi_3$, 则 $\pi_1\cap\pi_2\cap\pi_3$ 可由下述线性方程组给出：  
$$\begin{bmatrix}
    a & b & c \\
    \alpha & \beta & \gamma \\
    \lambda a + \mu\alpha & \lambda b + \mu\beta & \lambda c + \mu\gamma
\end{bmatrix} \begin{bmatrix}
    x \\ y \\ z
\end{bmatrix} = \begin{bmatrix}
    - d \\ - \delta \\ - k
\end{bmatrix}$$  

记为  
$$\boldsymbol{A}\boldsymbol{v} = \boldsymbol{r}$$  

则方程组的增广矩阵为  
$$\boldsymbol{M} = \begin{bmatrix}
    a & b & c & - d \\
    \alpha & \beta & \gamma & - \delta \\
    \lambda a + \mu\alpha & \lambda b + \mu\beta & \lambda c + \mu\gamma & - k
\end{bmatrix} \xrightarrow{} \begin{bmatrix}
    a & b & c & - d \\
    \alpha & \beta & \gamma & - \delta \\
    0 & 0 & 0 & \lambda d + \mu\delta - k
\end{bmatrix}$$  

由线性方程组的性质易知, 若 $\lambda d + \mu\delta - k \ne 0$, 即 $k \ne \lambda d + \mu\delta$, 则方程组$\boldsymbol{A}\boldsymbol{v} = \boldsymbol{r}$无解, 则 $\pi_1\cap\pi_2\cap\pi_3 = \varnothing$, 原命题得证.  
$\square$  

### 10. 略.

### 11. 证：

由题意易知, $M_1, M_2$ 分别在平面 $\pi$ 两侧, 于是设 $\overrightarrow{OM} = \left(x_0, y_0, z_0 \right) ^ T$, 则  
$$\overrightarrow{M_1M} = \left(x_0 - x_1, y_0 - y_1, z_0 - z_1 \right) ^ T, \overrightarrow{MM_2} = \left(x_2 - x_0, y_2 - y_0, z_2 - z_0 \right) ^ T$$  

由 $\overrightarrow{M_1M} = k \overrightarrow{MM_2}$ 得线性方程组  
$$\begin{bmatrix}
    1 + k & 0 & 0 \\
    0 & 1 + k & 0 \\
    0 & 0 & 1 + k
\end{bmatrix} \begin{bmatrix}
    x_0 \\ y_0 \\ z_0
\end{bmatrix} = \begin{bmatrix}
    x_1 + kx_2 \\ y_1 + ky_2 \\ z_1 + kz_2
\end{bmatrix}$$

立即得出  
$$\left(x_0, y_0, z_0 \right) ^ T = \frac{1}{1 + k} \left(x_1 + kx_2, y_1 + ky_2, z_1 + kz_2 \right) ^ T = \frac{\overrightarrow{OM_1} + k \overrightarrow{OM_2}}{1 + k}$$

又因为 $M \in\pi$, 得 $Ax_0 + By_0 + Cz_0 + D =0$, 得  
$$\left(A, B, C \right) ^ T \cdot\left(x_0, y_0, z_0 \right) ^ T = - D$$  

即  
$$\left(A, B, C \right) ^ T \cdot\left(x_1 + kx_2, y_1 + ky_2, z_1 + kz_2 \right) ^ T = - \left(1 + k \right) D$$  

展开得  
$$k\left(Ax_2 + By_2 + Cz_2 + D \right) = - \left(Ax_1 + By_1 + Cz_1 + D \right)$$  

则  
$$k = - \frac{\left(Ax_1 + By_1 + Cz_1 + D \right)}{\left(Ax_2 + By_2 + Cz_2 + D \right)}$$  

则原命题得证.  
$\square$  


### 12. 解：

## 习题 2.2
