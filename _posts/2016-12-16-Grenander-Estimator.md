---
layout: post
title: "Grenander Estimator"
date: 2016-12-16 03:22:02
permalink: /second-post.html
---

Grenander estimator is a type of estimator that is first proposed in the field of survival analysis. It is the nonparametric maximum likelihood estimator (NPMLE) of non-increasing density functions defined on <span>$\mathbb{R}^+\cup \{0\}$</span>.

Suppose $f$ is an non-increasing density defined on <span>$\mathbb{R}^+\cup \{0\}$</span>. Let $X_1$, $X_2$, $\ldots$, $X_n$ be an i.i.d. sample from $f$. Let $F_n(x)$ be the empirical cdf. Then

\begin{equation}
F_n(x)=\frac{1}{n}\sum_{i=1}^n 1_{(X_i<x)}
\end{equation}

Let $G_n$ be the least concave marjorant (LCM) of $F_n$, i.e., $G_n$ is the least concave function that is larger than or equal to $F_n$. Then the NPMLE $\hat{f}_n$ of $f$ is the left-hand derivative of $G_n$. 

Note that first $G_n$ is concave, therefore its one-sided derivative always exists. $\hat{f}_n$ can also be defined as follows.
<div>
\begin{equation}
\hat{f}_n(x)=\inf_{w\le x}\sup_{s>w}\frac{\Omega(w)-\Omega(s)}{w-s}
\end{equation}
</div>
Starting from its definition, we can derive certain properties that can be used to prove its consistency and asymptotic distributon. TBC.
