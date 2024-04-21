# Parameter-Estimation
## Prisha Sawhney
## 102116052
## 3CS10

# Maximum Likelihood Estimation (MLE)

## Introduction
Maximum likelihood estimation is a method that determines values for the parameters of a model. The parameter values are found such that they maximize the likelihood that the process described by the model produced the data that were observed.
For a discrete distribution, we maximize the PDF (Probability Density Function) whereas for a continuous distribution, we maximize the PMF (Probability Mass Function)

## Formulae

1. **Likelihood Function**:
   Given a set of observations $$\( \mathbf{x} = (x_1, \ldots, x_n) \)$$ and a set of parameters $$\( \theta \)$$, the likelihood function is defined as:

   $$L(\theta | \mathbf{x}) = \prod_{i=1}^{n} P(x_i | \theta)$$

   where $$\( P(x_i | \theta) \)$$ is the probability (or probability density) of observing $$\( x_i \)$$ given parameters $$\( \theta \)$$

2. **Log-Likelihood Function**:
   To simplify computations, it's common to work with the log-likelihood function, which transforms products into sums:

   $$\ell(\theta | \mathbf{x}) = \sum_{i=1}^{n} \log(P(x_i | \theta))$$

   The log-likelihood function is typically easier to work with when finding the parameter values that maximize the likelihood.

3. **MLE Estimation**:
   The goal of MLE is to find the parameter values that maximize the likelihood function:

   $$\hat{\theta} = {argmax}_{\theta} \ell(\theta | \mathbf{x})$$

