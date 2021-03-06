---
title: "Phase retrieval of structured signals"
layout: post
date: 2017-03-12 19:48
# image: /assets/images/machinelearning.jpg
# headerImage: true
tag:
- machine learning
- data science
- phase retrieval
category: project
mathjax : true
---
<font size="+2"> Abstract </font>

<p style='text-align: justify;'>
We consider the problem of recovering a signal $\mathbf{x}^* \in \mathbb{R}^n$, from magnitude-only measurements, $y_i = | \left\langle {\mathbf{a}_i},{\mathbf{x}^*} \right\rangle | $ for $i=\{1,2,\ldots,m\}$. This is a stylized version of the classical phase retrieval problem, and is a fundamental challenge in nano- and bio-imaging systems, astronomical imaging, and speech processing. It is well known that the above problem is ill-posed, and therefore some additional assumptions on the signal and/or the measurements are necessary.</p>

<p style='text-align: justify;'>
In this paper, we first study the case where the underlying signal $\mathbf{x}^*$ is $s$-sparse. For this case, we develop a novel recovery algorithm that we call <i>Compressive Phase Retrieval with Alternating Minimization</i>, or <i>CoPRAM</i>. Our algorithm is simple and be obtained via a natural combination of the classical alternating minimization approach for phase retrieval with the CoSaMP algorithm for sparse recovery. Despite its simplicity, we prove that our algorithm achieves a sample complexity of $O(s^2 \log n)$ with Gaussian measurements $\mathbf{a}_i$, which matches the best known existing results; moreover, it also demonstrates linear convergence in theory and practice. An appealing feature of our algorithm is that it requires no extra tuning parameters other than the signal sparsity level $s$.</p>

<p style='text-align: justify;'>
We then consider the case where the underlying signal $\mathbf{x}^*$ arises from <i>structured</i> sparsity models. We specifically examine the case of <i>block-sparse</i> signals with uniform block size of $b$ and block sparsity $k=s/b$. For this problem, we design a recovery algorithm that we call <i>Block CoPRAM</i> that further reduces the sample complexity to $O(ks \log n)$. For sufficiently large block lengths of $b=\Theta(s)$, this bound equates to $O(s \log n)$. To our knowledge, this constitutes the first end-to-end linearly convergent algorithm for phase retrieval where the Gaussian sample complexity has a sub-quadratic dependence on the signal sparsity level. </p>

You can read the full paper on <a target="_blank" href='https://arxiv.org/abs/1705.06412'> arXiv </a>.

<font size="+2"> Code </font>

You can also find all codes related to the paper on my <a target="_blank" href='https://github.com/GauriJagatap/model-copram'> GitHub page</a>.

<font size="+2"> Publications </font>

G. Jagatap and C. Hegde, "Fast, Sample-Efficient Algorithms for Structured Phase Retrieval", Neural Information Processing Systems (NIPS), December 2017.
[[Poster]({{ site.url }}/assets/poster.pdf)]
