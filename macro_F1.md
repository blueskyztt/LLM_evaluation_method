# macro F1
# 1 F1
For $N$ classification problems, $F_1$ of category $i$ is defined as:
$$F_1=\frac{2TP}{2TP+FP+FN}$$
Among them,
$TP$: predict category $i$ as the number of samples of category $i$.
$FN$: The number of samples that predict category $i$ as a non-$i$ class.
$FP$: The number of samples that predict non-$i$ classes as class $i$.
# 2 macro F1
macro $F_1$ is used to evaluate multi-classification problems.
For $N$ classification problems, macro $F_1$ is defined as:
$$macro-F_1=\frac{F_1-score_1+F_1-score_2+...+F_1-score_N}{N}$$
Among them, $F_1-score_i(1\leq i \leq N,i \in Z)$ is $F_1$ of category $i$.
Macro $F_1$ treats all categories equally, and its value will be affected by the rarity of the category. Macro $F_1$ is not affected by data imbalance.
# References
https://scikit-learn.org/stable/modules/generated/sklearn.metrics.f1_score.html







