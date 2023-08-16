# Perplexity

## 1 Language model
Simply put, a language model is a model used to calculate the probability of a sentence. Given a sentence
$$S=W_1,W_2,...,W_k,$$

its probability can be expressed as:
$$P(S)=P(W_1,W_2,...,W_k)=P(W_1)P(W_2|W_1)...P(W_k|W_1,W_2,...,W_{k-1}).$$

That is to say, given the first $k$ words in a sentence, we hope that the language model can predict what the $k+1$th word is, that is, give a distribution of the probability that the $k+1$th word may appear: $P(X_{k+1}|X_1,X_2,...,X_k)$.
## 2 Definition of perplexity
In language models, perplexity is a commonly used automatic evaluation metric. It measures the predictive ability of the model on a given dataset, and the lower the perplexity, the better the model predicts.
The formula for perplexity is as follows:
$$
\begin{equation}
\begin{aligned}
PP(S)&=P(w_1w_2...w_N)^{-{1 \over N}} \\
     &=\sqrt[N]{\prod_{i=1}^N{\dfrac{1} {P(w_i|w_1w_2...w_{i-1})}}}
\end{aligned}
\end{equation}
$$
 Among them, $S$ represents the sentence, $N$ is the length of the sentence, and $P(w_i)$ is the probability of the $i$th word. The first word is $P(w_1|w_0)$, and $w_0$ is START, which means the beginning of the sentence and is a placeholder.
## 3 Influencing factors of Perplexity

- The larger the training dataset, the lower the Perplexity will drop  
- The punctuation in the data will have a great impact on the Perplexity of the model
## References
https://huggingface.co/docs/transformers/perplexity





