## 1 Definition of CHRF
CHRF is mainly suitable for evaluating text generation tasks.
The general formula for the CHRF score is:
$$chrF \beta=（1+\beta^2）\frac{chrP \cdot chrR}{\beta^2 \cdot chrP+chrR} $$
Among them, $chrP$ is the accuracy, which is the proportion of character-level n-grams that match the generated translation and the reference translation in the generated translation.
$chrR$ is the recall rate, which is the proportion of character-level n-grams that match the generated translation and the reference translation in the reference translation.
 $\beta$ is a parameter that gives $\beta$ times more importance to recall than to precision. If $\beta=1$, recall and precision have equal importance. When $\beta=1$, it is CHRF. When $\beta=2$, it is CHRF2. When $\beta=3$, it is CHRF3.
## 2 Advantages and disadvantages of CHRF
### 2.1 Advantages of CHRF
- CHRF shows good correlations with human judgments
### 2.2 Disadvantages of CHRF
- CHRF is so far tested on only one non-European language 
## References
https://www.researchgate.net/publication/281677746_chrF_character_n-gram_F-score_for_automatic_MT_evaluation
