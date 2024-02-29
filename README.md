# Structured Adversarial Rewiring for Robust and Sparse Neural Networks
### Benedikt Seidel
### Institute of Theoretical Computer Science Bachelor Thesis Biomedical Engineering Winter Semester 2022/23

### Abstract
Adversarial robust sparse neural networks have been shown to perform astonishingly close to their dense counterparts. Meeting hardware limitations in real world applications, their robustness, performance, and further optimisation for hardware are of main interest. We build up further on the paper Training Adversarially Robust Sparse Networks via Bayesian Connectivity Sampling by [Özdenizci and Legenstein, 2021].[^1] where the neural networks evolve during the adversarial training process using Bayesian connectivity sampling to converge to a optimal solution given a sparsity constraint [see original Github project](https://github.com/IGITUGraz/SparseAdversarialTraining). Based on these principles we here applied a structured rewiring approach using the minimal euclidean distance, which is also known as the l2-norm, to further increase efficiency. Using this new approach, the reinitialisation of weights, which have a value smaller or equal to zero, thus symbolising a dead-end of information flow, occurs close to active weights (values larger than 0). Ultimately, this process causes enforcement of a structure that optimises performance in terms of calculation speed on hardware while still letting the network evolve in a Bayes-optimal manner.


[^1]: Özdenizci, O., & Legenstein, R. (2021). Training adversarially robust sparse networks via Bayesian connectivity sampling. International Conference on Machine Learning, 8314– 8324.
