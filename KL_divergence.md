# KL_divergence
## 1 Definition of KL divergence
KL divergence is used to evaluate text generation tasks.
If we have two separate probability distributions $P(x)$ and $Q(x)$ for the same random variable $X$, we can use Kullback-Leibler (KL) divergence to measure the difference between the two distributions.
In machine learning, $P$ is often used to represent the true distribution of the sample, and $Q$ is used to represent the distribution predicted by the model. Then KL divergence can calculate the difference between the two distributions, which is the Loss loss value:
$$D_{KL}(p\Vert q)=\sum_{i=1}^np(x_i)log(\frac{p(x_i)}{q(x_i)})$$
It can be seen from the above formula that the closer the distribution of $Q$ is to $P$, the smaller the value of KL divergence, that is, the smaller the loss value.
It is easy to get from the above formula, the value of KL divergence is non-negative.
The smaller the value of KL divergence, the more similar the distribution $P$ and the distribution $Q$ are; the larger the value of KL divergence, the less similar the distribution $P$ and the distribution $Q$ are.
In text generation, KL divergence is used to measure the difference in the distribution between the generated text and the reference text data.
## 2 Advantages and disadvantages of KL divergence
### 2.1 Advantages of KL divergence
- KL divergence can capture small differences between two distributions, which makes it useful for detecting subtle differences between model-generated text and reference text.
### 2.2 Disadvantages of KL divergence
- KL divergence is very sensitive to noise etc. and may lead to misleading results.
- KL divergence requires knowledge of the true distribution, which is not feasible in many practical situations because the true  distribution is often unknown or difficult to estimate.
## References
https://en.wikipedia.org/wiki/Kullback%E2%80%93Leibler_divergence