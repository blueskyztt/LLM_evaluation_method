# MRR
## 1 Definition of MRR
MRR (Mean Reciprocal Rank) is an evaluation metric used to evaluate information retrieval tasks and ranking tasks.
The calculation formula of MRR is as follows:
$$MRR=\frac{1}{S}\sum_{i=1}^S\frac{1}{p_i}$$
Among them, $S$ is the number of samples, which can be understood as the number of user demand items. $p_i$ is the position of the $i$-th demand item in the list of items recommended by the model. If the $i$th demand item is not in the recommendation list, then $\frac{1}{p_i}$ is 0.
The larger the value of MRR, the better the model performs in the ranking task. A perfect ranked list, where all correct answers are in the first position of the ranked list, would have an MRR value of 1.
## 2 Advantages and Disadvantages of MRR
### 2.1 Advantages of MRR
- MRR encourages the model to rank the correct answer at the top of the ranking list, because the higher the correct answer, the larger the value of MRR. This helps to focus the model on the answers the user is likely to be most interested in.
- MRR is calculated in a relatively simple way, which makes its results easy to understand and interpret without complex statistics or calculations.
### 2.2 Disadvantages of MRR
- MRR only focuses on the ranking position of the first correct answer and ignores answers in other positions. If other answers in the ranking list also have significant value to the user, then the MRR may not adequately reflect the performance of the model.
## References
https://en.wikipedia.org/wiki/Mean_reciprocal_rank
