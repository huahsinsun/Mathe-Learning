
***

Obsidian 作为 Markdown 编辑器无法原生支持完整的 Latex, 目前内置标准支持的是 MathJax^[一个 latex 的子集, 由 JavaScript 编写]

**& 符号的作用**：在 MathJax 中，`&` 符号用于创建对齐点，使公式在特定位置对齐，通常用于多行方程、方程组或带注释的方程推导。

要声明公式, 有两种方式:
* 行内公式使用 `$ $` 方法
* 行间 Block 公式使用 `$$....$$` 方法

$$
\begin{vmatrix}
a & b \\
c & d
\end{vmatrix} = ad-bc
$$
%%如果你希望加一点注释在源码里, 使用双百分号进行标注%%
***
快速学习

==符号&起到定位对齐的用法==

$ax^2+b_{1,2}=\frac{a-b}{a+b}$
$\alpha+\beta=\gamma$
$a^x_{y}$
$\leq,\neq,\geq$ ^[less qual]
$\rightarrow$

***
$\alpha, \beta, \gamma, \delta, \epsilon, \varepsilon, \zeta, \eta, \theta, \vartheta$
$\iota, \kappa, \lambda, \mu, \nu, \xi, \pi, \varpi, \rho, \varrho$
$\sigma, \varsigma, \tau, \upsilon, \phi, \varphi, \chi, \psi, \omega$

$\Gamma, \Delta, \Theta, \Lambda, \Xi, \Pi, \Sigma, \Upsilon, \Phi, \Psi, \Omega$

$(a+b)$ $[a+b]$ $\{a+b\}$ $\langle a+b \rangle$ $|a+b|$ $\|a+b\|$

$\left( \frac{a}{b} \right)$
$\left[ \frac{a}{b} \right]$
$\left\{ \frac{a}{b} \right\}$
$\left\langle \frac{a}{b} \right\rangle$
$\left| \frac{a}{b} \right|$

$\sum_{i=1}^{n} x_i$
$\prod_{i=1}^{n} x_i$
$\int_{a}^{b} f(x) dx$
$\oint_{C} f(z) dz$
$\lim_{x \to \infty} f(x)$

***
矩阵
$$
\begin{vmatrix}
a & b & c \\
d & e & f \\
g & h & i
\end{vmatrix}
$$

$$
\begin{matrix}
a & b & c \\
d & e & f \\
g & h & i
\end{matrix}
$$
$$
\left\{
\begin{matrix}
a & b & c \\
d & e & f \\
g & h & i
\end{matrix}
\right\}
$$
$$
\begin{pmatrix}
a & b & c \\
d & e & f \\
g & h & i
\end{pmatrix}
$$
$$
\begin{bmatrix}
a & b & c \\
d & e & f \\
g & h & i
\end{bmatrix}
$$
分段函数
$$f(x) = 
\begin{cases}
x^2, & \text{if } x > 0 \\
0, & \text{if } x = 0 \\
-x^2, & \text{if } x < 0
\end{cases}$$
$$f(x) = 
\begin{cases}
表达式_1, & 条件_1 \\
表达式_2, & 条件_2 \\
\vdots & \vdots \\
表达式_n, & 条件_n
\end{cases}$$
$$|x| = 
\begin{cases}
x, & \text{if } x \geq 0 \\
-x, & \text{if } x < 0
\end{cases}$$
$$\text{sgn}(x) = 
\begin{cases}
1, & \text{if } x > 0 \\
0, & \text{if } x = 0 \\
-1, & \text{if } x < 0
\end{cases}$$

方程组
**& 符号的作用**：在 MathJax 中，`&` 符号用于创建对齐点，使公式在特定位置对齐，通常用于多行方程、方程组或带注释的方程推导。
- 在等号前使用 `&`：使所有行的等号对齐
- 在变量前使用 `&`：使所有行的变量对齐
- 使用多个 `&`：创建多个对齐点（类似表格）
$$
x+2=5
$$
使用 align
$$
\begin{align}
x+2= & 5\\
y+5= &9\\
 k+9= &s
\end{align}
$$


$$\begin{align}
(x+1)^2 &= 9 & &\text{原方程} \\
x+1 &= \pm 3 & &\text{取平方根} \\
x &= -1 \pm 3 & &\text{移项} \\
x &= 2 \text{ 或 } x = -4 & &\text{得到结果}
\end{align}$$
使用大括号
$$\left\{
\begin{align}
3x + 2y &= 7 \\
2x - 5y &= -1
\end{align}
\right.$$

$$\left\{
\begin{array}{rcl}
3x + 2y &=& 7 \\
2x - 5y &=& -1
\end{array}
\right.$$
- `{rcl}` 就是告诉 MathJax 在每一列中应用右对齐、居中对齐和左对齐的规则。