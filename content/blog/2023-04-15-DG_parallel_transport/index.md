---
title: Connection, Parallel Transport and Geodesis
author: ["admin"]
date: '2023-04-15'
slug: Parallel Transport
categories: []
tags: []
image:
  caption: ''
  focal_point: ''
summary: 'Connection, Parallel Transport and Geodesis'
subtitle: 'Connection, Parallel Transport and Geodesis'
smartDashes: true
---
# Introduction
A vector $\mathbf{X}$ is a direactional derivative acting on $f \in C^{\infty}(M)$ as $\mathbf{X}: f \to \mathbf{X}[f]$. However, there is no direactional derivative acting on a tensor field of type $(p,q)$, which arises naturally from the differential structure $M$. What we need is an extra structure called the connection, which specify how tensors are transported along a curve.

# Covariant Derivative
We first give a heuristic approach to parallel transport and covariant derivatives. As we have noted several times, two vectors defined at different points can not be compared naively with each other since they belongs to different vector spaces, even though they may share the same chart $(U,\phi)$. Keeping this in mind, let us see how the derivative of a vector field in a Euclidean space $\mathbb{R}^m$ is defined, where $m$ is the dimension o fthe manifold. The derivative of a vector field $V = v^u e_u$, where $e_u = \frac{\partial}{\partial x^u}$, with respect to $x^v$ has the $u$-th component.

$$\frac{\partial v^u}{\partial x^v} = \lim_{\Delta x \to 0} \frac{V^u(\ldots,x^v+\Delta x^v,\ldots)}{\Delta x^v}$$

Here, $V^u(\ldots, x^v+\Delta x^v, \ldots)$ is the $u$-th component of the vector field $V$ at point $(\ldots, x^v+\Delta x^v, \ldots)$ and $V^u(\ldots, x^v, \ldots)$ is the $u$-th component of that vector field, $V$, at point $x$. To substract $V^u(x)$ from $V^u(x+\Delta x)$, we have to transport $V^u(x)$ to the point $x+\Delta x$ without change and compute the difference. This transport of a vector is called a *Parallel Transport*.

**Definition**: Parallel transport maps a vector $X$ at point $p$ that lives on a vector space $T_{p}M$ to a vector $Y$ at point $q$ that lives on a vector space $T_{q}M$, mathematically represented as $X \in T_{p}M \to Y \in T_{q}M$.

Intituively, this definition of the parallel transport represents the corresponding vector of $X \in T_pM$ in the vector space $T_qM$. Bascially it is a way of moving a vector over the manifold $M$. 

While defining this parallel transport, we have implicitly assumed that $V\vert_x$ parallel transported to $x+\Delta x$ has the same component $V^{u}(x)$. However, there is no natural way to parallel transport a vector in a manifold and we have to specify *"how it is parallel transported"* from one point to other. Let $\tilde{V}\vert_{x+\Delta x}$ denote a vector $V\vert_x$ parallel transported to $x+\Delta x$. We demand that the components satisfy:

$$
\begin{align} 
\tilde{V}^{u}(x+\Delta x) - V^u(x) &\propto \Delta x  \nonumber \\
\widetilde{(V^u + W^u)}(x+\Delta x) &= \tilde{V}(x+\Delta x) + \tilde{W}^u(x+\Delta x) \nonumber
\end{align}
$$

These condition are satisfy if we take:
$$
\begin{align}
\tilde{V}^u(x+\Delta x) = V^{u}(x) \Gamma_{v\lambda}^u (x) \Delta x^v
\end{align}
$$

where, $x^v=x^v\vert_{x+\Delta x} - \tilde{x}^v\vert_{x+\Delta x}$. The covariant derivative of a vector with respect to $x^v$ is defined by:
$$
\begin{align}
&\lim_{\Delta x^v \to 0} \frac{V^{u}(x+\Delta x)-\tilde{V}^u(x+\Delta x)}{\Delta x^v} \frac{\partial}{\partial x^u} \nonumber \\

&=\lim_{\Delta x^v \to 0} \frac{V^{u}(x+\Delta x)-V^u(x)-V^{\lambda}(x)\Gamma^{u}_{v\lambda}\Delta x^v}{\Delta x^v} \frac{\partial}{\partial x^u} \nonumber \\

&=(\frac{\partial V^u}{\partial x^v} + V^{\lambda}\Gamma_{v\lambda}^u) \frac{\partial}{\partial x^u} \nonumber \\

&= (\nabla_{\frac{\partial}{\partial x^v}} V)^u 
\end{align}
$$

Here, $(\nabla_{e_v} V)^u$ represents the $u$-th component of the covariant derivative along the $e_v$ direaction at point $x+\Delta x$ and the $\nabla$ denotes *connection*, which will be covered later. The quantity in Eqn $(2)$ is a vector at $x+\Delta x$ since, it is a difference of two vectors $V\vert_{x+\Delta x}$ and $\tilde{V}\vert_{x+\Delta x}$ defined at the same point $x+\Delta x$. There are many distinct rules of parallel transport possible, one for each choice of $\Gamma$. If the manifold is endowed with the metric, there exist a predefined choice of $\Gamma$, called Levi Civita Connection.

