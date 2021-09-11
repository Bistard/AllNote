# LaTeX Techniques

## others

```latex
\usepackage{amsthm}
```

## Proof

```latex
\begin{proof}
\end{proof}
```

## Equations

$$
\begin{align*}
    a &= 1 + 2 + 3 + 4 \\
      &= 3 + 7 \\
      &= 10
\end{align*}
$$


$$
\begin{align}
    a &= 1 + 2 + 3 + 4 \\
        &= 3 + 7 \\
        &= 10
\end{align}
$$


$$
\begin{align}
    a &= 1 + 2 + 3 + 4 \\
        &= 3 + 7 \tag*{this is a comment} \\
        &= 10
\end{align}
$$


$$
\begin{align}
    a &= 1 + 2 + 3 + 4 \\
        &= 3 + 7 \tag{this is a comment} \\
        &= 10
\end{align}
$$

## Symbols



$$
\infty \text{ } \mathbb R \text{ } \mathbb R^n \text{ } \mathbb N \text{ } \mathbb Z \text{ } \mathbb Q \text{ } \mu \text{ } \theta \text{ } \alpha \text{ } \beta \text{ } \gamma \text{ } \lambda
$$

$$
\emptyset \text{ } \varnothing
$$


$$
\cup \text{ } \cap \text{ } \leq \text{ } \geq \text{ } > \text{ } < \text{ } \neq \text{ } \doteq \text{ } \equiv \text{ } \approx \text{ } \sim
$$

$$
\subset \text{ } \not\subset \text{ } \subseteq \text{ } \nsubseteq \text{ }
$$

$$
\supset \text{ } \not\supset \text{ } \supseteq \text{ } \nsupseteq
$$

$$
x \in \mathbb R^2
$$



$$
\forall x \in S, \exists y \in S, \text{such that } y > x.
$$



$$
\rightarrow \text{ } \Rightarrow \text{ } \leftarrow \text{ } \Leftarrow \text{ } \leftrightarrow \text{ } \Leftrightarrow \text{ } \rightleftharpoons
$$



$$
\pm \text{ } \mp \times \text{ } \div \text{ } \ast \text{ }
$$

$$
\angle \text{ } \triangle
$$


$$
\vec{x} \text{ } \overrightarrow{ABC}
$$

$$
n \choose k
$$


$$
\prescript{}{V}{[T]}_U
$$

$$
(-\infty, \infty)
$$



$$
\lim\limits_{n\Rightarrow\infty}
$$



$$
\sum_{i=1}^{n}
$$



$$
\int e^x dx
$$



$$
\int_0^2e^x dx
$$



$$
\begin{pmatrix} 1 & 2 & 3 \\ 4 & 5 & 6 \\ 7 & 8 & 9 \end{pmatrix}
$$



$$
\begin{bmatrix} 1 & 2 & 3 \\ 4 & 5 & 6 \\ 7 & 8 & 9 \end{bmatrix}
$$



$$
\begin{vmatrix} 1 & 2 & 3 \\ 4 & 5 & 6 \\ 7 & 8 & 9 \end{vmatrix}
$$



$$
\left( \begin{array}{ccc|c} 1 & 2 & 3 & 4 \\ 5 & 6 & 7 & 8 \end{array} \right)
$$


$$
\begin{equation*}
    A_{m,n} = 
    \begin{pmatrix}
    a_{1,1} & a_{1,2} & \cdots & a_{1,n} \\
    a_{2,1} & a_{2,2} & \cdots & a_{2,n} \\
    \vdots  & \vdots  & \ddots & \vdots  \\
    a_{m,1} & a_{m,2} & \cdots & a_{m,n} 
    \end{pmatrix}
\end{equation*}
$$


$$
f_n(x) = \begin{cases}
             x(n), & \text{for } 0\leq n\leq 1\\
             x(n-1), & \text{for } 0\leq n\leq 1\\
             x(n-1), & \text{for } 0\leq n\leq 1
         \end{cases}
$$

$$

$$


