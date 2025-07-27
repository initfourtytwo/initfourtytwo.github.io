---
layout: post
title: 'Learning to Generalize as a Dev and as a Dad'
category: input
comments: true
---
<p align="center">
  <img src="/assets/certs/ml01.png" alt="Course Certificate" width="400">
</p>
<sub> This post is based on the Coursera course <a href="https://www.coursera.org/learn/machine-learning" target="_blank">Supervised Machine Learning: Regression and Classification</a> by Andrew Ng. </sub>

<br>

I’m two years into my journey as a software engineer and two weeks into my new role as a father. While I’m not actively coding these days, the mindset I built as a developer hasn’t left me. My days now feel like a constant context switch between the async thinking I once used for debugging data pipelines and the non-blocking I/O of a newborn. Surprisingly, I’m finding more overlap than I expected.

Andrew Ng’s lecture on the fundamentals of machine learning isn’t just a technical manual; it’s a toolkit of shockingly relevant mental models. Two concepts, in particular, have felt less like theory and more like a documentary of my current life.

### 1. The Cost Function is Your Honesty Metric

In machine learning, you don’t just build a model; you define a **cost function**, `J(w, b)`, that tells you precisely how wrong your model is. The entire goal of training is to find the parameters (`w`, `b`) that minimize this cost. It’s not a binary pass/fail like a unit test; it’s a continuous, quantifiable measure of error that guides you toward a better solution.

**Insight as a developer:** We talk about "code smells," but that’s subjective. A linter catches style errors, but that’s shallow. The cost function is different. It’s an unforgivingly honest metric. It’s like having a quantifiable way to measure technical debt or design impurity. It forces you to confront not just *that* your code is wrong, but *how* wrong, and provides a clear direction for improvement.

**Insight as a new father:** My son has a cost function: his crying. The parameters are my actions—feeding, burping, swaddling, rocking. The goal is to minimize the cost. The feedback is instant, and there’s no hiding from it. When I make a change and the crying subsides, `J` is decreasing. When it gets louder, I’ve moved in the wrong direction. I am running a real-time, high-stakes gradient descent, 24/7.

### 2. Overfitting is Memorizing the Bug, Not Understanding the System

The lecture explains **overfitting** as creating a model that’s so complex it fits the training data perfectly but fails miserably on new, unseen data. It has memorized the noise, not the signal. It’s brittle.

**Insight as a developer:** This is the most relatable anti-pattern in software. It’s the junior engineer who “fixes” a bug with a hyper-specific `if` statement that checks for a single user ID. It passes the test case from the bug report (the training data) but hasn’t addressed the underlying logic error. It’s a patch that doesn’t generalize. True craftsmanship isn't just making the tests pass; it's building a model of the system in your head that’s robust enough to handle data it hasn’t seen before.

**Insight as a new father:** I’m terrified of overfitting. If I conclude that *this specific cry* always means “hungry,” I’ve overfit. I’m failing to build a generalizable model of my son’s needs. He might be tired, gassy, or just need a change of scenery. By reacting to the noise of a single moment, I risk missing the signal of his overall state, leading to a much higher "cost" for both of us down the line.

---

The point of these models, whether in code or in life, isn't to find a "perfect" set of parameters that never need to change. The data is always shifting. The goal is to build a robust *process* for learning, for listening to the feedback, adjusting the parameters, and trying not to mistake the noise of the moment for the signal of the system.

It's about having the humility to admit your model is wrong and the discipline to keep trying to make it just a little bit better.

**Question for you:** If your life were a model, would it be learning—or just memorizing?