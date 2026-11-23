---
layout: post
title: "Scalar potential and differential forms"
date: 2025-02-22
---

Given an oriented Riemannian manifold
<span markdown="0">\((M^3,g)\)</span> and a vector field
<span markdown="0">\(X\)</span> on
<span markdown="0">\(M\)</span>, we can describe the generalized curl
using differential forms.

Write <span markdown="0">\(X^\flat\)</span> for the one-form
corresponding to <span markdown="0">\(X\)</span> under the metric.
Then

$$
(\nabla \times X)^\flat = \star dX^\flat,
$$

where <span markdown="0">\(d\)</span> is the exterior derivative and
<span markdown="0">\(\star\)</span> is the Hodge star operator
determined by the metric and orientation.

<!--more-->

For example, the vector-calculus identity

$$
\nabla \times \nabla f = 0
$$

becomes

$$
\star d(df)=0,
$$

which follows from <span markdown="0">\(d^2=0\)</span>.

Similarly, the divergence can be written as

$$
\nabla \cdot X = \star d(\star X^\flat).
$$

The identity “the divergence of a curl is zero” translates to

$$
\star d\star(\star dX^\flat)=0.
$$

This again follows from <span markdown="0">\(d^2=0\)</span>, since
<span markdown="0">\(\star\star=\mathrm{Id}\)</span> on forms in an
oriented three-dimensional Riemannian manifold.

Now suppose we have a vector field <span markdown="0">\(E\)</span>
and a Killing field <span markdown="0">\(\eta\)</span> on
<span markdown="0">\(M\)</span>. The Killing condition is

$$
\mathcal{L}_{\eta}g=0,
$$

meaning that the local flow of
<span markdown="0">\(\eta\)</span> preserves the metric.

Consider the one-form

$$
\alpha=\iota_{\eta}(\star E^\flat).
$$

We can ask whether it has a scalar potential: that is, whether there
exists a smooth function <span markdown="0">\(f\)</span> such that

$$
\alpha=df.
$$

A necessary condition is that
<span markdown="0">\(\alpha\)</span> be closed:

$$
d\alpha=d(df)=0.
$$

Equivalently, the vector field corresponding to
<span markdown="0">\(\alpha\)</span> must be curl-free. Locally, this
condition is also sufficient by the Poincaré lemma.

Globally, topology matters: a closed one-form need not have a
potential on every manifold. But on
<span markdown="0">\(\mathbb{R}^3\)</span>, every closed one-form is
exact, so a curl-free <span markdown="0">\(\alpha\)</span> does have a
global scalar potential.