# Affine Connection
**Definition:** An affine connection $\nabla$ is a map: $\chi (M) \times \chi(M) \to \chi(M)$, or $(X,Y) \to \nabla_{X}Y$ which satisfy the following conditions:
$$
\begin{align}
&\nabla_{X}(Y+Z) = \nabla_{X}Y + \nabla_{X}Z \nonumber \\
&\nabla_{X+Y}(Z) = \nabla_{X}Z + \nabla_{Y}Z \nonumber \\
&\nabla_{fX}(Y) = f \nabla_{X}Y \nonumber \\
&\nabla_{X}(fY) = X[f]Y + f\nabla_{X}Y \nonumber
\end{align}
$$ 
where, $f \in C^{\infty}(M)$, $\chi(M)$ denotes vector field and $X,Y,Z \in \chi(M)$.

Take a chart $(U,\phi)$ with the condition $x=\phi(p)$ on $M$, and define $\Gamma_{uv}^\lambda$ called the connection coefficients by:

$$\nabla_v e_u = \nabla_{e_v} e_u = \nabla_{\frac{\partial}{\partial x^v}} = e_{\lambda} \Gamma_{uv}^\lambda$$

where, $\{e_u\} = \{\frac{\partial}{\partial x^u}\}$ is the cordinate basis in $T_{p}M$. The connection coefficient specify how the basis vectors change from point to point. Let $V=V^ue_u$ and $W = W^ue_v$ be elements of $T_pM$. Then, $\nabla_V W$ is the connection of the vector $W$, at the direaction of the vector $V$. Intuitively, $\nabla_V W$ tells, if we move the vector at $T_pM$ at direction indicated by the vector $V \in T_pM$, what is the difference between vector components and how the basis vector changes. Mathematially, 
$$
\begin{align}
\nabla_V W &= \nabla_{V^u e_u} W^v e_v = V^u \nabla_{e_u} W^v + V^u W^v \nabla_{e_u} e_v \nonumber \\ 
&= V^u (\frac{\partial W^\lambda}{\partial x^u}+W^v \Gamma_{uv}^\lambda) e_{\lambda} \nonumber
\end{align}
$$
Thus the $\lambda$-th component of $\nabla_V W$ is defined as:
$$(\nabla_V W)^\lambda = V^u (\frac{\partial W^\lambda}{\partial x^u} + W^v \Gamma_{uv}^{\lambda})$$

Note that this definition of the connection coefficient is in agreement with the previous heuristic result. By definition, $\nabla$ maps two vectors $V$ and $W$ to  a new vector.

# Parallel Transport and Geodesics

Given a curve in a manifold $M$, we may define the parallel transport of a vector along the curve. Let $c:(a,b) \to M$ be a curve in $M$. For simplicity, we assume a small image is covered by a chart $(U,\phi)$, whoose coordinate is $x=\phi(p)$. Let $X$ be a vector field defined along $c(t)$: $X\vert_{c(t)} = X^u(c(t)) e_u\vert_{c(t)}$, where $e_u = \frac{\partial}{\partial x^u}$. If $X$ satisfies the conidtion: $\nabla_V X = 0$ for any $t \in (a,b)$. $X$ is said to be parallel transported along $c(t)$ and from the chain rule we know, $\frac{d}{dt} = \frac{dx^u(c(t))}{dt} \frac{\partial}{\partial x^u}$, where, $x^u(c(t)) = x^u \circ c$. Thus $V = \frac{d}{dt} = \frac{dx^u(c(t))}{dt} e_u\vert_{c(t)}$ is the tangent vector to $c(t)$. The condition is written as: 
$$
\begin{align}
&\nabla_V X = 0 \nonumber \\
&V^u \frac{\partial X^u}{\partial x^u} + \Gamma_{uv}^\lambda V^{u} X^{v} = 0 \nonumber \\
&\frac{dx^u(c(t))}{dt} \frac{\partial X^{\lambda}}{\partial x^u} + \Gamma_{uv}^{\lambda} V^{u} X^v = 0 \nonumber \\
&\frac{dX^\lambda}{dt} + \Gamma^{\lambda}_{uv} V^u X^v = 0 \nonumber \\
&\frac{dX^\lambda}{dt} + \Gamma^{\lambda}_{uv} \frac{dx^u(c(t))}{dt} X^v = 0 \nonumber
\end{align}
$$
If the tangent vector $v(t)$ itself is parallel transported along $c(t)$, namely if
$$\nabla_V V = 0$$
the curve $c(t)$ is called geodesic. Geodesic are, in a sense, the straighest possible curves in a Reimenian manifold. In components, the geodesic equation becomes:

$$\frac{d^2x^u}{dt^2} + \Gamma^u_{v\lambda} \frac{dx^v}{dt} \frac{dx^{\lambda}}{dt} = 0$$