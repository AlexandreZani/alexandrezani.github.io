---
layout: post
title: Some Properties of Sums of Vector Subspaces
tags:
- Math
- Linear Algebra
- Linear Algebra Done Right
---
Problem is from Linear Algebra Done Right (2nd Ed) by Sheldon Axler (p.14)

## Definition ##
The sum of vector spaces $$ U_1,...,U_m $$ is denoted $$ U_1 + ... + U_m $$.

For all $$ u_1 \in U_1,..., u_m \in U_m $$ $$ u_1 + ... + u_m \in U_1 + ... + U_m $$.

## Proposition ##
If $$ U_1,...,U_m $$ are subspaces of vector space $$V$$, then
the sum of the subspaces $$ U_1 + ... + U_m $$ is also a subspace of $$V$$.

## Proof ##
A subspace of $$V$$ has 4 properties which we will attempt to prove.

1. $$ U_1 + ... + U_m $$ is a subset of $$V$$
2. $$ U_1 + ... + U_m $$ contains an additive identity
3. $$ U_1 + ... + U_m $$ is closed under addition
4. $$ U_1 + ... + U_m $$ is closed under scalar multiplication

#### 1. $$ U_1 + ... + U_m $$ is a subset of $$V$$ ####

First, note that since $$ U_1,...,U_m $$ are all subspaces of $$V$$, it must
follow that for all $$ u_i \in U_i $$ it is also true that $$ u_i \in V$$.

Also, recall that $$V$$ is closed under addition, so if $$ x_i,x_i' \in V$$ then
$$ x_i + x_i' \in V$$.

Therefore, $$ u_1 + ... + u_m \in V $$ for all $$ u_1 \in U_1,..., u_m \in U_m $$

And so $$ U_1 + ... + U_m $$ is a subset of $$V$$∎

#### 2. $$ U_1 + ... + U_m $$ contains an additive identity ####

Since $$ u_1,...,u_m \in V $$ there must exist $$0 \in V$$ such that $$ u_i + 0 = u_i $$.

So, $$ u_1 + ... + u_m + 0 = u_1 + ... + u_m $$.

And so $$ U_1 + ... + U_m $$ must contain the additive identity $$0$$∎

#### 3. $$ U_1 + ... + U_m $$ is closed under addition ####

Since $$U_i$$ is closed over addition $$x_i + y_i \in U_i$$ for all $$x_i, y_i \in U_i$$.

So we can take the definition of the sums of subspaces and replace $$u_i$$ with
$$x_i + y_i$$

$$ x_1 + y_1 + ... + x_m + y_m \in U_1 + ... + U_m $$

We rearrange the terms to find

$$ (x_1 + ... + x_m) + (y_1 + ... + y_m) \in U_1 + ... + U_m $$

Or in other words, the sums of subspaces are closed under addition.∎

#### 4. $$ U_1 + ... + U_m $$ is closed under scalar multiplication ####

Vector space $$V$$ is defined over field $$F$$.

Since $$U_i$$ is a subspace of $$V$$, if $$u_i \in U_i$$ and $$c \in F$$ then
$$cu_i \in U_i$$.

Taking the definition of a sum of subspaces and replacing the elements of the
subspaces with scalar multiplied versions of themselves, we have

$$ cu_1 + ... + cu_m \in U_1 + ... + U_m $$.

From there, it is a simple matter to factor out $$c$$ (which we can do thanks
to the distribution law) and write

$$ c(u_1 + ... + u_m) \in U_1 + ... + U_m $$.

Or in other words, the sums of subspaces are closed under scalar multiplication.∎

Having proved the 4 propositions above, we can conclude that a sum of subspaces
of $$V$$ must be itself a subspace of $$V$$.∎
