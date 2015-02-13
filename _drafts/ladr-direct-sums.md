---
layout: post
title: Direct Sums
tags:
- Math
- Linear Algebra
- Linear Algebra Done Right
---
Problem is from Linear Algebra Done Right (2nd Ed) by Sheldon Axler (p.15)

## Definition ##
The direct sum of subspaces $$ U_1,...,U_m $$ is denoted $$ U_1 \oplus ... \oplus U_m $$.

If $$ U_1 \oplus ... \oplus U_m = V $$ for all elements of V, there is a unique
sum $$ u_1 + ... + u_m $$ where $$ u_i \in U_i $$.

## Proposition ##
If $$ U = \{(x,0) \in F^2 : x \in F\} $$ and $$ W = \{(0,y) \in F^2 : y \in F\} $$

Then $$ U \oplus W = F^2 $$

## Proof ##
Let's assume the above is incorrect. That means there must be $$ a + b = c $$
and $$ a' + b' = c $$ where $$ a,a' \in U $$ and $$ b,b' \in W $$ and $$ c \in F^2 $$

Let's rewrite those.

$$ (x, 0) + (0, y) \in (c_0, c_1) $$ and $$ (x', 0) + (0, y') \in (c_0, c_1) $$
where $$ x,x',y,y',c_0,c_1 \in F $$

$$ x + 0 = c_0 $$ and $$ x' + 0 = c_0 $$ and $$ 0 + y = c_1 $$ and $$ 0 + y' = c_1 $$

$$ x = x' = c_0 $$ and $$ y = y' = c_1 $$

Therefore, the proposition we started with is incorrect and $$ U + W $$ is a direct sum.∎
