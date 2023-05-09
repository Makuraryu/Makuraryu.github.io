---
layout: post
title: Linear Algebra Homework 4
categories: 数学
description: some word here
keywords: keyword1, keyword2
---


1.

(a).


$$

\begin{eqnarray*}
det(A)&&=\sum_{j_1j_2\cdots j_n}(-1)^{\tau(j_1j_2\cdots j_n)}a_1b_{j_1}a_2b_{j_2}\cdots a_nb_{j_n}\\
&&=\sum_{j_1j_2\cdots j_n}(-1)^{\tau(j_1j_2\cdots j_n)}a_1a_2\cdots a_nb_{j_1}b_{j_2}\cdots b_{j_n}.
\end{eqnarray*}
$$

Since the odd permutation and the even permutation of $ j_1j_2\cdots j_n $ is equal, $ det(A)=0 $.

(b).
$$
\begin{eqnarray*}
det(\lambda I-A)&&=
\begin{vmatrix}
\lambda-a_1b_1&-a_1b_2&\cdots&-a_1b_n\\
-a_2b_1&\lambda-a_2b_2&\cdots&-a_1b_n\\
\vdots&\vdots&\ddots&\vdots\\
-a_nb_1&-a_nb_2&\cdots&\lambda-a_nb_n\\
\end{vmatrix}\\
&&=\lambda^n-\lambda^{n-1}(a_1b_1+a_2b_2+\cdots +a_nb_n).
\end{eqnarray*}
$$
2.
$$
\begin{eqnarray*}
det(I-BA)&&=
det
\begin{pmatrix}
I&0\\
B&I-BA
\end{pmatrix}\\
&&=det\left(
\begin{pmatrix}
I&A\\
B&I
\end{pmatrix}\\
\begin{pmatrix}
I&-A\\
0&I
\end{pmatrix}\\
\right)\\
&&=det\begin{pmatrix}
I&A\\
B&I
\end{pmatrix}\cdot\det\begin{pmatrix}
I&-A\\
0&I
\end{pmatrix}\\
&&=det\begin{pmatrix}
I&A\\
B&I
\end{pmatrix}\\
&&=det\begin{pmatrix}
I-AB&0\\
B&I
\end{pmatrix}\\
&&=det\begin{pmatrix}I-AB\end{pmatrix}
\end{eqnarray*}
$$
3.

"$\Rightarrow$":If $w\in\left\langle v\right\rangle _T$, $w=a_nT^n(v)+\cdots +a_1T(v)+a_0v=(a_nT^n+\cdots+a_1T+a_0)v$, then there is $g(t)=a_nt^n+\cdots+a_1t+a_0$ that $g(T)v=w$.

"$\Rightarrow$":Suppose that $g(t)=a_nt^n+\cdots+a_1t+a_0$, $w =g(T)v$. Then $w\in\langle v \rangle _T$.



6.
$$
\begin{eqnarray*}
&&\rank(ABC)+\rank(B)=\\&&\rank
\begin{pmatrix}
ABC&0\\
0&B
\end{pmatrix}\ge
\rank
\begin{pmatrix}
ABC&AB\\
0&B
\end{pmatrix}
\ge
\rank
\begin{pmatrix}
0&AB\\
-BC&B
\end{pmatrix}\ge\rank(AB)+\rank(BC)\\
\end{eqnarray*}
$$

Therfore, $\rank(ABC)\ge\rank(AB)+\rank(BC)-\rank(B)$.

7.
$$
\begin{eqnarray*}
AB&&=\begin{pmatrix}0&-1&-1\\-1&0&-1\\1&1&2\end{pmatrix}\\
&&\simeq \begin{pmatrix}1&0&0\\0&1&0\\0&0&0\end{pmatrix}\\
\end{eqnarray*}
$$
Therefore, $\rank(AB)=2$.

Sicne $\rank(AB)\le\rank(A)\le 2$, $\rank(AB)\le\rank(B)\le 2$, $\rank(A)=\rank(B)=2$.

There exist $C_{2\times3},D_{3\times2}$, such that 
$$
\begin{eqnarray*}
CA&&=\begin{pmatrix}1&0\\0&1\end{pmatrix}\\
BD&&=\begin{pmatrix}1&0\\0&1\end{pmatrix}\\
\end{eqnarray*}
$$
Then
$$
\begin{eqnarray*}
BA&&=CA(BA)BD\\&&=C(AB)(AB)D\\
&&=C\begin{pmatrix}0&-1&-1\\-1&0&-1\\1&1&2\end{pmatrix}D\\
&&=CABD=(CA)(BD)\\
&&=I_2
\end{eqnarray*}
$$








