---
layout: post
title: "All the coefficients of the characteristic polynomial are some traces"
date: 2025-01-30
---

If <span markdown="0">\(V\)</span> is an
<span markdown="0">\(n\)</span>-dimensional vector space and
<span markdown="0">\(A: V \to V\)</span> is a linear map, you probably
remember that in its characteristic polynomial
<span markdown="0">\(p_A(t) = \det(tI-A)\)</span>, the coefficient of
<span markdown="0">\(t^{n-1}\)</span> is minus the trace
<span markdown="0">\(\mathrm{Tr}(A)\)</span>, while the constant
coefficient is <span markdown="0">\((-1)^n\det(A)\)</span>.

A question might be: is there a formalism and computing principle
that produces the coefficient of each <span markdown="0">\(t^k\)</span>,
so that the trace and determinant are just two instances of the same
formalism?

I like the surprise in the answer: yes. The coefficients can be
expressed as traces of maps on exterior powers of
<span markdown="0">\(V\)</span>.

Note that <span markdown="0">\(\bigwedge^1 A = A: V \to V\)</span>.
For each <span markdown="0">\(k\)</span>, we can define the induced map

$$
\bigwedge^k A : \bigwedge^k V \longrightarrow \bigwedge^k V
$$

by

$$
v_1 \wedge \dots \wedge v_k
\longmapsto
A(v_1) \wedge \dots \wedge A(v_k).
$$

Choose a basis <span markdown="0">\(e_1,\dots,e_n\)</span> of
<span markdown="0">\(V\)</span>. For an increasing multi-index
<span markdown="0">\(I=(i_1,\dots,i_k)\)</span>, write

$$
e_I = e_{i_1} \wedge \dots \wedge e_{i_k}
$$

and

$$
A(e_I) = A(e_{i_1}) \wedge \dots \wedge A(e_{i_k}).
$$

The vectors <span markdown="0">\(e_I\)</span> form a basis of
<span markdown="0">\(\bigwedge^k V\)</span>. If
<span markdown="0">\(e^I\)</span> denotes the corresponding dual basis
element, the trace of <span markdown="0">\(\bigwedge^k A\)</span> is

$$
\mathrm{Tr}\left(\bigwedge^k A\right)
=
\sum_{\substack{I\text{ increasing}\\ |I|=k}}
e^I\!\left(A(e_I)\right).
$$

In other words, we sum the diagonal coefficients of the matrix of
<span markdown="0">\(\bigwedge^k A\)</span>, just as we do for the
ordinary trace. The difference is that its rows and columns are
indexed by increasing multi-indices rather than single numbers.

For <span markdown="0">\(k=n\)</span>, the space
<span markdown="0">\(\bigwedge^n V\)</span> is one-dimensional, and

$$
\mathrm{Tr}\left(\bigwedge^n A\right)=\det(A).
$$

If we also take <span markdown="0">\(\bigwedge^0 A\)</span> to be the
identity on the one-dimensional space
<span markdown="0">\(\bigwedge^0 V\)</span>, the coefficients of the
characteristic polynomial are given by

$$
p_A(t)
=
\sum_{k=0}^{n}
(-1)^k t^{n-k}
\mathrm{Tr}\left(\bigwedge^k A\right).
$$

It seems that exterior algebra is a convenient framework for working
with the combinatorial attributes of a matrix, since the alternating
properties needed to define those attributes are already built into
wedge products.

Let me mention one other example. The Pfaffian
<span markdown="0">\(\mathrm{Pf}(A)\)</span> of a
<span markdown="0">\(2n \times 2n\)</span> skew-symmetric matrix
<span markdown="0">\(A=(a_{ij})\)</span> is a useful quantity in
geometry and mathematical physics. It is defined by

$$
\mathrm{Pf}(A)
=
\frac{1}{2^n n!}
\sum_{\sigma \in S_{2n}}
\mathrm{sgn}(\sigma)
\prod_{i=1}^{n} a_{\sigma(2i-1),\sigma(2i)}.
$$

If we let

$$
\omega = \frac{1}{2}\sum_{i,j=1}^{2n}
a_{ij}\,e_i \wedge e_j,
$$

then the Pfaffian can also be retrieved from the equality

$$
\underbrace{\omega \wedge \omega \wedge \dots \wedge \omega}
_{n\text{ times}}
=
n!\,\mathrm{Pf}(A)\,
e_1 \wedge \dots \wedge e_{2n}.
$$
