---
title: Index Projection for Large Datasets
layout: post
---

There is a large category of computational problems that can be solved by storing a map of truth values.
Since these can be stored in a single bit, it is relatively cost-effective to pre-calculate values for large
combinations of [first-order logical](http://en.wikipedia.org/wiki/First-order_logic) constructs. Even problems
that do not appear to be formally logical in nature can be solved by trading precision in continuous variables
for an acceptably priced system in the end.

> The purpose of this post is to describe an algorithm for solving certain problems by storing large boolean
> indices in economically feasible in memory data grids.

This will be accomplished three steps:

1. An example from middle-school mathematics
2. An example from a real-world problem domain
3. Description of a generalized API (with source code and recipes)

We will finish with an analysis showing that storage can be substantially cheaper in the average case.

Our solution is a mash-up of <a href="http://en.wikipedia.org/wiki/Projection_(mathematics)">mathematical projection</a> with
the [distributed bitmap](http://docs.gigaspaces.com/sbp/distributed-bitmap.html) algorithm.

# Part 1: Storing 3-D coordinates

High school is fun!