# MCC
## 1 Definition of MCC
MCC (Matthews Correlation Coefficient) is an evaluation index used to evaluate binary classification models. 
The calculation formula of MCC is as follows:
$$MCC=\frac{TP \cdot TN-FP \cdot FN}{\sqrt{(TP+FP)(TP+FN)(TN+FP)(TN+FN)}}$$
Among them, 
$TP$: The number of samples that predict the positive class as the positive class.
$FN$: The number of samples that predict the positive class as a negative class.
$FP$: The number of samples that predict the negative class as a positive class.
$TN$: The number of samples that predict the negative class as a negative class.
The value of MCC ranges from -1 to 1, with values closer to 1 indicating better model performance, values closer to -1 indicating worse model performance, and values close to 0 indicating model performance approaching randomness.
## 2 Advantages and Disadvantages of MCC
### 2.1 Advantages of MCC
- It can also provide relatively balanced evaluation results for unbalanced data sets.
### 2.2 Disadvantages of MCC
- MCC is only suitable for binary classification problems. For multi-category problems, it is necessary to perform category-by-category calculations or use other multi-category evaluation indicators.
- Although the value of MCC can indicate the performance of the model, the specific interpretation is not intuitive.
## References
https://scikit-learn.org/stable/modules/generated/sklearn.metrics.matthews_corrcoef.html


