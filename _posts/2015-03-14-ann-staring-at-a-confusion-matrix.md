---
layout: post
title: Staring At Confusion
tags:
- Machine Learning
- Artificial Neural Networks
---
Today, I spent some time implementing a simple feed-forward artificial neural
network in Python using numpy. After feeding it some simple data, I pulled up
the [MNIST handwritten digits dataset|http://yann.lecun.com/exdb/mnist/] and
threw my (slow and buggy) code at it.

I used a single hidden layer composed of 78 neurons and a logistic activation
function. (Both decisions were the result of carefully scrutinizing the thin air
and deftly yanking those ideas as they passed by.) I was able to get to ~20%
correct answers before crashing on some underflow error which is not bad I think
for a little bit of hacking.

But that was not even close to the coolest thing. As I was fitting in small
batches of 1, passing over the data over and over again, I took to printing a
confusion matrix every few 10k batches. This proved very illuminating, or at
least interesting.

A confusion matrix is a diagnostic tool in machine learning and especially when
performing classification problems. It is a table where the rows are the correct
classes and the columns are the predicted classes. The cells contain the number
of predictions for each actual class.

This sounds abstract but all it really is is a table which allows you to see
what your current model thinks the real world looks like. So you can see that
of the samples which are supposed to be '9', 200 are actually identified as a
'7' for instance. In other words, how often the model confused a '9' for a '7'.
You can see where the name came from now.

The cool thing though was watching the model be trained and learn
slowly about different digits. After a single pass over the data, the whole,
dataset was identified as '9'. Slowly, much as a parent has to explain to a
child that "No, the cat, the pidgeon and grandma are not all 'doggie'" the model
started getting better at recognizing other digits. Perhaps most interestingly,
it did not learn all of them at the same time but rather would make progress on
a few at a time. 

Somebody who likes visualizations should visualize this process. Free idea for
anyone who cares to take it.
